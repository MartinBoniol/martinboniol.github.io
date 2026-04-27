---
permalink: /thesis
hidden: true
classes: wide
# layout: single-hf
# layout: single
layout: default
title: "Detection of Anomalies and Identification of their Precursors in Large Data Series Collections"
author_profile: true
redirect_from: 
  - /thesis
  - /thesis.html
---

# Verification of Neural Network mechanisms of ACAS-Xu

### Work In Progress, by Martin Boniol



## Context

Collision avoidance systems for air traffic, such as the Traffic Collision Avoidance System (TCAS), have been used for decades to reduce the risk of mid-air collisions. Their successor, the ACAS-X family, incorporates more advanced decision-making methods to address new challenges related to increasing air traffic and the emergence of drones.

The ACAS-X family includes two main variants:

- **ACAS-XA**: dedicated to commercial aviation, replacing legacy systems (TCAS and TCAS-II)  
- **ACAS-XU**: designed for drones, more complex, and introducing new challenges:
  - horizontal maneuvering
  - non-cooperative traffic management

The decision logic of these systems relies on Markov Decision Process (MDP) models to generate (offline) lookup tables (*LUTs – Look-Up Tables*) based on geometric state parameters of aircraft, enabling both horizontal and vertical collision avoidance guidance.
These LUTs store maneuver decisions depending on aircraft states.

#### Example of horizontal decisions

- **COC** (Clear of Conflict)  
- **WL / SL** (Weak / Strong Left)  
- **WR / SR** (Weak / Strong Right)  

Despite their deterministic nature, these LUTs are extremely large, making their deployment on embedded systems challenging.  
Several approaches have proposed compressing them using neural networks, but these methods rely on approximations and raise safety and formal verification concerns.

In this context, this PhD work aims to analyze, evaluate, and improve compression and verification methods for ACAS-Xu systems.



[Back to main page](https://boniolp.github.io/)
