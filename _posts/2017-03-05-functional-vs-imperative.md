---
title: Is imperative programming imperative for game dev? 
---

In software development, early optimization is usually a sin.

But a smooth gamepaly is simply a requirement for some types of
games (like a racing demo), so I had to check if an acceptable
framerate was even possible to start with.

So, today I used a good part of my Sunday trying to improve the FPS of
my little demo.

And after some experimentation reality kicked in:
the clean and nice functional approach that I was thriving for in the code
wasnt really a match for the shared-modifiable-state-lets-just-use-another-global-here
imperative style alternative. :(

It is already bad enough that I am using garbage-collected Javascript to
build a game, and that the framework I picked to use (pixi.js) is all 
object oriented and heavily based on side effects :P

I ended up refactoring the code to something I am not proud of in order
to get a less-laggy demo, imperative won this battle today, but I havent 
gave up yet, and more refactoring is comming tomorrow. I need to
find a good balance/compromise, this is 2017 after all, we were
supose to have spare memory and cpu cycles to afford our pure functions
and immutability by now. I want to insist on the ideal!

Anyways, here is the [daily build](https://github.com/20kbudget/road/releases/tag/v0.5.0).
