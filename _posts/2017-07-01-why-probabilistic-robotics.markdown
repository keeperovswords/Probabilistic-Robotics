---
layout: post
title:  "Why Probabilistic Robotics?"
date:   2017-07-01 09:50:51 +0200
categories: main
---

<h1>Basic</h1>
Robotics involve two main concepts: control and perception permanently. Control means how the robots interactive in the real world such as motion, localization etc. Perception
enables the robots to perceives the information from environment by armed with some devices such as sensor and radar etc. Robotics is kind of science to build a feasible
solution for our control and perception tasks. As robots act in the working environment, the physical world changes inherently unpredictably. The unpredictable factors are abstracted as <strong>Uncertainty</strong>.

<h1>Uncertainty</h1>
Basically, the uncertainty can be summaried as the following parts:
<ul>
<li>Environment: In our live world there exist always the unpredictability, say, you want to design a autonomous driving car. You can build your simulation experiment carefully, but it's almost impossible to build a real case in highway, cause the dynamics of this scenario changes unpredictably.</li>
<li>Sensor: Sensor is the only way that our robots percepts or perceives the information of the environment. Normally the perception is limited by the range and resolution of sensors. Furthermore the sensor measurements delivers also the noisy information by the sensor perturbations.</li> 
<li>Robots: As the robots works its actuation is also inaccurate, say, the kinematic configuration looses the actuation accuracy.  The wear and tear contributes to this inaccuracy as well as physical connection factors.</li> 
<li>Models: Models or modeling is the only way that we abstract the environment. They describes the underlying processes of the robot and environment partially. So it's also inaccurate.</li> 
<li>Computation: Robots are real-time system. So it limits the amount of computation as we need. Most algorithms compute approximately over time runs, which is also a factor of inaccuracy.</li> 
</ul>
All of these factors contribute to uncertainty or unpredictability. For building a robot we need to handle them appropriately.

<h1>Probabilistic Robotics</h1>
With the probabilistic theory we can abstract and handle the uncertainty smoothly. The uncertain activities can be represented as the probabilistic distribution over the possible hypotheses. 
The ambiguity or degree of belief can be nicely accommodate the factors we mentioned before. The degree of belief implies the momentary estimate of the considered elements, say, the state of current robots in localization problem. 
Probabilistic approaches for estimation is the **only** typically approach that's robust again the sensor limitations, environment dynamics and etc. This approach needs a weak requirements of model accuracy than any other algorithms do. 
It's also broadly applicable to problems involving perceptions and actions in real world.<br />

As the live world changes, the model of robots and environment changes correspondingly. As robot works the uncertainty lurks anywhere and anytime. With probabilistic model we can abstract the model and handle them in a plausible way to build robot conceptions. The disadvantage of probabilistic approach should be also considered. 
Say, the probabilistic algorithms take all probabilistic densities into account and it's less ineffective and needs more computation resources.