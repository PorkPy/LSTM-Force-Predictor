# LSTM-Pulling-Force-Predictor
This repository holds the data and code to implement an LSTM model in Pytorch that can predict pulling forces based only on a UR10 robots joint positions.
This work is part of a Phd study on autonomous manipulation of long thin flexible objects such as hoses, wiring harnesses and cables. Such objects are known in the robotic manipulation community as deformable linear objects or DLOs.
The task of the robot in this work was to pull a hose through a small orifice towards a goal position, such as a hose connector. 
Recent work has shown that reinforcement learning (RL) can be used to teach robots how to pick objects and place them elsewhere in a task-space, but what happens if those objects are constrained by the environment? What happens if a long and thin object gets wrapped around obstacles in the task-space while the robot is trying to reach the goal?
Simple pick and place tasks can be solved using static nonlinear function approximators such as neural networks, but when the object being manipulated is in constant contact with the environment, the route the robot takes through the task space is vitally important. 
The sequence of actions the robot takes  and the resultant forces can be modelled using a recurrent neural network such as a long-short-term-memory (LSTM). An LSTM incorporates a hidden state which remembers previous states and uses this memory together with the current observation to make either future predictions or suggest actions.
 
