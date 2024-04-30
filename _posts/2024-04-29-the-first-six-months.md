---
layout: post
title:  The First Six Months
categories: [blog,]
---
Last October I quit my job to explore new career options.
This post is a review of how that's gone, what I've been up to and where I would like to go from here.

## What I've Been Doing

### Vulkan
Graphics Programming is the #1 career choice for me right now, so naturally I am learn Vulkan.
I had followed [OpenGL Tutorial](http://www.opengl-tutorial.org/) and [Vulkan Tutorial](https://vulkan-tutorial.com/) already some years ago but coming back to my repo for the latter I was quite paralysed by the complexity.
There had obviously been a lot of re-typing example code verbatim and not enough understanding.

This time around I have taken the approach of writing a wrapper as I develop simple apps that allow me to tear off comprehendible chunks.
Instead of racing to the first triangle, the first app I've made is an image viewer.
Provided with a filepath it will decode the image (using [stbi](https://github.com/nothings/stb/blob/master/stb_image.h)), send it to the graphics card and present it to a window.
I would totally recommend this as an exercise for a Vulkan student as it requires only limited number of concepts and what's more these concepts are somewhat at 'either end' of a Vulkan pipeline, so form a scaffolding that can be filled-in with more features.

<video  style="display:block; margin:0 auto; width:50%; height:auto;" autoplay="autoplay" controls loop="loop">
    <source src="{{ site.baseurl }}/images/image-viewer-demo.mp4" type="video/mp4" />
</video>

My next project is [Boids](https://en.wikipedia.org/wiki/Boids) running in compute shaders.
Now the fun begins.
How many boids will I manage to fit into 16.67ms?

<video  style="display:block; margin:0 auto; width:90%; height:auto;" autoplay="autoplay" controls loop="loop">
    <source src="{{ site.baseurl }}/images/boids-demo.mp4" type="video/mp4" />
</video>

I'll be posting updates with my progress on this project.

### Game Jams
In early February I participated in the in-person [Game Dev London](https://www.gamedev.london/) [Global Game Jam](https://globalgamejam.org/).
As a consequence I can proudly present [Not Amused](https://flatwhitecanvas.itch.io/notamused), our Medieval Court Quip-Em-Up.
It was my first game jam and my first time making a game.
I think the memories have been weathered smooth enough that I can now call this 48-hour crunch simulation 'fun'.
Actually since it ended I did feel that I would do it again, especially since next time I would not be starting with zero-knowledge of any game engine (we used Unity).
It was a real privilege to work with some very talented people; while the gameplay is quite 'broken' I was happy that the assets from the writers, visual artist and sound designers made it in to the submission.

<iframe style="display:block; margin:0 auto;" width="560" height="315" src="https://www.youtube.com/embed/6BDhy0-FWlM?si=NXR_op3p0Xq2J7Xr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

In March I submitted myself to another one: Greenwich Game Jam.
Being familiar with Unity definitely helped and on top of that this time we had a second programmer!
I believe the theme was 'moderation', so our game was about balancing a sailing boat while the crew run around the deck completing tasks.

<iframe style="display:block; margin:0 auto;" width="560" height="315" src="https://www.youtube.com/embed/HogWrpeXQ40?si=CetgPH1u-HXFBB1N" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### CADA
I've been getting involved in the [Autonomy](https://autonomy.work/) think tank's [new initiative](https://autonomy.work/cada/) aiming to nucleate and co-ordinate technically-skilled, left-wing people.
I'm very much looking forward to meeting and learning from like-minded people and putting personal project time into research that could have real political impact.


### Kripkenstein
Prompted by an anecdote about a couple of school students who learned 'the wrong rule' during a class on long-division, I have returned to Kripke's '*Wittgenstein On Rules and Private Language*'.
Do we mean the same thing by 'addition'? Do you mean the same thing you think you used to? What is rule-following anyway?
I was first made aware of this book during my undergrad but I didn't give it a serious read until now.
I can say I found it as frustrating now as I did then.
My own view is informed predominantly by Noam Chomsky's philosophy (science) of language.
I hope to post some thoughts here (none of them particularly novel) to get them out of my system.

### Cycling
Various adventures with camping equipment strapped to my bike.
Kielder Forest and the North Pennines were particularly fun.

<img src="{{ site.baseurl }}/images/north-pennines-bike.jpg" style="display:block; width: 90%" alt="My bicycle up a hill"/>


## What's Next

### Gaussian Splats
I would like to reproduce the [Gaussian Splat](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/) paper.
Gaussian splatting is a new photogrammetry technique which enables recording and rendering of photo-realistic 3D scenes using only video capture (no camera pose necessary).
I'm very excited about diving into the details of this technique as it's a rare milestone able to boast both theoretical novelty and state-of-the-art performance (in terms of both photo-realism and rendering speed).
It will be interesting to see if the ultra-fast gaussian rendering can be applied to real-time rendering in other scenarios.
Also fascinating is how this 'hand-crafted' representation beat out the previous state-of-the-art neural-network based [NeRF](https://www.matthewtancik.com/nerf) techniques.

### Machine Learning and Linguistics
The recent success of the [transformer architecture](https://arxiv.org/abs/1706.03762) in machine learning, particularly in Natural Language Processing has been curious to me for two reasons.
Firstly there seems to be minimal interest in how insights from the cognitive science of linguistics can be applied to the improvement of these models, instead the pendulum seems firmly set in letting the models figure out the structure of the problem themselves.
This seems to me to be in analogy with how early neural network applications to computer vision used fully connected networks to take on character recognition, only later exploiting the translation-invariance of the problem with the invention of convolutional neural networks.
I have to admit that the impressive performance of ChatGPT and its ilk does make grammar seem like a problem easily solved by optimisation of enough parameters over a large enough corpus (the output from these models seems to always be well-formed sentences to me).
And, in-fact, the transformer architecture is so efficient that it was immediately successful in its application to computer-vision and audio processing.
For now, who should care about silly sub-problems like syntax?

The second curiosity is the lack of research into cognitive linguistics making use of 'large language models'.
I'm not an apprentice, let alone an expert in this field (or machine learning), however from an understanding of human language perspective, it does seem enticing to try to understand what LLMs have learned about syntax.
Of course this immediately lands you in territory I hear ML people are calling 'mechanical interpretability', or the persistent and hard question of how do we make sense of the computation our models are performing.

### FM Radio interference
I've played many, many hours of the military flight simulator [DCS](https://www.digitalcombatsimulator.com/) over the past decade or so, including in online communities where we have fun attempting to fly as the real pilots would.
One of the greatest 3rd-party tools that help us in the quest for more and more realism is [DCS Simple Radio System](http://dcssimpleradio.com/), a VoIP program which applies realistic radio effects to communication between virtual cockpits.
The software is an incredible achievement and is used almost universally by the multiplayer DCS community.
From what I can tell it's largely the work of one person, which we are allowed to use open-source and for free.

One aspect of real-world radio communication SRS simulates is FM radio interference.
FM radio is different to AM radio in that the audio signal is not a linear functional of the radio signal.
As a consequence what you hear when two FM radios transmit simultaneously on the same carrier frequency is not the same as two people talking over each other, instead you get a horrible warbling interference.
This is simulated in SRS, but as far as I can tell in a quite rudimentary way.
Specifically the implementation seems to be something like "if two people are transmitting then discard their audio and instead play a loud warbling tone".
What's missing is that the strength of effect is actually dependent on the relative signal strength of the two transmitters.
If one of the transmitters is much closer than the other then what's heard by the receiver is more like a superposition of the warbling tone with the transmitted audio of the nearby transmitter.
(This can be heard at times during [this video](https://www.youtube.com/watch?v=SL6U6RJ1qdM).)
What I would like to do is understand and simulate FM radio demodulation and implement a more-realistic version of FM radio interference in SRS.