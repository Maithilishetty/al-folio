---
layout: page
title: Optimal control for effective radiotherapy 
description: Internship project at Indian Institute of Science (IISc)
img: assets/img/cancer.jpg
importance: 4
---

This project was carried out as part of my semester long internship at the Indian Institute of Science. 
During this internship, I simulated an optimal controller for effective radiotherapy using Model Predictive Static Programming. This technique aims to solve 
the originial nonlinear optimal control problem in a computationally efficient manner. It derives it's ideas from Model Predictive Control (MPC) and Approximate Dynamic Programming (ADP).
The initial phase of my project was to use a modified MPSP technique called Impulsive-MPSP or I-MPSP to determine the distribution of radiation dosages to drive the number of cancel cells to zero using external beam radiotherapy. To model 
the tumor dynamics, a two-compartment oxygen model. This was a re-implementation of a [prior](https://www.sciencedirect.com/science/article/pii/S147466701643497X) work in this area.   

The second stage of the project involved extending this technique to account for the uncertainites in the model. 
