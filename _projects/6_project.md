---
layout: page
title: Reinforcement learning & adaptive control
description: Projects on RL and adaptive control
img: assets/img/rl.png
importance: 6
---

As part of my bachelor thesis, I designed a deep determinstic policy gradient algorithm to control a robot manipulator in uncertain environments. Primarily, deep reinforcement learning (DRL) addresses the
problems that previously limited the performance of RL algorithms while working with high-dimensional state and action
spaces. In this project, I explored the deep deterministic policy gradient (DDPG) algorithm that operates over continuous action spaces. The application of reference tracking for a two-
link robot manipulator (TLRM) in uncertain environments was considered. The TLRM is subjected to uncertainties such
as frictional forces and external torque disturbances. In the simulation study, comparison of the performance of the RL-
based controller with the well-known proportional-derivative (PD) controller. Results indicate a considerable improvement
in the mean square error (MSE) and variance accounted for (VAF) metrics when the RL-based controller is utilized. This paper was published as part of the proceedings of the [Indian Control Conference, 2021](https://ieeexplore.ieee.org/document/9703155)

For more details, refer to the below slides: 

<object data="/assets/pdf/ICC_Presentation.pdf" width="1000" height="1000" type='application/pdf'></object>

&nbsp;


**Adaptive Control: NAVARCH 583 Final Project** 

Transient response of adaptive systems is not predefined while their steady state behaviour can
be predicted. Large errors in the initial parameter estimates can result in poor and oscillatory
transient performance characteristics. This affects operational safety and reliability and can also
result in failure in practical systems. Examples of such systems include flight control systems
due to controller effector failures and flexible transmission systems. Thus, there is a need
to improve the transient performance of adaptive systems, in terms of parametric, identification
and tracking errors. To achieve this, concepts of multiple models, switching and tuning have
been applied extensively in control theory. As part of our project, we conducted
a study on the efficacy of multiple estimation models and investigated their use in adaptive
systems for identification and control in order to improve transient performance. Furthermore,
detailed comparative studies are presented between the different parameter estimation algo-
rithms, switching methodologies and sensitivity to number of estimation models 

The report attached below has more details on the algorithm and the results: 

<object data="/assets/pdf/NA_583_Report.pdf" width="1000" height="1000" type='application/pdf'></object>

