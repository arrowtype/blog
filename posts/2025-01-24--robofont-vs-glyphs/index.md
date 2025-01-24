---
title: RoboFont vs Glyphs, and why I use both
description: How and when I use RoboFont vs Glyphs for type design
date: 2025-01-24
tags:
  - type dev
  - type design
  - software
layout: layouts/post.njk
permalink: robofont-vs-glyphs/
# thumbnail: robofont-vs-glyphs/thumbnail.png
---

Wow, it’s been a long time since I last made a blog post. I’ve spent a lot more time [making YouTube videos](https://youtube.com/c/arrowtype) recently, but I just got a question via email, and it’s on a topic I’ve wanted to write about for years, but never found the time for. I apologize up front for any half-baked thoughts here. It seems better to write and share than to keep to myself.

The email:

> Hi Stephen,
> 
> I hope you don’t mind me reaching out! I’ve been following your YouTube channel for the past few years, and I just wanted to say how much I enjoy your content. It’s been fascinating to get a behind-the-scenes look at the typefaces you’re working on, and I’ve found your advice incredibly helpful—it’s made a big difference for me, so thank you!
> 
> I’ve noticed in your videos that you often switch between Glyphs and Robofont, and I was curious if you could share a bit about your typical workflow when creating a typeface with both apps. I completed the OhNo Type Beginner’s Course and tried the 30-day trial of Robofont. While I found it really intriguing, I didn’t get much time to dive deeply into it.
> 
> Thanks so much in advance for any insights you’re able to share, and keep up the amazing work—it’s always inspiring!
> 
> Best Regards,
> Person

You’ve asked a good question. I’d like to someday answer it in a video or blog post, but that would take some thought to do well for a general audience. Then again, I’ll use this email to draft up my thoughts on the subject.

## Some thoughts, loosely organized

To be honest, these days, I mostly work on my own projects in Glyphs. I love both apps, though, and I am so grateful and impressed by their creators, teams, documentation, and support forums.

My general take is: 
- If you are self-teaching, Glyphs is easier to learn and be productive in. If you are following a formal course (such as OHno Type content, or a school program), it’s best to just use whatever software your instruction is using. That way, you can learn from them without a layer of software translation getting in the way.
- Like any art form, the important thing to learn is seeing and making the art, not using the equipment. It’s similar to graphic design, or photography, or painting, or writing, or skateboarding ... equipment is only a means to an end. You could make a great typeface in any font editor that allows you to draw, space, and kern glyphs, then output these into a standard font format.

The best parts of RoboFont:
- Space Center emphasizes and organizes the spacing side of design. 
- MetricsMachine makes kerning a very direct, controllable process. Kerning in glyphs feels somewhat chaotic, by comparison. Part of this is that it leaves the workflow more up to the user, and kerning in Glyphs does become much better once you start to use the right sample text. (Finding or making the right sample text is a bit harder, though.)
- I also like some details of drawing in RoboFont, like the fact that oncurve and offcurve nodes are selected in different ways (so offcurve stay attached to moving oncurve nodes, unless you specifically select them), whereas Glyphs treats them more equally, which is occasionally helpful but often slightly annoying.

The best parts of Glyphs: 
- It’s just so fluid and fast to work in, and so many things that are semi-basic, like duplicating, renaming, and deleting glyphs, scaling the UPM, setting font info data across multiple Masters or Exports, etc... are simple UI operations – whereas many of these things require scripts to do at all in RoboFont, or else to do across multiple sources. 
- RoboFont also historically had some laggy drawing (this may have changed with the latest version, which I think is finally running more natively on Apple M chips, but I haven’t drawn in it much just recently.) 
- Glyphs is also very helpful in writing feature code, automating a lot of it. I’ve found Kern-On very helpful for work-in-progress fonts, which is most of my catalog, so far. I will probably take my fonts back through RoboFont & MetricsMachine, before considering them “v1” / finished, however.
- I slightly prefer [the way “scaling edit” works in Glyphs](https://www.youtube.com/watch?v=MNdCHYEAUZM). It’s one step more powerful than the similar tool in RoboFont, and in Glyphs, it’s available via modifier key hold, whereas it’s a separate tool in RoboFont.

I also have two pretty silly reasons for preferring Glyphs, lately:
1. I like making YouTube videos to share work sessions, and I figure that Glyphs is probably more popular among newcomers to type design, and has a more intuitive design workflow, and therefore, it makes more sense in videos. 
2. I really like tiny keyboards. (Why? A proper explanation would take a separate blog post, but: they’re portable, customizable, and simply cute.) and these tend to eschew the number row, making numbers available through holding a layer key. This is great in normal operation (and it even allows you to fit a numpad on a layer, which I highly prefer to a typical keyboard). However, RoboFont tools are selected with number keys, and I haven’t ever found a way around this, so it’s a two-key operation to switch tools, which is slightly annoying.

A discussion of font editors should also take file formats into account, as these are a big part of the experience. The best part of the .UFO file format (used in RoboFont) is how simple it is to edit via Python scripting, with no desktop app required.
- This is also somewhat possible via glyphsLib, but this library is weird in that it only supports glyphs3 files in an experimental way, in a development branch. This is annoying, as the glyphs3 format has existed for over 4 years. Running glyphsLib on a glyphs3 file will break certain things. The saving grace is how easy it is to edit whole families in Glyphs with the UI, but if you are trying to fix something basic (like a copyright string) in multiple families, UFOs are much nicer.
- I also appreciate how the UFO format is handled in Git, which I use for every project. Now that Glyphs offers the .glyphspackage file format, though, it’s basically just as good (or maybe even slightly better?) on this front.

In the past, I’ve had families that I started in RoboFont, but then moved to Glyphs.
- In [Shantell Sans](http://shantellsans.com), the design started in RoboFont in part because I was getting better results from its Outliner plugin than the Glyphs equivalent. (I was drawing single strokes, then expanding these to filled shapes.) I later moved to Glyphs to take advantage of Kern-On. But, the build process actually exports back to UFOs so it can manipulate these to create shifted glyph alternates, etc. This is partly explained in this lecture.
- In [Name Sans](http://arrowtype.com/name-sans), I designed pretty much the full family as an upright/Roman-only system, but I knew I needed Italics eventually. Once I was pretty confident in the full design, I used a script to prep Italics, then edited these UFOs directly in Glyphs so I could clean up the skewed outlines as quickly and fluidly as possibly. With that many edits, Glyphs was definitely more efficient. But, I ultimately kept the family as a UFO-based project, as I had figured out all my technical stuff there already.

There are certain things that can only be done in Glyphs, and certain things that can only be done in UFOs.
- Glyphs has various “smart” features like corner components that require Glyphs to interpret, and Glyphs to build into output OTF/TTF fonts. My take is that these can be useful in an early design phase, but shouldn’t really be trusted in a final font source, because they are fragile between software versions, and don’t allow full control over the actual shapes. But, different designers have different opinions.
- There are some aspects of creating variable fonts / large families that work better in UFOs + Designspaces, where you have more precise control because you are closer to the final products. (Literally: when you build from Glyphs sources using FontMake, it first outputs to UFOs, then builds fonts from there.) A specific feature that I don’t think works properly from Glyphs (neither via Glyphs build or FontMake build) is giving a glyph both Intermediate layers (e.g. to adjust shaping at an intermediate weight) and Alternate layers/glyphs (usually swapped to via an RVRN feature, or rules in a designspace). This [miiight be fixed](https://github.com/googlefonts/glyphsLib/issues/1050) in a branch of glyphsLib, though? I’m not quite sure at the moment. 

There are two basic ways to shift between apps:
1. Install glyphsLib, and use glyphs2ufo and/or ufo2glyphs on the command line.
2. Just open UFOs or an entire designspace doc in Glyphs, or export to UFOs from Glyphs. (It doesn’t seem like you can save from Glyphs to a designspace, in the app – you’d have to do this with glyphsLib, or set up the Designspace separately.)

Glyphs files tend to have extra data, which can be good and bad when exporting to/from UFOs. It’s handy to use Git when doing this kind of back-and-forth, so you can see what is changing.

## Sign off

Hope some of that is helpful, and sorry if I’ve just dropped too many technical things without full explanation! It’s a pretty deep subject, and something I continue to learn about all the time. 

All the best in your projects and type design journey!