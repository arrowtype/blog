---
title: Getting started in Type Design (and possible next steps)
description: An article linking to helpful resources for people looking to get started in type design
date: 2020-05-01
tags:
  - tips
  - tools
layout: layouts/post.njk
permalink: getting-started/index.html
---

So, you’re interested in type design, but you are still figuring out how & where to start or get to the next step. This post is a non-exhaustive attempt to share an overview of how you might learn some basics, how you can get started with font editing software, and where you might consider growing your skills after that. 

This post reflects my bias and (some of) my personal experience, and it completely skips important topics like formal education, calligraphy and **sketching**, bezier drawing tips, and more. This article started as an email listing my favorite RoboFont extensions, and then I thought that it would be worth sharing publicly, instead. It is something which will evolve over time.

## General learning

### Useful Internet resources

- The format of this post is somewhat informed by James Edmonson’s (OHno Type) blog post [Getting Started in Type Design](https://ohnotype.co/blog/getting-started). It includes some useful topics I haven’t included in this post. Also, The next two resources in this list are borrowed directly from it.
- [Type Basics, by Underware](http://www.typeworkshop.com/index.php?id1=type-basics). Not a flashy layout, but a serious of extremely helpful drawings with important lessons for type design.
- [Type Mechanics, by Tobias Frere-Jones](https://frerejones.com/blog?tag=Education%20Mechanics). More useful explanations of some visual things that are important to know, but not always obvious.
- [Spacing](https://ohnotype.co/blog/spacing) & [Proofing](https://ohnotype.co/blog/proof-it), also by OHno Type, are two excellent, practical posts for subjects beyond drawing that are super significant to good type design.
  - I have collected a few useful spacing tests at https://github.com/arrowtype/spacing

### Useful books

- For the very basics of letter-shaping, the first book I read in type design was really helpful: [Designing Type, by Karen Cheng](https://yalebooks.yale.edu/book/9780300111507/designing-type). It goes through each letter, showing their general forms via classic typefaces. Not necessarily useful if you have been designing for awhile, but it helped me gain an overall awareness of what is “general practice” that I found really helpful as a beginner.
- For deeper (but still approacheable) reflections on theory, [The Theory of Type Design, by Gerard Unger](https://www.amazon.com/Theory-Type-Design-Gerard-Unger/dp/9462084408) is a great book with a beautiful set of visual examples and references.
- For one useful theory of approaching type design in a systematic way, [The Stroke, by Gerrit Noordzij](https://www.typotheque.com/books/the_stroke) is a classic.


## My favorite font editors: Glyphs & RoboFont

Making type is involves many things. Digital drawing is only one of the areas to master, but it is a core aspect. When I started out as a student in graphic design, I remember thinking, “Wait, Adobe doesn’t just make a type editor??” I was daunted by what seemed like a confusing world of indie apps, and not sure what to use and how to get started. Here is what I would tell someone in that position, today.

[Glyphs](http://glyphsapp.com/) & [RoboFont](https://robofont.com/) are the two most-commonly used editors in professional type design, and also the two editors I have the most familiarity with. This post isn’t really a comparison of the two; I 100% recommend either of them. 

Generally, Glyphs is more approacheable and feels more “Mac-like” as an app: it is quite approachable and does some helpful things for you. RoboFont is a bit more intimidating to get started with, but provides more flexibility because it is less “opinionated” about what tools you need.

I got started in Glyphs, and I now use RoboFont more. I use RoboFont largely because I like the way it encourages me to think about my workflow and consider what a given type family should be like. RoboFont is somewhat nicer for scripting (partly because it uses Python3), and its format is nicer for Git versioning. I also really like its approach to spacing. 

To be honest, my initial motivation to use RoboFont was that most of my heroes in type use it. A couple years in, however, I have become more fluent in drawing with it, and I like it for many reasons – [here’s more on my favorite extensions & tools to use with RoboFont](../robofont-tips). But, there are also many professionals who use Glyphs to make amazing type. Some studios even use both, though this takes some scripting to handle well. 

I have a lot of love for both apps!

## Alternative editors

- [Glyphs Mini](https://glyphsapp.com/glyphs-mini) has many of the features of Glyphs, with the main exception that it only allows 1 master per font (meaning that if you want to make multi-style typefaces, you will want to upgrade. If you are just drawing a single font, doing lettering, or making a logotype, this is about 5x better for drawing letters than Adobe Illustrator
- [FontLab 7](https://www.fontlab.com/font-editor/fontlab/) has some amazing features and I’m sure people are doing good work on it, though I don’t have much personal familiarity with it. Unlike RoboFont & Glyphs, it is available on Mac *and* Windows, so if you’re on a Windows machine, this might be the app for you.
- [FontForge](https://fontforge.org/en-US/) is an open-source font editor which is cross platform and freely available for Mac, Windows, and Linux. I also don’t have much familiarity with this one, but if you are just looking to explore type design without a big initial investment, this might be the perfect solution.

## Getting started in Glyphs

Glyphs does an amazing job in tutorials & support. Check out https://glyphsapp.com/tutorials for advice on getting started. The [Glyphs Forum](https://forum.glyphsapp.com/) provides excellent support, often faster than seems reasonably possible. There are great extensions for Glyphs, but I don’t really know much about these – see https://glyphsapp.com/extend for some good suggestions.

## Getting started in RoboFont

Due to its unopinionated nature, RoboFont can an intimidating program to get started in,. If you are just getting started (or if you’re just curious to see what I like), here’s some basic advice that may help get you off the ground.

The docs are pretty good at https://robofont.com/documentation/introduction/. Read through these, and keep clicking to the next page. Don’t get distracted by all the links in each page on the first read through – consider clicking them on subsequent reads.

If you have questions, the RoboFont Forum is very helpful: https://forum.robofont.com/. They usually answer questions within a day (many questions, of course, are already answered if you search for them).

### RoboFont Extensions

In an earlier version of this post, I had tips here on some of my favorite RoboFont extensions. However, I have since added more extensions and detail in a separate post on [RoboFont Tips](../2020-12-11--robofont-tips).

## Other useful tools:

- [Alphabet Type’s CharSet Builder](https://www.alphabet-type.com/tools/charset-builder/) is a really handy tool to create character sets (an important early hurdle in RoboFont)
- [FontGoggles](https://fontgoggles.org/) is a really good tool to quickly view fonts, useful to quickly test font builds. It can also be useful as a way to quickly compare how various fonts handle the design of certain characters, etc.
- [Type-X](https://chrome.google.com/webstore/detail/type-x/bfnfnnicdjkkialkldogjjmmfeiopbin) is a tool I designed and built in collaboration with Roel Nieskens. It allows you to quickly & easily test any font on your system on (almost) any website. This can help you to judge your work in different web contexts (and can be a fun motivator to improve what you’re working on).


## Technical areas

- **Version control:** Git is pretty challenging to get started with, but extremely useful for all areas of technical design & code. 
  - [Git for Humans](https://abookapart.com/products/git-for-humans) is a a great introduction to using Git. 
  - GitHub is the most popular Git website, and they also have a nice [getting-started guide](https://guides.github.com/introduction/git-handbook/).
- **Scripting:** scripting makes it possible to work efficiently with complex fonts, and not have to rely on someone else building everything for you. 
  - RoboFont has a good [guide to getting started](https://robofont.com/documentation/building-tools/), including a great guide to starting with Python, the most common scripting language used for font design & development (and many other things, like software development, data analysis, and more).
  - [DrawBot](https://www.drawbot.com/) makes it possible to create graphic designs & animations with Python. Not only is this a fun way to learn Python, but it can be a genuinely useful tool to generate proofs, books, or animations that (sometimes) would be impossible to create with more-general design tools
  - On the Glyphs side, they provide a very handy 4-part [Scripting Glyphs](https://glyphsapp.com/tutorials/scripting-glyphs-part-1) tutorial.
- **Mastering:** A topic as big as type design itself. Here are a few places you might get started.
  - [OpenType Cookbook](http://opentypecookbook.com/) is a friendly introduction to scripting OpenType features. It is very approacheable, and helps answer questions like “How can I add automatically-swapping alternates to a font?” and “How can I make ligatures work how I want?”
  - [The OpenType Spec](https://docs.microsoft.com/en-us/typography/opentype/spec/) answers basically every question about what is possible in fonts, such as “What are the possible [OpenType feature tags](https://docs.microsoft.com/en-us/typography/opentype/spec/featuretags) and what do they mean?” and “What are the [valid values for font variation axes](https://docs.microsoft.com/en-us/typography/opentype/spec/dvaraxisreg)?”
  - [FontMake](https://github.com/googlefonts/fontmake/) is a great way to get started into building fonts in a way that gives you more control than tools like Batch can (you can even use shell scripting as a quick way to create handy workflows to build & sort fonts). 
  - [FontTools](https://fonttools.readthedocs.io/en/latest/) provides a bunch of Python-based tools to help handle font files – of note, TTX makes it easy to inspect built OTF/TTF font files, TTFont can make it efficient to edit font data, and 
