---
title: "euler! you failed me!"
date: "2021-05-05"
---

Progress update, split in 2 parts: technical and other.

## technical update

So I learned about Euler's method (of numerical integration) and that seemed like a perfectly logical place to start. Here's the projectile motion one I promised:

![Projectile Motion](./ProjectileMotion.mp4)

Looks a little choppy...

Now for where Euler hath failed me:

![Spring-Mass 1](./SpringMass.mp4)

What the heck is going on here?

Energy isn't being conserved (I'm glad Mr. Fong didn't test this with his face on the line). Part of the problem is that my framerate is too low. I rendered the same code at 60fps:

![Spring-Mass 2](./SpringMass1.mp4)

It's better, but energy still isn't being conserved.

I did some digging, and it turns out that a better method is the Euler-Cromer method. The only difference between it and what I was doing is that you update the velocity, then update the position. In the proper Euler's method, you update both at the same time. In the modified version, you update the velocity and use the updated velocity to update the position. What this basically ensures is that the velocity (and hence the kinetic energy) doesn't behave unphysically (i.e. violate the conservation of energy).

All this amounts to in code is just moving one line of code up 1 line. Fun!

## ~ business ~ update 

I had a conversation with Mr. Fong, and I need to focus on what I'm going to put in my video. I had the idea of doing fluid simulations, and talking about solving differential equations, and how differential equations are the language of reality (incidentally as I grow older I seem to be growing fluent in *many* languages of reality). I'll have to cut those (I think).

Ultimately the audience isn't someone with *my* knowledge of physics, it's someone with a good amount *less* familiarity with physics. That's part of why fluid simulations are a bad idea -- the equations governing them aren't simple, and they also look much more opaque (due to their use of derivative notation *and* gradients). Also, they're hard, and not really that close to the other simulations I've been doing. 

Mr. Fong came up with a good idea: talk about wind tunnels and the such (I'm sorry Mr. Fong I didn't write down the quote). Basically, simulations provide engineers and physicists ways to test things without the material costs of building a real, physical object. Instead of building 100 suspension springs and testing each of them, use a simulation to get an approximate solution, and test it against reality.

The same thing applies to wind tunnel testing. Once you have a 3d model of the car, you can simulate a wind tunnel and change the major issues before you spend a lot of money and time using a real wind tunnels.

I think this is a much better hook than my original idea, which was trying to convey a generic the-world-is-math-and-thats-beautiful idea. 

Hopefully people enjoy it!
