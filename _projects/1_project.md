---
layout: page
title: Adaptive Cruise Control
description: EECS 461 final course project
img: assets/img/dynamic-cruise-control.jpg
importance: 1
---

As part of this project, I
developed an adaptive cruise controller with automatic steering
control. The haptic wheel was used as a steering wheel for
the simulated vehicle on the simulink graphics software. The
position of the wheel obtained using quadrature decoding is
used to determine the angle of the front wheels. By toggling
one of the DIP switches, we can enable or disable the ACC
system. When disabled, we can manually control the speed of
the vehicle using the potentiometer. When ACC is enabled,
we use the first 8 DIP switches to set the speed of the vehicle.
As mentioned previously, ACC performs both velocity and
position control. When there is a lead vehicle within the
specified safe distance ahead of our vehicle, position control is
enabled. Otherwise, velocity control is enabled. The automatic
steering control is used to automatically align the vehicle at
the center of the road while performing any speed or velocity
control. The project was modeled entirely in simulink, auto-
code generation was utilized to obtain the C code processed
within S32K144.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <iframe src="https://drive.google.com/file/d/1s90g8vkiLGhlbYOCSgmCIyB8rntlR7on/preview" width="350" height="323" allow="autoplay"></iframe>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/haptic.jpeg" %}
    </div>
</div>
<div class="caption">
   Left, video of the working final project. Right: setup of the haptic wheel. 
</div>

