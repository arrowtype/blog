---
title: Getting the most out of RoboFont
description: Extensions & Tips for RoboFont
date: 2020-12-11
updated: 2021-04-17
tags:
  - robofont
  - tools
layout: layouts/post.njk
permalink: robofont-tips/index.html
---

Type designers are lucky to have a variety of extremely-capable tools for creating new fonts. My favorite of these is the font editor RoboFont, along with its ecosystem.

I covered some of the reasons I like RoboFont in my earlier post, [Getting Started in Type](../getting-started). This post actually started as a section of that article, but I have since realized that I would like to add more extensions and more details. If you haven’t already read that article, there are lots of helpful tips there, so consider giving it a look, too!

## First things first

Like most powerful software, RoboFont has a lot of functionality, and you will save time by doing a bit of reading before diving in. It is extremely useful to get familiar with the [RoboFont Docs](https://robofont.com/documentation/) (even if you just skim parts of it at first). If you are new to RoboFont or just wondering what it’s all about, start with the [RoboFont Introduction](https://robofont.com/documentation/introduction/).

As a new user, you will probably want to define the default character set for new fonts. [Here’s how](https://robofont.com/documentation/how-tos/defining-character-sets/). Glyph Browser, an extension mentioned below, further extends this part of the process.

## My favorite RoboFont extensions

Extensions are a big part of the RoboFont experience. Most RoboFont extensions can be found on [Mechanic](https://robofontmechanic.com/).

You can get more-detailed documentation about RoboFont extensions at [robofont.com/documentation/extensions/](https://robofont.com/documentation/extensions/).

However, it can be overwhelming to know which extensions are available, and which ones you actually want to use. After working for about three years almost daily in RoboFont, here are the RoboFont extensions that I find most useful.

### [Mechanic](https://robofontmechanic.com/), by Frederik Berlaen and Antonio Cavedoni

Mechanic is an easy way to manage (most) RoboFont extensions. It’s pretty essential, as it allows you to easily find and install most of the other extensions listed here. Extensions mentioned below but not available via Mechanic are linked to, but the ones not linked to are simplest to find & install via Mechanic.

### Add Overlap, by Alexandre Saumier Demers

Adds corner overlaps to selected points. I like [Okay Type’s fork of this](https://github.com/okay-type/AddOverlap), which adds a little UI at the bottom-right corner of Glyph Windows which allows positive, negative, or zero overlap to corner points.

### Add Segment Guideline, by Jan Šindler

This is a very simple but useful way to add a guideline to a selected segment. I’ve set it to the shortcut **Command /**, and I use it constantly – especially when drawing glyphs with diagonal strokes.

### Batch, by Frederik Berlaen

This is a simple UI to help you build fonts from RoboFont. I do almost all of my font builds with [FontMake](https://github.com/googlefonts/fontmake), but this is a whole extra skill to learn, and probably not necessary for every font project.

### [CornerTools](https://github.com/roboDocs/CornerTools), by Loïc Sander

Want to add a bunch of rounded corners or inktraps to a font? This is a fast way to do it! This is a super nice tool to modify corners. Read the project readme for instructions.

### DesignSpace Edit, by Erik van Blokland

This will help set up and edit correctly-formatted DesignSpace documents that you can build with Batch or FontMake, for font projects involving interpolation to create static instances and/or variable fonts. I often start here to make a new DesignSpace, then use a code editor to make edits more efficiently.

### EditThatNextMaster, by Erik van Blokland

A common early complaint about RoboFont is that it’s a bit tricky to move between sources for a multiple-master font project. This solves that by assigning a hotkey to move between views of open UFOs.

### Eyeliner, by Ryan Bugden

Simple but essential: this makes it easy to see when a point is on a guide or metric line.

### Glyph Browser, by Erik van Blokland

This is an essential tool to make it easy to add specific glyphs with correct unicodes & naming. It allows you to either search by typing a glyph name (e.g. `paragraph` or by character (e.g. `¶`).

### [GlyphMirror](https://github.com/RafalBuchner/glyphMirror), by Rafał Buchner

This draws mirrored versions of your drawing in a background visual, and these can be flipped in different ways and moved around. This makes it fast and easy to achieve and check symmetry, when you want it.

### Properties, by Jérémie Hornus

This displays distances between selected points, lengths of selected segments, and more.

### Overlay UFOs, by David Jonathan Ross

This displays glyphs from the same or other open UFOs while you draw. Helpful to draw and check related shapes within a single font (e.g. `n` and `h`), to check related shapes between different sources of a big project, and to have a guide for shaping in less-familiar characters.

### Outliner, by Frederik Berlaen

THis is helpful if you want to draw a single line, then expand it, e.g. as a quick way to start a Comic Sans-style font.

### [Popup Tools](https://github.com/typesupply/popuptools), by Tal Leming

This is a little pop-up panel that allows the alignment & distribution of selected nodes & contours. It’s something I’ve wanted maaaany times, especially as someone who has spent a lot of time in design tools like Figma, Sketch, & Illustrator, where I used these functions constantly. But, I got so used to drawing without it, I am not yet sure whether it will be something I use a lot. 

### Ramsay St, by Frederik Berlaen

This will show related glyphs in the glyph view, on either side of the glyph you’re currently drawing. I used it a lot at first, but I hardly ever use it now – I’ve moved to using the Space Center quite a bit more for this purpose.

### ScalingEditTool, by Timo Klaavo

This is a super-necessary tool to move points in a way that is less disruptive to attached curves. You kind of have to try it to understand it, but when I draw, I constantly go between the default Edit Tool and the Scaling Edit Tool. (In fact, the ease of shifting between tools with number keys is one reason I enjoy drawing in RoboFont! It’s weird at first, but much more ergonomic once you get used to it.)

### [ScaleFast](https://github.com/roboDocs/ScaleFast), by Loïc Sander

This one is extremely awesome for scaling glyphs to speed up the process of making things like superiors & inferiors, small caps, legal symbols, and more.

### Shape Tool, by Frederik Berlaen

It’s sort of hilarious that this isn’t built into RoboFont, but it also says something about the thinking behind RoboFont as a tool. This extension lets you draw circles/ellipses & squares/rectangles. It’s not built into RoboFont because you might want to tweak the circle-drawing algorhythm yourself, e.g. to draw the slightly-boxy “circles” necessary to make a geometric font that actually *looks* circular (I haven’t done this, but I probably should try it sometime).

### [Space Station](https://github.com/typesupply/spacestation), by Tal Leming

I only just discovered this one, but it’s a godsend. It enables you to allow a systematic approach to spacing. A really useful aspect of it is that it allows you to import/export simple configuration files, which have a simple syntax which makes it easy to say which glyphs should match the sidebearings and/or widths of which other glyphs. Instead of approaching the problem in a way that is too automated, it encourages you to think systematically about spacing, and is easy to use either purely as a reference/quality-control tool, or as a way to quickly cascade spacing adjustments through a whole font.

### Speed Punk, by Yanone

This is one way to consider the smoothness of curves.

### Theme Manager, by Connor Davenport and Andy Clymer

This makes it easy to control your drawing theme. I use it to switch between light & dark drawing modes (more info below), to keep my eyes happy at night.

### word-o-mat, by Nina Stössinger

This allows you to create strings with desired characters in the Space Center, in order to judge your glyphs in context. Really, really handy.

## Paid extensions

A few very good extensions are complex software in their own right, and these must be purhcased separately. This allows the developers to provide support and to maintain these products, and because these are pretty critical pieces of my workflow, I find that to be a very good deal.

### MetricsMachine

Extremely worthwhile, to help with kerning. If you get this, MM2SpaceCenter is a nice (free) add-on extension to give more context in the Space Center as you work on kerning.

### Prepolator 

Very worthwhile if you are working on fonts which you plan to interpolate. A new version of this is currently in the works, and it automates the process *a lot* more. It is amazingly helpful for an otherwise annoying task.

### Skateboard 

Extremely helpful for planning & designing variable fonts.

## Additional macOS apps that are especially useful with RoboFont

[VS Code](https://code.visualstudio.com/) is an excellent code editor, file explorer, Git client, and terminal, all built into one elegant package. I nearly always have a project open in a VS Code workspace while I’m working in RoboFont. This is entirely optional, but if you’re doing a mix of scripting, font building, and Git versioning, it is so handy to one place to many all these technical bits.

[Paste](https://pasteapp.io/) gives you access to your Clipboard History, which is helpful in *many* situations (email, code, interface design, etc etc), but also handy in RoboFont. You can copy a couple of contours, then (if you remember the order you copied things in) paste them as needed. Hard to explain, but very handy.

[Divvy](https://mizage.com/divvy/) allows you to easily set the sizing of windows without dragging things around manually. This is helpful in lots of scenarios beyond type design, but especially nice in a multi-window app like RoboFont. Set up some global shortcuts to make this even quicker! There are other "window manager" apps for Mac, but this one offers my preferred balance of simplicity and power.

## Dark Mode in RoboFont

Sometimes, it’s nice to work in the evening without blasting your eyes with a ton of bright light. Luckily, RoboFont settings allow you to get a pretty serviceable dark mode in two steps:

1. You can use [this script](https://gist.github.com/arrowtype/268bb9db71231ca4fc39143760e94947) as a “Start Up Script” (see script for instructions) to automatically set a light/dark mode each time you start RoboFont, based on your macOS preferences. If you change the macOS preference and want to update light/dark mode, you can also run the script without restarting RoboFont.
2. If you also want a dark mode for the Glyph View (if you want dark mode, you will want this too), you can also install the Theme Editor extension, then use my [“Dark Connor” theme](https://gist.github.com/arrowtype/f450d2c7cfbcea61ab7ad6c43af14932) or make your own.

## Three drawing tips

So much can be (and is) written about drawing type, but here are two things that aren’t as obvious:

1. Most of the time, it is helpful to work with the Glyph View and the Space Center side-by-side. Use Divvy (mentioned above) to set up 50% of your screen with a glyph, and the other 50% with the Space Center, then adjust the glyph while keeping an eye on the glyph in the context of spacing strings, at different scales, and/or more! I didn’t do this for a long time, but then I picked up the tip from James Edmonson (OHno Type Co) on Instagram, and it changed my life.
2. Get familiar with using the Transform (T) tool, along with the modifier keys. This can be very unintuitive at fist, but becomes pretty powerful over time. I will try to make a video or say more about this at some point, because it can be easy to miss but seriously helpful.
3. A really handy feature of RoboFont (especially for early-stage drawing & exploration) is the [Test Install](https://robofont.com/documentation/how-tos/using-test-install/), which allows you to quickly install the font you are working on, then immediately use it in other apps to test it out, make proofs, etc. Sometimes, this won’t work if you have special feature syntax in the “Features” tab. I often use minimal to no features here, then add them in a separate build process. But, this varies a lot from project to project.

## Ask for help!

If you get stuck on a problem, chances are, someone will be happy to help you out. Sometimes, just the act of clearly writing out your problem will help you solve it on your own! This applies to basically all aspects of computers and software, but is particularly true in learning & using RoboFont and its associated tools.

Generally, if you run into an unexpected issue, open the Output Window (Python > Output Window, or Option+Command+o) and check for error messages.

- [The RoboFont Forum](http://forum.robofont.com/) has lots of existing questions & answers, and new questions are welcomed, and generally answered pretty quickly!
- Google your errors (if you have an error message, try pasting in the relevant part – usually the last line or two)
- Use GitHub Issues (this can be a little more advanced; try to find the relevant repo for a particular tool, if you have an issue with it)
- Twitter has it’s problems, but you can also learn a lot from the people there. You can mention me, [@ArrowType](https://twitter.com/ArrowType), and I will either try to chip in or mention someone who might know more.
- [Type Crit Crew](https://medium.com/typecritcrew/type-crit-crew-fdd180b881c) is a collective of type designers (myself included) who have made free office hours bookable by folks who are seeking type critique or advice. Getting critique and talking with experts can be a bit daunting, but folks here are super kind, and you can learn so much in this way!

## Happy RoboFonting!

There is *a lot* more that could be said about RoboFont, but hopefully this post is able to help you learn a few useful things you didn’t already know. Enjoy!
