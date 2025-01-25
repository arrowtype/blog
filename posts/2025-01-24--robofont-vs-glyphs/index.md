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

Wow, it’s been a long time since I last made a blog post. I’ve spent a lot more time [making YouTube videos](https://youtube.com/c/arrowtype) recently, but I just got a question via email, and it’s on a topic I’ve wanted to write about for years but never found the time for.

I apologize up front for any half-baked thoughts here. I have incomplete knowledge and biases from my specific projects and opportunities. Still, this is a topic that deserves attention, so it seems better to write about and share than to keep to myself.

The email:

> Hi Stephen,
> 
> I hope you don’t mind me reaching out! I’ve been following your YouTube channel for the past few years, and I just wanted to say how much I enjoy your content. It’s been fascinating to get a behind-the-scenes look at the typefaces you’re working on, and I’ve found your advice incredibly helpful—it’s made a big difference for me, so thank you!
> 
> I’ve noticed in your videos that you often switch between Glyphs and RoboFont, and I was curious if you could share a bit about your typical workflow when creating a typeface with both apps. I completed the [OHno Type Beginner’s Course](https://ohnotypeschool.teachable.com) and tried the 30-day trial of Robofont. While I found it really intriguing, I didn’t get much time to dive deeply into it.
> 
> Thanks so much in advance for any insights you’re able to share, and keep up the amazing work—it’s always inspiring!
> 
> Best Regards,
> Person

Clearly, this person never specifically asked for “RoboFont vs Glyphs” as a head-to-head comparison, and I do try to address their question at the end. But, I think they may have the deeper question of “What app should I invest my time into?” which is a valid question.

I sent them a quick reply, and I’ve cleaned it up a bit for this blog post.

## My context

I work in both apps quite often due to a quirk of my primary job: I help other people make and finish fonts. This involves building font “binaries” like OTFs and TTFs, using tools like [FontMake](https://github.com/googlefonts/fontmake), checking those outputs with tools like [Font Bakery](https://github.com/fonttools/fontbakery), and fixing problems that exist. Fixing problems often involves using either RoboFont or Glyphs (or some combination of the two) to adjust font info or design data. Sometimes, it means manipulating source files or font binaries with Python-based tools such as [ufoLib2](https://github.com/fonttools/ufoLib2), [glyphsLib](https://github.com/googlefonts/glyphsLib), and [TTfont](https://fonttools.readthedocs.io/en/latest/ttLib/ttFont.html).

Let’s take a step back from all the technical stuff, though...

### My work background

I drew my first font in about 2012, in [Fontographer](https://en.wikipedia.org/wiki/Fontographer), which was mostly a terrible choice. This software was first made in the ’80s and seemingly hadn’t changed much by 2012. This consistency is great for those who like to draw in Fontographer but not as intuitive for someone new to drawing type. [Glyphs](https://glyphsapp.com) was already around, and it would have been the much better choice in most ways. I moved to Glyphs for fonts I drew in 2013–2014 for my undergrad Senior thesis, and I found it so empowering and fun to use. (On the other hand, there is a lot of educational value and long-term power in simpler tools that don’t gloss over what you are doing with too much automation. In a sense, this push-and-pull between control-vs-speed is at the heart of the RoboFont-vs-Glyphs question! This isn’t to say that RoboFont is slow, or that Glyphs doesn’t give control... it’s more that, out-of-the-box, each app prioritizes one side or the other of that tradeoff.)

I later got a Masters degree in type design at [KABK TypeMedia in the class of 2018](http://2018.typemedia.org). There, I transitioned to [Robofont](https://robofont.com), as most of my teachers and classmates used it. (After all, RoboFont started as a TypeMedia project, and a few of the instructors are actively involved in the creation and development of the UFO and Designspace formats.)

After TypeMedia, I worked as a freelancer for Google Fonts, building fonts made by others and preparing them for publication on Google Fonts. These fonts were mainly in the Glyphs format, but some were built with UFOs and a Designspace (i.e., created in RoboFont). I was also hired by Google Fonts to finish my TypeMedia thesis project, [Recursive](https://www.recursive.design), and publish it as an [OFL](https://openfontlicense.org) project. Recursive was a UFO+designspace project from start to publication.

These days, [in my personal and commissioned font projects](https://www.arrowtype.com), I spend most of my time working in Glyphs. 

I also currently work part-time as a font engineer at [The Type Founders](https://thetypefounders.com), where I once again take fonts designed by others and build/prepare these for publication.

Along the way, I’ve also freelanced for indie foundries, helping them set up build & QA processes and finish their fonts built in either RoboFont or Glyphs.

### All font editors are beautiful

I love both RoboFont and Glyphs, and I am so grateful and impressed by their creators, teams, documentation, and support forums. I’ve met and conversed with the people who have built and supported both apps; they are all lovely people.

I should also acknowledge that I’m leaving a notable app out of this discussion: [FontLab](https://www.fontlab.com). I simply don’t have much personal experience with it. If you’re primarily a Windows user, it seems to be the main option. It is the primary tool of one of my favorite type designers, [Matthijs Herzberg](https://www.herzbergdesign.com). Even on Mac, where Glyphs and RoboFont get most of the attention, FontLab is a powerful option. However, it’s not as popular with the designers and companies I have worked for so far, so my main experience with it is converting FontLab sources to UFOs and then building fonts from there.

There are still more apps for creating and editing fonts, but a complete survey of tools isn’t the point of this article.

## Which app is better?

Like most things, it depends.

My high-level take is: 
- If you are self-teaching, Glyphs is easier to learn and be productive in. If you are following a formal course (such as the OHno Type course or a school program like TypeMedia or Type@Cooper), it’s best to use whatever software your instructor uses. That way, you can learn from them without a layer of software translation getting in the way.
- Like any art form, the vital thing to learn is seeing and making the art, much more than learning to use the equipment. In this sense, type design is similar to graphic design, photography, painting, writing, playing guitar, skateboarding, or a million other pursuits ... equipment is only a means to an end. Your choice of gear may make specific tasks more straightforward or efficient, but gear is seldom the limiting factor. A pro can do good work on almost anything, whereas a beginner can’t buy their way to knowledge. You could make a great typeface using any font editor that allows you to draw, space, and kern glyphs, then output these into a standard font format.

## The best parts of either app

The best parts of RoboFont:
- Space Center emphasizes and organizes the spacing side of design, which is easy to overlook but arguably the most important aspect of type design. 
- MetricsMachine makes kerning a very direct, controllable process. (Kerning in Glyphs feels somewhat chaotic by comparison. Part of this is that it leaves the workflow more up to the user, and kerning in Glyphs becomes much better once you use the right sample text. Finding or making the right sample text is a bit harder, though.)
- I also like some very specific details of drawing in RoboFont, like the fact that [on-curve and off-curve points](https://doc.robofont.com/documentation/topics/understanding-contours/#points) are selected in different ways (so offcurve nodes stay attached to moving on-curve points, unless you specifically select the offcurves). By contrast, Glyphs treats on-curve and off-curve points more equally, which is occasionally helpful but often slightly annoying. This is hard to explain, and it might not make sense to anyone reading this, and that is okay.
- If you want to learn about scripting in Python, RoboFont makes this more approachable than Glyphs, mainly due to a more intuitive file structure: each “master” drawing of a typeface is its own .ufo package, whereas a Glyphs file puts all masters into a single package. The flip side of this benefit, though, is that you basically *have to* embrace code to be effective in RoboFont.

The best parts of Glyphs: 
- It’s just so fluid and fast to work in, and so many things that are semi-basic, like duplicating, renaming, and deleting glyphs, scaling the UPM, setting font info data across multiple Masters or Exports, etc... are simple UI operations – whereas many of these things require scripts to do at all in RoboFont, or else to do across multiple sources. 
- RoboFont also historically had some laggy drawing (this may have changed with the latest version, which I think is finally running more natively on Apple M chips, but I haven’t drawn in it much just recently.) 
- Glyphs is also very helpful in writing feature code, such as language localization, numeral styles, stylistic sets, and more. 
- I’ve found [Kern-On](https://kern-on.com) very helpful for kerning work-in-progress fonts, which is most of my catalog, so far. However, I will probably take my fonts back through RoboFont & MetricsMachine before considering them “v1” / finished. Like anything involving “AI,” Kern-On results in a slightly amorphous output that is hard to fully understand and trust.
- I slightly prefer [the way “scaling edit” works in Glyphs](https://www.youtube.com/watch?v=MNdCHYEAUZM). It’s one step more powerful than the similar tool in RoboFont, and in Glyphs, it’s available via modifier key hold, whereas it’s a separate tool in RoboFont. (For what it’s worth, it seems like FontLab may have an even better “power nudge” tool, though I don’t have much personal experience with it.)
- If you want to avoid scripting, Glyphs will allow you to get further with no code. Glyphs is still a great choice if you want to embrace scripting, but it may be more challenging for beginners.

### File formats: .ufo vs .glyphs

A discussion of font editors should also consider file formats, as these are a big part of the experience. The best part of the .UFO file format (used in RoboFont) is how simple it is to edit via Python scripting, even with no desktop app required. You can write a Python script to make an edit to one or many UFOs, and run that script in a terminal, without ever opening RoboFont.

This kind of “remote” editing operation is also (somewhat) possible via glyphsLib. Still, the glyphsLib library is a bit confusing in that it only supports glyphs3 files in an experimental way, in a development branch. (This is somewhat annoying, as the glyphs3 format has existed for over 4 years. But, I can’t really blame anyone for this, as it is amazing that any of this software exists at all, and I know that everyone involved in glyphsLib is busy with other work that is probably more vital to their paying rent, etc.) Running glyphsLib on a glyphs3 file will break certain things. The saving grace is how easy it is to edit whole families in Glyphs with the UI, making scripting less of a requirement for most projects. However, if you are trying to fix something basic (like a copyright string) across multiple families, UFOs are much more convenient.

There is also a philosophical difference between UFO and Glyphs formats: the UFO is an open standard, whereas Glyphs is made and controlled by a private company. So, the UFO format can be read and edited by many apps, while the Glyphs format can only really be edited by Glyphs. As part of this, it is arguably more future-proof to work in UFO files, because your ability to use them doesn’t hinge on the continued success or business model of a single company. On the flip side, glyphsLib is mostly very good at converting Glyphs files to UFOs, so even if Glyphs were e.g. bought by Adobe, you could (in theory) convert your Glyphs files from 2024 to UFO files in 2030, using the right version of glyphsLib. If one of the formats *were* to come under the control of a company like Adobe and locked down into something much more proprietary, locked behind a subscription, it would be a different story.

Finally, I appreciate how the UFO format is handled in Git, a tool I use for every project. A UFO is made of many separate files, so it’s easier to see what changed in a given Git commit. Now that Glyphs offers the .glyphspackage file format, however, it’s basically just as good (or maybe slightly better?) on this front.

### Silly, personal reasons

I also have two pretty silly reasons for preferring Glyphs for drawing fonts:
1. I like making YouTube videos to share work sessions, and Glyphs is probably more popular among newcomers to type design. I also believe it has a more intuitive design workflow for a casual observer, and therefore, it makes more sense in videos. 
2. I really like [tiny keyboards](https://www.instagram.com/p/C4jI-9NRPDj/?img_index=1). (Why? A proper explanation would take a separate blog post, but they’re portable, customizable, and quite simply... I just love how they look and feel to use.) Such keyboards tend to eschew the number row, making numbers available by holding a layer key. This is great for day-to-day computer operations, and it even allows you to fit a numpad on a layer, which I highly prefer to a typical keyboard. Regarding font editors, however: RoboFont’s essential tools are selected with number keys, and I haven’t ever found a way around this. So, it’s a two-key operation to switch tools, which is slightly annoying. I prefer tool selection via alpha keys.

### Projects where I’ve gone back-and-forth

In the past, I’ve had families that I started in RoboFont but then moved to Glyphs. I’ve also had families that are primarily made in RoboFont, but taken into Glyphs for a specific operation, then moved back into RoboFont. In the future, I will probably have families that started in Glyphs, but end up in RoboFont.
- In [Shantell Sans](http://shantellsans.com), the design started in RoboFont, partly because I was getting better results from its Outliner plugin than the Glyphs equivalent. (I was drawing single strokes, then expanding these into filled shapes.) I later moved to Glyphs to take advantage of Kern-On. But, the build process actually exports back to UFOs, so it can manipulate these to create shifted glyph alternates, etc. This is partly explained in this lecture.
- In [Name Sans](http://arrowtype.com/name-sans), I designed almost the full family as an upright/Roman-only system first, but I knew I needed Italics eventually. Once I was confident in the full design, I [used a script to prep Italics](https://www.youtube.com/watch?v=vmNsWayJp9U&t=4s), then edited these UFOs directly in Glyphs so I could clean up the skewed outlines as quickly and fluidly as possibly. With a huge batch of outline edits to be done, Glyphs was definitely more efficient due to its lag-free drawing. But, I ultimately kept the family as a UFO-based project, as I had already figured out all my technical stuff there.

### When you need to use one or the other

Certain things can only be done in Glyphs, and certain things can only be done in UFOs.
- Glyphs have various “smart” features like corner components that require Glyphs to interpret and build into output OTF/TTF fonts. My take is that these tools can be useful in an early design phase but shouldn’t relied on in a final font source because they are fragile between software versions and don’t allow full control over the actual shapes. However, different designers have different opinions on this.
- There are some aspects of creating variable fonts / large families that work better in UFOs + Designspaces, where you have more precise control because you are closer to the final products. (Literally: when you build from Glyphs sources using FontMake, it first outputs to UFOs, then builds OTF/TTF fonts from there.) A specific feature that I don’t think works properly from Glyphs (neither via Glyphs build or FontMake build) is giving a glyph both Intermediate layers (e.g. to adjust shaping at an intermediate weight) and Alternate layers/glyphs (usually swapped to via an RVRN feature, or rules in a designspace). This [miiight be fixed](https://github.com/googlefonts/glyphsLib/issues/1050) in a branch of glyphsLib, though? I’m not quite sure at the moment. Other similarly technical ends can’t always be achieved entirely within Glyphs sources, as they are somewhat abstracted to make design more intuitive and fluid.

### How to go between the two apps

There are two basic ways to shift between apps:
1. Install glyphsLib, then use glyphs2ufo and/or ufo2glyphs on the command line.
2. Just open one or more UFOs (or an entire Designspace doc) in Glyphs, or export to UFOs from Glyphs. (It doesn’t seem like you can save from Glyphs to a Designspace, in the app – you’d have to do this with glyphsLib, or set up the Designspace separately.)

Glyphs files tend to have extra data, which can be good and bad when exporting to/from UFOs. It’s handy to use Git when doing this kind of back-and-forth so you can see what is changing. It is sometimes helpful to also run “UFO normalization” before and after the conversion so you can maintain a similar formatting of the UFO data. For this, you can run [ufonormalizer](https://github.com/unified-font-object/ufoNormalizer) or simply open and save UFOs with ufoLib2.

## Signing off

I have suddenly remembered why I don’t write blog posts very often: it takes a lot of time to write something that is even close to decent!

Hopefully, though, this information is helpful to folks out there trying to understand this surprisingly deep question. If I’ve just dropped too many technical things without full explanation, and you are left more confused that when you started... welcome to type design! (But also, feel free to [email me](https://www.arrowtype.com/contact) to ask for more info.) The ins and outs of “RoboFont vs Glyphs” is a question that touches on all aspects of type design and development, and as such, it’s something I continue to learn about all the time. 

No matter what you’re making and which tools you use, all the best in your creative endeavors!

## Update 1: layers

Soon after I published this, a friend reached out to mention how RoboFont and Glyphs handle layers differently. I can’t believe I forgot to mention this! A few notes on this:
- The Glyphs *Background* layer is a quick **Command+B** keystroke away, and I use it constantly. RoboFont allows you to shift between layers with **Option+Command+Up/Down**, but the layers have some limitations.
- Glyphs allows you to put a component into a background layer: so, for instance, if you are drawing an `ohorn` with a custom shape, you can place a live-updating `o` component in the background for a visual confirmation that your main shape is similar.
- Glyphs also makes [Intermediate layers](https://glyphsapp.com/learn/intermediate-layers) and [Alternate layers](https://glyphsapp.com/learn/switching-shapes) simpler to add and generally simpler to handle than RoboFont. (In UFOs, you can still use intermediate layers – within a UFO or in a separate UFO – and reference that layer from your Designspace.) This advantage in Glyphs somewhat ends if you try to use *both* Intermediate and Alternate layers, as I mentioned above. Hopefully, though, this limitation will be resolved in time.
- Glyphs *also* assigns layers per glyph, and when you add a layer, it is date and time-stamped by default. This can be an easy way to quickly create a version history of glyph drawings as you iterate on an idea. This per-glyph model would also be possible in the UFO format, but RoboFont instead handles layers in a global sense, across a whole UFO, making them less useful for version history. (But there are better ways to handle versions and alternate glyph ideas. For versioning, save duplicate, date-stamped font files as you go, and/or use Git. To explore which shape of a glyph to use, make duplicate glyphs and test them in spacing strings, proofs, and marketing graphics.)

## Update 2: composing accented glyphs & character sets

Working back in Glyphs later in the day from posting this, I was reminded of another aspect that differs quite a bit between these two applications: building precomposed glyphs. These are glyphs with accents that designers precompose in a font, such as `aring` (`å`) or `Eacute` (`É`), and so on.
In general, this is much easier and faster in Glyphs than RoboFont, because:
- Composing accents uses “anchors” to specify where accents will attach to base glyphs. Glyphs gives a menu option for “Set Anchors” that will add in the main anchors needed for a wide range of language support, placing them at roughly the correct position. In RoboFont, you need to manually place these in each UFO source or use a script or extension to do so.
- A bigger efficiency in Glyphs comes from automatically adjusting composed glyphs when you move anchors or accents in individual glyphs. In RoboFont, you have to recompose glyphs to apply such changes.

Possible drawbacks of the Glyphs approach are:
1. If the software does too much “magic” for you, it can be easy to become complacent and not notice if something has gone wrong. For example, you may create composed glyphs and get them to look how they should, but they will change if you adjust your anchor points in either the base or accents. It might disrupt your prior work if you don’t anticipate or notice this repositioning.
2. Glyphs has certain assumptions about names for combining accents and bases, and it will only compose glyphs intelligently if you give the bases & accents the exact names expected by Glyphs. For example, Glyphs will create the proper `Acircumflex.ss01` if your file has *both* `Acircumflex.ss01` and `circumflexcomb.case`, but if the former is called `Acircumflex.alt` and/or the latter is named `circumflexcmb.case` (without the “o” in “comb”), you will have to use a glyph recipe, like `Acircumflex.alt+circumflexcmb.case=Acircumflex.ss01`. (This probably seems like a weird gripe, but other standards specifically use the accent name `circumflexcmb`, without the “o”.)  In RoboFont, you pretty much always need to use similar recipes in its [Glyph Construction extension](https://doc.robofont.com/documentation/how-tos/building-accented-glyphs-with-glyph-construction/), which is less automatic, but allows a more tailored workflow, without the application being too opinionated about how you do things.

### Character sets

As a related subject to composing glyphs, the two applications differ in how they expect you to set up character sets. 
- In Glyphs, [building character sets](https://handbook.glyphsapp.com/glyph-set/) happens in a few ways. Glyphs gives you a welcome screen for new fonts, and this offers to set up character sets for different scripts, like Latin, Cyrillic, or Arabic. It also gives a sidebar with categories for Glyphs, like “Latin > Basic,” “Latin > Central European,” “Punctuation > Parentheses,” “Figures > Tabular Figures,” and many others. Right-clicking on these allows you to add to that category of glyphs with appropriate naming and Unicode encoding. Building a character set is pretty straightforward if you accept the decisions made by the Glyphs team. To extend that, you can also add glyphs by names and lists of names, but Glyphs expects you to get the names “right” in order to get correct Unicode encoding and proper glyph composition support (as mentioned above).
- In RoboFont, [defining character sets](https://doc.robofont.com/documentation/tutorials/defining-character-sets/#:~:text=In%20RoboFont%2C%20character%20sets%20can,separated%20list%20of%20glyph%20names.) isn’t too bad, but requires a bit of research and setup. RoboFont will set up glyphs with appropriate Unicodes, so long as you use the correct glyph names, according to the [GNUFL](https://github.com/LettError/glyphNameFormatter or [AGLFN](https://github.com/adobe-type-tools/agl-aglfn)). For this, I find it essential to use the [Glyph Browser extension](https://github.com/LettError/glyphBrowser). This extension is a bit like the Glyphs sidebar but is more powerful in some ways (you can search for glyphs by name or by typing them in) and less handy in some ways (I somewhat prefer the Glyphs categories to the more standard but more general character set categories that are presented in Glyph Browser).

## Signing off, again

Who am I writing this for, anyway? I’ve attempted to present this comparison for someone new to the field of type design. Still, I must admit that I’ve included so many technical details that it would probably be difficult for most newcomers to follow.

Even so, if you *have* found this at all informative or entertaining, I’m glad! Come check out my [YouTube](http://youtube.com/arrowtype) or [Mastodon](https://typo.social/@arrowtype) for more type nerdery, and please say hello while you’re there!
