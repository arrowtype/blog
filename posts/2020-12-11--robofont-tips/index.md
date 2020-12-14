---
title: Getting the most out of RoboFont
description: Extensions & Tips for RoboFont
date: 2020-12-11
tags:
  - robofont
  - tools
layout: layouts/post.njk
---

Type designers are lucky to have a variety of extremely-capable tools for creating new fonts. 

The font editor I use most is RoboFont, for reasons mentioned in my earlier post, [Getting Started in Type](../2020-05-01--getting-started-in-type). This post actually started as a section of that article, but I have since realized that I would like to add more extensions and more details. If you haven’t already read that article, there are lots of helpful tips there, so consider giving it a look, too!

## Extensions I couldn’t live without

Most RoboFont extensions can be found at https://robofontmechanic.com/. I have added specific links where tools are better or only available in specific repos.

Some of the free extensions I couldn’t work without:
- Mechanic, to handle extensions (pretty essential)
- Add Overlap, to add corner overlaps to selected points. I like [Okay Type’s fork of this](https://github.com/okay-type/AddOverlap), which adds a little UI at the bottom-right corner of Glyph Windows which allows positive, negative, or zero overlap to corner points.
- Add Segment Guideline, a very simple but useful way to add a guideline to a selected segment
- Batch, to help you build fonts from RoboFont
- [CornerTools](https://github.com/roboDocs/CornerTools) – really nice tools to modify corners (read the readme on there for instructions)
- Glyph Browser, to make it easy to add specific glyphs with correct unicodes & naming
- DesignSpace Edit, to help set up designspace documents that you can build with FontMake
- EditThatNextMaster, to help working with multiple related fonts
- Eyeliner, to make it easy to set when a point is on a guide or metric line
- GlyphMirror, an extension to draw mirrored versions of your drawing in a background visual, which makes it fast and easy to achieve symmetry. (This one is not yet available on Mechanic; get it from [its GitHub repo](https://github.com/RafalBuchner/glyphMirror)
- Properties, to display distances in selected points, etc
- Overlay UFOs, to display glyphs from the same or other open UFOs while you draw
- Outliner, if you want to draw a single line, then expand it, e.g. as a quick way to start a Comic Sans-style font.
- Ramsay St, to show related glyphs in the glyph view (though, I use the Space Center quite a bit more for this)
- ScalingEditTool, a super-necessary tool to move points in a way that is less disruptive to attached curves
- [ScaleFast](https://github.com/roboDocs/ScaleFast), extremely awesome for scaling glyphs to speed up the process of making things like superiors & inferiors, small caps, legal symbols, and more
- Shape Tool, to draw circles & rectangles
- SpeedPunk, as one way to consider the smoothness of curves
- Theme Editor, to make it easy to control your drawing theme
- word-o-mat, to create strings to judge type in the Space Center

**Paid extensions**

- MetricsMachine is extremely worthwhile, to help with kerning. If you get this, MM2SpaceCenter is a nice (free) add-on extension to give more context in the Space Center as you work on kerning.
- Prepolator is very worthwhile if you are working on fonts which you plan to interpolate. A new version of this is currently in the works, and it automates the process *a lot* more. It is amazingly helpful for an otherwise annoying task.
- Skateboard is extremely helpful for planning & designing variable fonts.

You can get more-detailed documentation about RoboFont extensions at https://robofont.com/documentation/extensions/.

## Additional macOS tools I couldn’t live without

[Paste](https://pasteapp.io/) gives you access to your Clipboard History, which is helpful in *many* situations (email, code, interface design, etc etc), but also handy in RoboFont. You can copy a couple of contours, then (if you remember the order you copied things in) paste them as needed. Hard to explain, but very handy.

[Divvy](https://mizage.com/divvy/) allows you to easily set the sizing of windows without dragging things around manually. This is helpful in lots of scenarios beyond type design, but especially nice in a multi-window app like RoboFont. Set up some global shortcuts to make this even quicker! There are other "window manager" apps for Mac, but this one offers my preferred balance of simplicity and power.

## Dark Mode in RoboFont

Sometimes, it’s nice to work in the evening without blasting your eyes with a ton of bright light. Luckily, RoboFont settings allow you to get a pretty serviceable dark mode in two steps:

1. You can use [this script](https://gist.github.com/arrowtype/268bb9db71231ca4fc39143760e94947) as a "Start Up Script" (see script for instructions) to automatically set a light/dark mode each time you start RoboFont, based on your macOS preferences. If you change the macOS preference and want to update light/dark mode, you can also run the script without restarting RoboFont.
2. If you also want a dark mode for the Glyph View (if you want dark mode, you will want this too), you can also install the Theme Editor extension, then use my ["Dark Connor" theme](https://gist.github.com/arrowtype/f450d2c7cfbcea61ab7ad6c43af14932) or make your own.

## Drawing Tips

Most of the time, it is helpful to work with the Glyph View and the Space Center side-by-side. Use Divvy (mentioned above) to set up 50% of your screen with a glyph, and the other 50% with the Space Center, then adjust the glyph while keeping an eye on the glyph in the context of spacing strings, at different scales, and/or more! I didn’t do this for a long time, but then I picked up the tip from James Edmonson (OHno Type Co) on Instagram, and it changed my life.

Get familiar with using the Transform (T) tool, along with the modifier keys. This can be very unintuitive at fist, but becomes pretty powerful over time. I will try to make a video or say more about this at some point, because it can be easy to miss but seriously helpful.

## Ask for help!

If you get stuck on a problem, chances are, someone will be happy to help you out. Sometimes, just the act of clearly writing out your problem will help you solve it on your own! This applies to basically all aspects of computers and software, but is particularly true in learning & using RoboFont and its associated tools.

Generally, if you run into an unexpected issue, open the Output Window (Python > Output Window, or Option+Command+o) and check for error messages.

- Google it (if you have an error message, try pasting in the relevant part – usually the last line or two)
- The RoboFont Forum
- GitHub Issues (try to find the relevant repo for a particular tool)
- Twitter (you can mention me, @ArrowType, and I will either try to chip in or mention someone who might know more)
- Type Crit Crew (helpful for a lot beyond troubleshooting, too!)

## Happy RoboFonting!

There is *a lot* more that could be said about RoboFont, but hopefully this post is able to help you learn a few useful things you didn’t already know. Enjoy!
