---
title: What changed in Name Sans v0.4? Everything – and nothing much.
description: A look a how Name Sans has evolved from v0.1 to v0.4
date: 2020-12-15
tags:
  - name sans
layout: layouts/post.njk
---



The update between Name Sans Versions 0.3 & 0.4 was a leap, not a step. Ultimately, all decisions were made in pursuit of the core goal of this family: to bring the beauty and charm of the NYC Subway mosaic name tablets into a useful, extensive, modern type system.

Of course, in type, even relatively big changes – which make a major difference in the visual impact & reading experience for viewers – are ultimately details. Because they are details, they can be hard for the outside observer to track. I wanted to take a moment to document what changed, and why. 

## Initial development and evolution since

A lot of the best type families are the product of many years of development, experimentation, testing, and revision. Certainly, this is how I see Name Sans. It started as sketches in my notebooks as a daily commuter in NYC. And, as I get further into making it a full type family, I keep seeing it more clearly. I am essentially discovering what the family ought to be, and doing this process mostly in the open.

Initially, I thought that the idea for a family based on the NYC Subway mosaics would be my thesis project at KABK TypeMedia. 

After being accepted into the program, I told one mentor that I planned to make a typeface based on the mosaics, and they remarked with some incredulity. To paraphrase, they asked, “Is that even possible? There’s not a cohesive set of styles in the system! It’s a bunch of different works.”

Ultimately, I ended up pursuing a different thesis project (Recursive [ ADD LINK ] ) at TypeMedia, and I am very glad I waited to seriously start working on Name Sans. 

For one, it would have felt a little silly to work on typeface about NYC from another continent. It’s not that it’s impossible – obviously, the internet & photography exist, and anyone could make a typeface like this, working from any location. Still, for me, part of making Name Sans has been making some of it, then riding the Subway and contemplating the mosaics as I see them, with the project in mind. And, I’ve carried these nebulous experiences with me as I work on and evaluate the typeface.

After TypeMedia, as I was really diving into drawing this family as a variable font, I was still very much approaching it with the same mentality I used for Recursive: wanting to push the limits of font technology and try to make something new and never possible before. At that point, some of the main questions in my head were related to the fact that there are no clear typefaces or blueprints used to create templates of these letters[1].

[1] At least, I so far haven’t been able to find blueprints, though it’s possible that they *are* lurking in the MTA archives somewhere, and just hard to discover as regular New Yorker and then as a type designer in a pandemic).

1. What are specific, distinctive shapes & features that are important to preserve from the name tablets?
2. Should this have counter connections that are smooth (like Helvetica) or sharp (like Franklin Gothic)?
3. How can I make an Optical Size axis that went beyond just presenting the same general appearance across sizes, but really pushed people’s ideas of what a Text & Display family could be?

My answer to these questions was, basically:

1. Distinctive visual motifs: intense geometry, low contrast in strokes, a level of “stiffness” portrayed with straightened shallow curves, and optical corrections which are either emphasized or reduced (like the way an S gets smaller at the top in some signs, while the B doesn’t – whereas both tend to be more subtly balanced in most typefaces).
2. Smooth or sharp connections: Why not both? With a clever Bézier construction, I could make a single variable font that had sharp connections at small Optical Sizes and smooth connections are larger sizes, then tight curves for connections at middle sizes.
3. Pushing people’s ideas: Aside from the smooth/sharp connections, I also used a few techniques. In smaller sizes,  I really emphasized the contrast of strokes and enlarged “inktraps,” while at larger sizes, I pushed the roundness of shapes, the tightness in spacing, and narrowness of apertures (the openings in letters like a, c, e, & s). And across the board, I worked to make an extreme weight range which could go from as thin to as thick possible. 

In the time since releasing each version of Name Sans (starting with Version 0.1 on January 7, 2020, which now feels like decades ago), I have used the typeface as much as possible, especially digitally. I often override web pages with the latest version to see how it fits in web layouts, and how it feels to see, read, and write with. I have also carefully observed how others have used it in real projects – what expectations of mine do they break, and what styles do they gravitate towards?

This led me to a few observations:

1. One of my favorite aspects grew over time: it felt familiar, but was also a little “sharper” than the (countless) others in the same overall genre. It had a sense of angularity and slight idiosyncrasy that gave me something of the same feeling as the texture of mosaic tile.
2. Several designers ended up using the Display styles at text sizes, not seeing the Text styles as better despite me making them deliberately different. Sure, some of this might be expectations carrying over from a world where optical sizing is uncommon in sans-serifs, but also, I felt that some of this might be indicating a desire for more visual similarity between sizes, rather than less. Worse, there were some Optical Size values at which I didn’t really *like* the results. Around 18–24, the joins weren’t quite sharp and weren’t quite smooth, and I couldn’t really get past my distaste for this.
3. Some of the ideas I had for what might help the crispness & readability of text at small sizes ended up failing in practice. The large notches and higher contrast stroke joins ended up (to my eyes) creating undesired spots of disruption: broken strokes or faded notches that needed more presence.

## Being truer to the source material

On top of these observations, I came to a simpler problem that made me re-evaluate my design. 

I started to try matching some of my favorite signs with the way the family had turned out, in order to make graphics about where different design features had come from. 

In this process, I couldn’t shake the feeling that I had let in a few too many of my own ideas about what makes type modern, and by extension had let go of a few too many ideas that makes the mosaics what they are. 

In particular, the apertures of the Display were narrow without a clear precedent, and the sharp-to-smooth joins were an idea that was too focused on tech and not focused enough on providing a clear, singular design.

- A few of my favorite signs

- Signs versus v0.3

I knew this was all a problem. But I had other issues: I had already delivered these styles to users, and it felt like I was pretty far along in the completion of the family. Should I really “abandon” my progress and go down a different route? Was that sensible, from a business perspective?

It got me to the point I was thinking, “I guess I could finish this, then make a Name Sans II, someday.” Designers and artists sometimes say that, after a certain point, their ideas take a back seat to “what the work itself wants.” In this case, I had a choice of two paths: giving the design what it “wanted” and finishing the thing, or reasserting my own ideas of what this needed to be, even if it would take more time.

Wrestling with this choice, I realized: life is short, and I may not *get* to make a totally-different sequel of this family. Less dramatically, Future Fonts is meant for fonts in progress, and users buy in early *knowing and expecting* that fonts aren’t final yet. I decided to not be overly beholden to my past beta releases, but rather to pursue the best possible solution for this design.

And so, I began to experiment.


- Signs versus v0.4


## Making a more-cohesive system

- Explanation of family structure

## What do the Optical Sizes do?

- In the days of hand-cut metal type, fonts inherently had size-specific designs. 
- Obvious changes: thin parts of serif designs were made proportionally thicker
- Less obvious changes: at small sizes letter spacing was increased to keep letters from appearing overly-squished. At large sizes, spacing was tightened to keep words bonded together.

- How much spacing does type need? This is the basis of some good blog posts already. [LINK] The short answer: enough to look good. At smaller sizes, a common theory is that inter-letter spacing should roughly match the amount of space inside letters. At larger sizes, this approach makes for very airy spacing. The visual continuity and impact of large type can be improved by tighter spacing. Of course, as with all things in type, this is influenced by culture: what people are used to reading (Helvetica, Roboto, Apple SF) influences this. So, a necessary approach is to balance considerations.

Digital fonts were so often designed with just a single, “scalable” set of outlines, graphic designers have learned tricks to make it (mostly) work: give a bit of extra spacing to small text, remove a bit of spacing from large text. Correct kerning manually where needed.

This approach is useful to learn, but full of problems. First, most users of type aren’t specialists who have a good sense of how much to track type for a given size. Complicating things further, every typeface is different, and requires different tracking.   What’s more, substantially different proportions of kerning can look right or wrong at different sizes [say more here?]. So, even for experts, tracking decisions are time-consuming and imperfect at best.

In many families, the middle weights are designed for smaller use, while the extremes of light and heavy are intended for larger sizing. But what if you want middle weights at larger sizes? Or extreme weights at smaller sizes?

Name Sans employs several strategies to keep sizing simple and useful.

- Larger sizes (96pt and up): tight spacing, geometry prioritized
- Smaller sizes (12pt and down): looser spacing, slightly condensed proportions to save space and preserve feeling of geometry in long-form reading (where round letters begin to feel elliptical)
- Medium Sizes balance these approaches. Because Name Sans is a variable font, it provides a fluid (but curved) transition, improving the aesthetics and readability across many sizes.


## Weights

The weight range is as wide as possible, but adjusted for optical sizes.

## Making it all useful

- The ranges of design options in a variable font can either be equally good throughout, or have areas that aren’t as intentional.
- Sometimes, axes that are gradual but not as elegant in the middle are still useful. In my project Recursive, the *Casual* axis looks better on either side, and the middle is intended mostly to allow transitions on digital interaction – such as when a user hovers over a link.
- Often, though, it’s better to give users products that have as few downsides as possible. In terms of a variable font, that means providing axes which yield elegant results through their full spectrum.

### Bézier tricks vs simple optical sizing

Up to v0.3, I took the approach that Display sizes could be geometric and have smooth joins, while Text sizes could be Humanist and have sharp joins. This worked pretty well across medium sizes, too! It was a Bézier interpolation trick I was excited and proud to have found. Maybe, I thought, people would be more likely to use a range of sizes if they were clearly different.

But, it had problems.

- There were medium/smallish sizes where I *didn’t* like the result.
- The Text sizes had visual issues that bugged me, in practice. I test fonts in my browser a lot [link to TYPEx]. In small text, my eyes kept seeing that letters had weak spots in joints – for instance, the top left of `n` was a bit light or faded.
- I ended up seeing designers using the Display sizes for small text, anyway. This indicated to me that the liked the style available in the display, and actually wanted more continuity across the family.

### Meanwhile, the Display was a little too much of a departure

## Less words, more diagrams

So, what’s different? Let’s take a look.