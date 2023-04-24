# Obstacle-Avoidance-integrating-Safety-Bound-with-Reinforcement-Learning

Author: Jueming Hu, Arizona State University

Email: jueming.hu@asu.edu

This fork is used to provide an implementation for [1].

[1] demonstrates path planning for UAS obstacle avoidance using a **probabilistic dynamic anisotropic (DA) safety bound coupled with reinforcement learning (RL) methods**. The DA safety bound is influenced by UAS performance, weather condition, and uncertainties in UAS operations such as positioning error. 

A **new reward function** based on the operational DA safety bound concept enables trajectory optimization under risk-based dynamic separation criterion. A **Q-learning RL algorithm** is used to learn the optimal path plan with the DA safety bound reward function. A comparison of optimized trajectories around static obstacles is conducted to show the deconflict capability of the DA safety bound with RL methods. 

## Files

- main_RL_train_result.ipynb: **main file for training and visualization.**

- SafetyBound.py: obtain the size of safety bound.

- geometryCheck.py: check potential collision among different shapes.

- ObstacleAvoidanceENV.py: define RL environment, including transition model and reward function.

- plotting.py: visualization of RL training process

- draw.py: visualization of learned trajectories

- Q_learning.py: Q-learning algorithm




## Required python packages

- gym
- itertools
- matplotlib
- numpy
- pandas 
- sys
- matplotlib
- collections
- shapely
- math
- random
- sys

## Reference
[1] Hu, J., & Liu, Y. (2020). UAS conflict resolution integrating a risk-based operational safety bound as airspace reservation with reinforcement learning. In *AIAA Scitech 2020 Forum* (p. 1372).
