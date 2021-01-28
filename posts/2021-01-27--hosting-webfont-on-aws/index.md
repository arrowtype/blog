---
title: Hosting licensed fonts on AWS S3 for open-source websites
description: How to use Amazon Web Services to host a font
date: 2021-01-27
tags:
  - web dev
  - webfonts
layout: layouts/post.njk
permalink: host-webfont-on-aws/
---

In some situations, you may need to use a font on the web, but may not be able to host it alongside your web code. In this case, you can host the font on AWS and call it in as a URL in your `@font-face` CSS!

For example, you may wish to use a web-licensed font with a project that is openly-hosted on GitHub or with a project made on a service like CodePen or JSfiddle. **If your font license allows it**, this can be a nice solution to an otherwise tricky problem. Note: licensing will vary between typefaces and type foundries – read your license or email the type foundry if you aren’t sure!

With the S3 Buckets feature of Amazon Web Services (AWS), this is relatively easy & very inexpensive – unless you are making a hugely-popular website, perhaps. You can (and should) configure it to only work on specific domain URLs, so you don’t break your licensing) or end up paying for other people to use your font hosting!). Here’s how.

## Make your S3 Bucket

1. Register for AWS, then Sign into the Management Console, search for `buckets` and click on **Buckets S3 feature**
2. Click **Create Bucket**
3. Give the bucket a name (e.g. `arrowtype`) and select a region that you think is closest to you / most of your users
4. Uncheck **Block all public access** and check the box for “I acknowledge that the current settings might result in this bucket and the objects within becoming public.”
5. Maybe enable versioning
6. Scroll to the bottom and click **Create bucket**

## Upload your font

1. Go into your new bucket, and click **Upload** then **Add files**, then select and upload your woff2 font file.
2. Click on the file within the bucket, then find **Object actions > Make Public**, so you can access this from your CSS later (don’t worry; the next step will prevent other sites from using it)

## Edit CORS on the bucket

1. Navigate back to the top level of your bucket
2. Scroll to the “Cross-origin resource sharing (CORS)” section, then click **Edit**
4. Set CORS permissions to allow your specified URL(s) to access the objects in the bucket, similar to the JSON shown below. You can use a wildcard (`*`) to allow subdomains, like `https://*.arrowtype.com`. Note that I also include `http://localhost:8080`, the URL which my local-development builds get served to. Replace this with the localhost port number(s) you need to support.

```json
[
    {
        "AllowedHeaders": [
            "*"
        ],
        "AllowedMethods": [
            "GET"
        ],
        "AllowedOrigins": [
            "https://*.arrowtype.com",
            "https://arrowtype.com",
            "http://localhost:8080"
        ],
        "ExposeHeaders": []
    }
]
```

## Get your font object’s URL

1. Go back into the bucket’s “Objects” tab, and click on the file name of your font.
2. Find and copy the “Object URL,” which will look something like `https://arrowtype2.s3.amazonaws.com/name_sans-variable.woff2`. 

Note: because of the CORS configuration for this URL, you can’t use it on other websites, though you could use it in local development if you really wanted to ... but honestly, please just [buy your own license](https://name.arrowtype.com) if you want to use it – while it’s still in early access, it’s available at a steep discount! Or, use another font – there are many great type options in the world, both free and paid!

## Set your CSS so local fonts don’t interfere with your development

In your CSS, you can use a font’s basic family name in order to just use a local copy of that font. This can make fonts appear more quickly for users, if those users already have that font on their system. However, especially with newer fonts, this may cause problems. How do you know that your users will have the latest version of a font? Often, the OS will serve an unintended font style, even if it does have the latest version.

So, I often make sure to use a name that specifically _won’t_ call a local file. I do this either by removing spaces or adding a suffix like ”VF“.

```css
@font-face {
  font-family: 'NameSansVF';
  font-weight: 1 1000;
  src: url("https://arrowtype.s3-us-west-2.amazonaws.com/name_sans-variable.woff2");
}
html {
 font-family: 'NameSansVF', sans-serif;
}
```

Your font should now work locally and also in deployment. Of course, the only way to know is to deploy the site and test it on a few different devices!

Additionally, the font is (relatively) safe from being directly used on any site that just copies your CSS. You can verify this out by [trying it on CodePen](https://codepen.io/thundernixon/pen/LYbPGGd?editors=1100), where it shouldn’t work (unless you allow CodePen URLs in your CORS settings).

## To update the font

If you need to update the font version on S3 in the future, you can simply repeat the process of uploading a file. 

Just remember to also follow the **Make Public** steps, or things will break!

## But what if fonts were already in a public Git repo?

This is a [pretty big problem](https://pixelambacht.nl/2017/github-font-piracy/), but luckily, it’s not too hard to fix.

You can use a tool called BFG to remove them – even [GitHub recommends this tool](https://docs.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository).

1. Make a backup copy of your project before using the BFG, in case you mess something up!
2. Download the latest release from [the BFG website](https://rtyley.github.io/bfg-repo-cleaner/). 
3. Open a terminal, navigate to your project’s root, point to the downloaded BFG file, and use the `--delete-files` option to delete the font filename you’d like to keep private:

```bash
cd ~/code/blog-11ty # change to the root of your web project
java -jar ~/Downloads/bfg-1.13.2.jar --delete-files name_sans-variable.woff2
```

4. Use `git push --force` to force push the edited Git history to your repo.

## Happy webfonting!

This specific workflow is fairly new to me. Did I forget to describe a step? Did I say anything inaccurate? Feel free to let me know! I’m [on Twitter](https://twitter.com/ArrowType), and this blog has open [Issues on GitHub](https://github.com/arrowtype/blog/issues).
