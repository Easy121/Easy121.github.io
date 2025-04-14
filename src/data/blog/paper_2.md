---
author: Zijun Guo
pubDatetime: 2025-03-31
title: Fast Optimization-Based Trajectory Planning With Cumulative Key Constraints for Automated Parking in Unstructured Environments
featured: true
draft: false
tags:
  - planning
  - optimization
  - parking
description:
  Journal Paper. 
---

## Abstract

The optimization problem for trajectory planning becomes intractable as the dimensions of collision avoidance constraints increase. 
Existing methods either avoid unstructured environments or use simplified constraints that sacrifice a portion of the solution space. 
To tackle the intractability while preserving the feasible region, we introduce trajectory planning with cumulative key constraints (TPCKC), with which we won first prize in the trajectory planning competition of automated parking (TPCAP).
In the proposed method, only the violated vertex-to-polytope constraints are treated as key constraints and added to a collision avoidance constraint set.
Iteratively, an optimization problem with the constraint set is solved, and its solution is checked for new collisions.
The cumulation of constraints ends when the solution, restricted by key constraints only, is collision-free. 
The proposed method is compared with three optimization-based representatives on the TPCAP benchmarks. Practical real-time performance in all tested cases, together with the highest success rate and trajectory quality, is achieved with the proposed method. Besides simulation, TPCKC is also validated in a real-world experiment on an electric chassis platform under environmental changes.

## Publication

[IEEE Transactions on Vehicular Technology](https://ieeexplore.ieee.org/document/10945669)

[Accepted pdf](/pdf/paper_2.pdf)
