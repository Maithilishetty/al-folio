---
layout: page
title: Visual-inertial SLAM
description: EECS 568 final course project
img: assets/img/dataset_image.png
importance: 2
---

Simultaneous localization and mapping (SLAM) in
underwater environments pose major challenges due to limited
lighting, turbidity, lack of relevant features, imprecision of sen-
sors, presence of marine currents, etc. Therefore, in this project
we design a real-time image enhancement algorithm for visual
simultaneous localization and mapping (SLAM) for autonomous
underwater vehicles (AUV). Compared to atmospheric environ-
ments, underwater environment have issues with low contrast
and color distortion. Our method focuses on underwater gray-
scale image enhancement for a real-world dataset by using a
simplified enhancement model. In this project, the visual-inertial
SLAM methods such as ORB-SLAM3 and Open Keyframe-based
Visual-Inertial Odometry (OKVIS) are used. The results indicate
that the enhanced images have better performance than the
original images in feature points extraction and overall tracking
performance.


The main contributions of this project are: 
1. Application and performance analysis of the recently developed ORB-SLAM3 method in underwater environments.
2. Integration of real-time image enhancement pipeline within ORB-SLAM3 and OKVIS. 
3. Performance comparison based on absolute translational error (ATE).  


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/visual odometry.png" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/orbslam.png" %}
    </div>
</div>
<div class="caption">
   Left: ROV used with an underwater image of the seabed and the estimated trajectory in red. Right: ORB-SLAM3 system components.
</div>

Both OKVIS and ORB-SLAM3 rely on feature recognition and matching to calculate the estimated change in state from camera frames. 
Therefore, increased feature matching results in reduced failures and better tracking in both algorithms. This can be seen in the below set of figures for ORB-SLAM3. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/unmatch.png" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/enmatch.png" %}
    </div>
</div>
<div class="caption">
   Left: Matches before enhancement. Right: Matches after enhancement.
</div>