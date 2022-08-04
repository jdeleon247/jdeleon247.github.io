---
layout: post
title: Ragdoll + animation experiment
author: Jonathan
date: 2022-05-05
---

#### wacky flailing movement.


This project had a much larger scope at the onset, my first idea was to create a basic melee style fighting game and spend a bunch of time creating animations and blending them with IK. Having no experience actually creating animations, that quickly became a futile effort, so I chose instead to focus on the animation rigging portion of creating animations and create a ragdoll sim triggered by physical collisions:

![image](/assets/images/ragdoll_code.png)

Relatively straightforward code, but surprisingly effective once you have created a model with the appropriately sized, positioned and jointed colliders. Like this:

![image](/assets/images/model_with_collision.png)

Another portion I wanted to go deeper into was the transition between ragdoll and a controlled character, something you see in a lot of sandbox type games, but I was unfortunately unable to dedicate much time to that research. Instead I worked on a basic character controller that uses ternary operations to provide a relatively easy to understand interface for triggering animations in a blend tree:

![image](/assets/images/movement_code.png)

<img src="/assets/images/GitHub-Mark-Light-32px.png"> [Github link to project](https://github.com/jdeleon247/ragdoll-experiment)