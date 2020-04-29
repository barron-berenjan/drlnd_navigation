# Dueling DQN

This repository provides the code required to train an agent using a Dueling Deep Q-network to solve the _Navigation_ assignment from  Udacity's Deep Reinforcement Learning Nanodgree

## Environment

In this project, an agent is trained to navigate (and collect bananas!) in a large, square world. 

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal is to train an agent that collects as many yellow bananas as possible while avoiding blue bananas.

The __state space__ has 37 dimensions which include the agent's velocity, along with ray-based perception of objects around the agent's forward direction. 

There are 4 discrete actions available for the agent to take: `LEFT`, `RIGHT`, `UP`, `DOWN` and the agent learns to choose the best one. 

State Space: each state has 37 dimensions

The task is episodic, and to solve the environment, the agent requires to get an average score of +13 over 100 consecutive episodes.

## Dependencies and Set-up

To set up your python environment to run the code in this repository, follow the instructions below.

1. Clone this repository

2. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name drlnd python=3.6
	source activate drlnd
	```
	- __Windows__: 
	```bash
	conda create --name drlnd python=3.6 
	activate drlnd
	```
  
 3. Clone the [DRLND repository](https://github.com/udacity/deep-reinforcement-learning), and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

 4. The environment for this project is based on the [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents). For this project you will __not need__ to install Unity and a pre-built environment can be downloaded from one of the links below. You need only select the environment that matches your operating system:

	- __Linux__: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
	- __Mac OSX__: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
	- __Windows (32-bit)__: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
	- __Windows (64-bit)__: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

__Note: Unzip the file in the same directory as the notebooks from this repository.__


### Training the Agent

Run the cells in `DuelingDQN_Train.ipynb` to train the agent. The agent will stop training once on average of +13 bananas are collected over 100 consecutive episodes.

### Watch A Trained Agent in action

Run `DuelingDQN_Control.ipynb` to watch a pre-trained agent collect Bananas!


