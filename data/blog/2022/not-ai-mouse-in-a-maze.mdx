---
title: "Not AI mouse in a maze"
date: "2022-10-04"
tags: ["Python"]
draft: false
---

Building on the [Not AI Car](not-ai-car) project, I started out trying to get the car to drive across a maze. I changed the car to a mouse, as the lines detecting the edge looked like whiskers.

As I'd done with the track, the first thing to code was an algorithm to generate a random maze each time. The backtracking algorithm was well suited to this application and there were many implementations to choose from (see the code for links), so I just need to make a few modifications.

One of my rules for the mouse was that it wasn't allowed to remember where it had already been in the maze, so it couldn't map it out, crossing off dead ends after exploring them. It could however leave a "scent" trail that would slowly evaporate, so it could tell if it had been somewhere before if it returned soon enough. The measurements at various angles then included the level of scent in each direction, as well as the distances to the maze walls.

The algorithm for "driving" the mouse was then updated to not only keep a reasonable distance from the walls, but to also avoid the scent from a previous visit (at least until the scent had faded enough).

Dealing with dead ends was difficult. They were easy to detect but hard to get out, so I had to write code to detect if the mouse was in a dead end and then use a different method to calculate how to "steer" out.

This was a good project for learning how to deal with performance issues in Python. Most of the arrays used numpy and most of the calculations used numpy functions but performance was still slow. At one point, the mouse was only moving 16 frames/steps per second. I increased this to over 3,000 FPS by:
- Using profiling to identify the sections of code that most time was being spent on, so I could prioritise the code to be worked on. There are instructions on how to do this at the start of the programme.
- Using numba to JIT compile certain functions.
- Not rendering every frame. Pygame's rendering was taking more time than the calculations for each frame so, unless I wanted to play back what happened in navigating a particular maze, there was no need to render every frame.

The mouse was very good at getting through the maze, solving it 99% of the time, but there were a few cases that caused problems. So, it was time to see if using AI would help - wait for the next post to find out...

You can find the code and a video of the mouse on [Github](https://github.com/mikebarram/Not-AI-Mouse-In-A-Maze/)