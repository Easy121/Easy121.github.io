---
author: Zijun Guo
pubDatetime: 2024-10-04
title: Time-Optimal Learning-Based LTV-MPC for Autonomous Racing
featured: true
draft: false
tags:
  - control
  - model predictive control
  - autonomous racing
description:
  Conference Paper. 
---

## Abstract

Autonomous racing is a time- and accuracy-critical application of vehicle motion planning and control techniques. Despite being
promising for its ability to handle constraints, model predictive control (MPC) for autonomous racing is limited by the relatively low computational speed and the problem of model mismatch. In this work, we present a time-optimal linear-time-variant-MPC (LTV-MPC) that incorporates a min-time objective function, the friction ellipse constraint, and the successive linearization over the prediction horizon to improve computational speed and prediction accuracy. To tackle model mismatch, the proposed LTV-MPC is further combined with Gaussian process regression to learn the lateral tire force error. Compensation for the error is implemented over the prediction horizon and on the friction ellipse constraint. This work presents simulation validation on the racing track of
Formula Student Autonomous China (FSAC) and experimental validation on a self-designed track. We show that compared with nonlinear
MPC, the proposed LTV-MPC reduces the average computation time from 66 ms to 2.5 ms with a 0.6% increase in lap time. With learned tire force error, a 2% reduction in lap time can be achieved.

## Publication

[16th International Symposium on Advanced Vehicle Control](https://link.springer.com/chapter/10.1007/978-3-031-70392-8_33)

[Open-source pdf](/pdf/paper_1.pdf)
