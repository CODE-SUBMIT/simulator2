# Multi-agent Deep Reinforcement Learning for 3D Furniture Layout Simulation in Indoor Graphics Scenes

## Installation
Please install the dependencies via conda:
 * PyTorch >= 1.0.0
 * networkx
 * numpy
 * Python >= 3.6

## Introduction

In the industrial interior design process, professional designers plan the furniture layout achieve a satisfactory 3D design for selling. In this repository, we explore the interior graphics scenes design task as a Markov decision process (MDP) in 3D simulation, which is solved by multi-agent reinforcement learning (RL). The goal is to produce proper furniture layout in the 3D simulation of the indoor graphics scenes. In particular, we first transform the 3D interior graphic scenes into two 2D simulation scenes. We then design the simulated environment and apply two reinforcement learning agents to learn the optimal 3D layout for the MDP formulation in a cooperative way. 

## Numerical results

We conduct our experiments on a large-scale real-world interior layout dataset that contains industrial designs from professional designers. Our numerical results demonstrate that the proposed model yields higher-quality layouts as compared with the state-of-art model.  

The figure below illustrate an example of furniture layout produced in the 2D simulation graphic scenes. It is obvious to see that only one out of six 3D layouts (in red block) is practical in the real 3D graphic scenes.

![2D&3D](fig1.jpg)

The figure below shows the simulation environment for the layout of furniture in the 3D indoor scenes. The 3D graphic scenes can be decomposed into two 2D simulation scenes. Two RL agents are trained cooperatively on $S^1$ (the x-y plane) and $S^2$ (the y-z plane), respectively. 

![MDP Formulation](fig2.jpg)

The 3D graphic scene is first decomposed into two 2D scenes (first row). Two simulators then transfer the real indoor scenes into two 2D simulated graphics indoor scenes (second row). Two RL agents produce 2D furniture layouts (third row) given initially random position (fourth row) in the 2D space. Finally, a 3D layout is produced in the 3D graphic scene (last row).

![Results](fig3.jpg)

Codes and more results will be released soon. Please contact deepearthgo@gmail.com if you have any questions.

