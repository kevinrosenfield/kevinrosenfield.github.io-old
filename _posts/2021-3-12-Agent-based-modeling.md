---
layout: post
title: Agent-based models
---
<div style="text-align: left">
I have been spending a lot of time coding agent-based models over the last few months. Aside from being incredibly fun to work on, I'm hoping that these models will allow me to test several hypotheses related to behavior, mating, and evolution in humans and non-human primates.
</div>

<br>

<div style="text-align: left">
Agent-based models are a specific type of mathematical model that seek to understand the emergence of phenomena at one level of organization (e.g. the human brain, a population of chimpanzees, or a galaxy) by modeling the behavior of 'agents' at lower levels (e.g. individual neurons, chimpanzees, or stars). Key to this kind of procedure is understanding the ways in which agents interact with, and even modify, characteristics of other agents and the environment itself.
</div>

<br>

<div style="text-align: left">
For example, one of the most intuitive agent-based models is known as the <a href="https://ccl.northwestern.edu/netlogo/models/WolfSheepPredation">wolf-sheep predation model</a>. The main question it seeks to address is "What properties allow a predator-prey ecosystem to reach and maintain stability (here, stability simply means that neither species goes extinct)?" The clip below shows how this plays out in an agent-based modeling program called Netlogo (I did not write this particular model). As you'll see, this ecosystem (a simple one, only including sheep and wolves) is not stable; the wolves go extinct as a result of huge swings in sheep and wolf poulation sizes.
</div>

<br>

<div style="text-align: center">
<video width="400" height="400" style="margin:0 auto" controls>
  <source src="/images/IMG_7462.mov" type="video/mp4">
</video>
</div>

<br>

<div style="text-align: left">
Agent-based models are meant to be simplistic. They do not mirror the complexity of the real world, and for <b>very</b> good reason. If someone figured out a way to write a model that included all of the variables and interactions that occur in a real wolf-sheep ecosystem, it would be useless. First of all, if we're going to model things <i>exactly</i> as they are, we might as well just observe them in the real world. More importantly, models of every kind are helpful precisely due to their simplicity, not despite it.
</div>

<br>

<div style="text-align: left">
When we design experiments to try to tease apart causes and effects, one of our most important tasks is to ensure that variabes not related to our research question are experimentally controlled (i.e. that they do not vary in ways that might influence the outcome). This is precisely what we are doing by leaving certain variables out of an agent-based model when we are asking a question that does not involve them. Of course, there is a downside to this, namely that when make things very simple, we sacrifice external validity, or the ability of the model to accurately depict what happens in the real world. But that's okay, because other researchers will conduct studies with high external validity by studying real wolves and sheep!
</div>

<br>

<div style="text-align: left">
All this being said, the video shows that even an agent-based model can be <i>too</i> simple. Why exactly do the wolves go extinct (to be clear, if you run the model many times, it is not always the wolves; sometimes the sheep die out)? It turns out that, while fluctuations in sheep population size keep wolf population size in check, there is nothing to stop the sheep population from exploding. As you'll see in the next video, when we tell the sheep that they need to eat or they'll starve, and provide a limited nutritional resource (grass), their population will remain in check, stabilizing the entire ecosystem.
</div>

<br>

<div style="text-align: center">
<video width="400" height="400" style="margin:0 auto" controls>
  <source src="/images/IMG_7464.mov" type="video/mp4">
</video>
</div>

<div style="text-align: left">
When sheep need to eat grass to stay alive, it is much rarer for either sheep or wolves to go extinct. What truly makes this an agent-based model rather than some other kind of model is that, under the hood, each agent has <i>individual characteristics</i>. Each sheep and each wolf has it's own unique value representing its curent nutritional needs, which changes everytime it eats. The higher-level pattern that emerges (e.g. ecosystem stability, species extinction) is the result we are interested in.
</div>

<br>

<div style="text-align: left">
In most models, as in the wolf-sheep model, agents also have unique x- and y-coordinates, making them <i>spatially explicit</i>. This makes the models a much more realistic in some ways. As in the real world, sheep can only eat from food patches they are physically close to.
</div>

<br>

<div style="text-align: left">
In a future post, I'll dive into some of the code necessary to get an agent-based model off the ground in Netlogo, Python, and R.
</div>

<br>

<div style="text-align: left">
-Kevin
</div>
