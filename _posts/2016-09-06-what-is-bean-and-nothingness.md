---
layout: post
section-type: post
title: What is Bean and Nothingness?
tags: development
author: nic
---

Welcome to the *Bean and Nothingness* development blog! Future posts will cover smaller things that come up during the development of the game, both engineering- and game-design-related, but as we kick off the blog it seems good to spend some time talking about the idea behind the game as a whole and how it came to be.

### The Game

*Bean and Nothingness* is a real-time, 2-D, tile-based puzzle game. It looks kind of like this:

![]({{ site.baseurl }}/img/game-look.png)

The puzzles are built around the behavior of the nine types of monsters. The monsters are created by the player out of combinations of beans --- the exact beans required to make each monster depends on the puzzle you're playing --- and each one behaves in a unique but predictable way. (For example, the orange dinosaur up there in the corner will run at the main character whenever it sees her, and the sleeping yellow thing below it can explode when it's pushed.) The monsters interact with the player, the beans, and each other, and most puzzles involve understanding and exploiting these interactions to get to the end without being stampeded, eaten, zapped, drowned, frozen, or blown up.

### History and Goals

The project began a few years ago when most of us were in the math Ph.D. program at the University of Michigan. The original plan was to throw together something small over the course of a few months as a distraction from research and teaching, and maybe, if it was fun and we worked well together, we'd try to tackle something bigger after that. Pretty quickly, though, it was apparent that the game we were making wanted to be much bigger, and the project has evolved from there. Now, a few years and jobs later, the development process is very far along; we've written almost all the puzzles and landed on a basically final set of mechanics.

The central design decisions behind the game were based on the things we love about the puzzle games we've enjoyed the most. Specifically, it was important from very early on that *Bean and Nothingness* be:

- *Challenging*: A lot of puzzle games start out with a good difficulty curve that plateaus pretty quickly, and the final puzzles aren't as hard as the mechanics allow.

- *Deep*: The best puzzle games have mechanics that interact with each other well and that can be mined for interesting puzzles for a long time. For us, this means careful consideration of the way each monster will interact with every other (and with the all-important beans).

- *Deterministic*: The puzzle mechanics in *Bean and Nothingness* are very tactical: they depend a lot on the exact relationships between the positions of the objects involved. For this to work, it is important for the game to behave predictably --- for the player to know that giving the same inputs at the same times will always have the same effect.

[Stephen's Sausage Roll](http://www.stephenssausageroll.com/) and [Snakebird](http://snakebird.noumenongames.com/) are great examples of games that got these things right. *Bean and Nothingness* has one aspect that these games don't, though: all of the action takes place in real time. This decision, which was also made quite early, made achieving these goals quite a bit harder, especially the determinism. Most real-time puzzle games have looser mechanics than a step-based game like *Snakebird*, but in designing *Bean and Nothingness* it's been important to us to never sacrifice the sort of precision that allows for deep and complicated puzzles.

### What's Left To Do

*Bean and Nothingness* is still in very active development, and there's a lot we haven't done. We're continuously polishing the graphics, the sound, and the puzzles, and as of this post we're hard at work on the story. Keep following for more news!