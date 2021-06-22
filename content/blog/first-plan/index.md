---
title: "wait what am i doing?"
date: "2021-05-04"
---

So! after taking brief exploration periods in each of my ideas from my brainstorm, here are some of my thoughts.

## quantum cryptography

Now, I really enjoyed going a lil deeper in quantum cryptography, but I don't think it's the right fit for this project. The primary issue is the amount of context you would need to even find it interesting. It's nice if you could lecture about it, but not so nice if all you get is a passing exposure. You need context about quantum physics (what is a photon? what does it mean for something to be polarized?) and cryptography (what's key exchange?) and algorithms (QKD ain't simple).

If it was just a problem of too much background, I think I'd be able to handle it. I could simplify, leave out technical details and stay on an intuitive level. The issue there is the lack of connect to the physical world (both in the touch-grass sense and in the physics sense). If I gloss over the quantum details, where's the physics? Building a real quantum cryptography system is also slightly out of my budget:(

I will have a blog post about what I've learned (should be up on [here](https://dronhazra.com/blog)) but this isn't the best place to pursue this.

## quantum physics

This falls into similar traps as quantum cryptography, in that it's very abstract. But, it didn't have the same background issue, because in many ways you start from first principles. And, some aspects of quantum weirdness are difficult not in the math, but in the thinking ("the physics"). The primary thing stopping me from doing this is that the topic is too broad. It's not really a project, it's more like "I want to learn about this thing". That's fine, but it's difficult to show evidence of that. Plus, the people watching don't really care if I learned or not, *they* want to learn. 

Plus, 3Blue1Brown did a [fantastic video](https://www.youtube.com/watch?v=MzRCDLre1b4) on the same subject. So go watch that instead.

## physics simulations

Spoiler alert: I'm doing this one:) It's a nice blend between abstract and real, with some nice physics but also programming and a clear connection to the real world. After talking to Mr. Fong, I realize that just having simulations isn't enough -- I should probably ground my simulations in reality.

Some implementation details:

So far as I understand it, I don't really need any extra software skills, just something to draw things on the screen and to update it's position. Here's the first [video](https://youtu.be/eED4bSkYCB8) I watched on it. They used manim to make the simulation, so I might as well go with that. I've been wanting to play around with manim for a while now anyway, so it works out.

I'll start with the same example in the video (projectile motion) but without the collision. My bucket list of simulations to make are:

 - Simple Harmonic Motion (Mass-Spring system)
 - Damped Harmonic Motion
 - Fluid Simulation (Navier-Stokes)

We'll see if I get to all of them. 

