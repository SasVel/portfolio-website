+++
title = "This is Koz!"
date = "2026-10-30T08:53:38+02:00"
dateFormat = "02-01-2006" 
cover = "img/koz/koz_cover.png"
layout = "game_page"
embedLink = ".Site.Params.GameLink.Koz"
tags = ["game-dev", "koz"]
keywords = ["", ""]
description = "This is an example post."
showFullContent = false
readingTime = true
hideComments = false
+++

# The weird, yet charming idea.

Koz started as an ambitious university project for a pygame course.
It was my first experience building a game outside of an engine and it was a wild one.
I wanted to make something like a visual representation of what is going on in my head when playing Scoundrel and go off from there.

## What is [Scoundrel](http://www.stfj.net/art/2011/Scoundrel.pdf)?
Scoundrel is a *single player roguelike card game* by Zach Gage and Kurt Bieg. 
You can have an awesome roguelike experience by yourself with a deck of cards and a counter.
![Ripple Shuffle & Roll's cover for his tutorial on Scoundrel](/img/koz/rs_scoundrel_cover.jpg)
*[Ripple Shuffle & Roll's tutorial](https://youtu.be/7fP-QLtWQZs?si=6TzTVj6jkvMDWEln)*

I was absolutely fascinated how addicting a stupid game like Scoundrel can be. So Koz is my own little spiritual successor of that gem of a game.

It's inspired from other digital roguelike card games like Slay the Spire and Inscription. I wanted the artstyle to be symbolic of the feeling of randomness playing Scoundrel - bashed together with not much thought, but working so well nontheless.

![Koz assets irl](/img/koz/koz_assets_physical.jpg)

I also had an urge to challenge myself to draw everything physically, since Scoundrel is very much a real life card game.

## Python is easy...right?
...yeah...


I was so green back then, so full of wonder and delusion. Thinking it would be a fun little
side course I delve right into pygame development. Then I realised all I have is a library for rendering images on the screen. Nothing else.
But...how hard could it be to develop some systems I already know in python...I mean it's *python, come on*.

**It was very hard. It ate a solid chunk of my semester.**

I had to develop from scratch:
 - UI management system with anchoring
 - tweening
 - observer pattern
 - Entity Component System for the cards themselves
 - Color palette controlled by a JSON.

This was while battling the hidden pitfalls of python, such as a dependency hell that was only resolved by initialising every part of the game on startup.
Ruining the whole point of having dependancies, all game objects reserve memory immediately after initialisation.
But at least it worked, and that is a sacrifice I was willing to make. The game is small enough to not be a RAM hog, even with my shitty solution.

*Also finding PygameCE was a game changer, it has a ton of little improvements, as well as having slightly better documentation.*

It was a fun project that made me a better developer, no doubt about that. The ECS system from scratch made me sweat. Coding without an engine felt like making a whole new world out of nothing, it was incredibly freeing, yet very scary. You can't really blame anybody or any feature, when all features are made by you. **All decisions fall on your shoulders alone.**

The game worked at the end and I was a happy bugger. But I was not satisfied, I didn't manage to make shaders work, good particle effects would also take forever. So I made my first game rewrite - from Pygame to Godot!

This is [the original repo](https://github.com/SasVel/Koz-Pygame.git) for the project if you want to enjoy some badly written code.



