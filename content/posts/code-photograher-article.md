+++
title = "Code Like a Photographer"
date = "2026-06-27T18:59:25+02:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
authorTwitter = "" #do not include @
cover = "img/covers/CodePhotographerCover.jpg"
tags = ["article", "thoughts"]
keywords = ["", ""]
description = "The value of a re-write."
showFullContent = false
readingTime = true
+++

*Photo by me.*

I’m a sort of experienced programmer by now, with a couple years under my belt working on various projects, both professional and personal. Wouldn’t say I’m great, but I’ve been around the block.

In my development journey I never really found the time or motivation to re-write **a whole project** from scratch, since I never really **found a reason**. It’s already done after all, I’ve built the thing, **so logically I should know it by heart**. Re-doing the whole process would just be a waste of time. **Does sound legit, doesn’t it?**

## **The Backstory**

I made a game in [Pygame](https://pyga.me/docs/index.html) couple of months ago, it’s a dungeon crawler card game called [Koz](https://github.com/SasVel/Koz-Pygame). It was a wild ride to implement an Entity Component System all from scratch, but overall it was worth it. I quite enjoyed what I’ve built and wanted to expand on it beyond my starting goal, but Pygame is just a library, not a game engine and a lot of the utilities of a modern game making utility are missing. Lackluster shader support, no UI utilities, etc.

> Read more about [Koz](/posts/koz-intro).

So I decided to re-write the whole game in Godot. Noble idea, I know, **but hear me out.**

## **Limitations as a driving factor**

Our limitations often mold our creative projects. It’s **not the freedom we have, but the lack of such** , that actually pushes a project of any kind to fruition. 

Photography encompasses that idea perfectly. Due to limitations in gear, time of day, environment or time available, the photographer is forced into finding creative solutions that result in individuality and beauty in the final photo. 

So how does that translate at all to my Pygame game? If we think of creating software in the same way as photography, said limitations are found in the form of:

  * Hardware
  * Software tools we use
  * Our own understanding
    * of the tools/design patterns necessary
    * of business logic itself

Hardware limitations are pretty much non-existent for most projects, that is if you think about what you’re doing **(or actually read what Gemini/Claude spits out).** Limitations in software are way more common. That is the **photography gear in our analogy** , it’s actually good to have said limitations! There are even languages built on that very concept (like [Rust](https://rust-lang.org/) or [Go](https://go.dev/)).

Often building software is not just using the tools provided, but building upon them in order to use them, more akin to **building a camera with the parts of another camera to take the picture.**

## **Change of focus**

So the issue with expanding software understanding is that it’s far from one-dimensional. But our focus as developers often is **exactly** one-dimensional. Changing focus all the time makes all parts of your work a bit worse. Re-writing the game in Godot let me free up the space in my mind previously preoccupied with business logic, and solely focus on implementing the design patterns of the application in the best way possible. Adapting the design pattern's logic in the new environment gave me a lot of insight about how to spot and adapt them for my specific use case and I can confidently say using the same patterns would be times easier than before.

So that is the gist of it! Solely focusing on building the foundations **freed up mind real estate** to improve the final product and to improve myself. Re-writing projects (**within reason, I’m not advocating to redo your OS in Rust**) is definitely a tool worth considering! 

The repository for [Godot Koz.](https://github.com/SasVel/koz-godot) 

> {{< game_embed name="Koz" link="https://itch.io/embed-upload/18108046?color=9e2835" rateLink="https://sasvel.itch.io/koz/rate">}}
