[//]: # (Image References)

# Project 1: Navigation

### Project Details

This project is part of the Deep Reinforcement Learning Nanodegree program offered by Udacity.

In this project, an agent is trained to navigate and collect objects in a large, square world. The world contains blue and yellow bananas. The agent's goal is to collect as many yellow bananas as possible before the episode ends while avoiding blue bananas. The state space is a continuous 37 dimensional observation vector, $s \in \R^{37}$. The state, $s$, contains information about the agent's velocity and ray based perception of objects currently in front of the agent. The action space is discrete and can take on four different values $\mathcal{A}= \{ 0, 1, 2, 3 \}$. Each action, $a \in \mathcal{A}$, corresponds to the agent moving forward ($a=0$), backward ($a=1$), turning left ($a=2$), or turning right ($a=3$). The agent recieves a reward fo $+1$ for every yellow banana collected and $-1$ for every blue banana collected. 

The environment is considered solved when the agent obtains an average score of greater than $+13$ over 100 consecutive episodes.

![Trained Agent][image1]

### Getting Started

The following instructions detail how to set up the environment and are provided as part of Udacity's Deep Reinforcement Learning Nanodegree program.

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the DRLND GitHub repository, in the `p1_navigation/` folder, and unzip (or decompress) the file. 

### Instructions for Training an Agent

The code for training an agent is contained in `DQN_Navigation_Banana.ipynb`. 
Running this notebook will allow you to train an Agent in this environment using Deep Q-learning or load a pretrained agent (whose weights are contained in model.pt).

After training, you will be able to visualize the agents performance in real time and see the agent's score (how many yellow bananas minus how many blue bananas the agent collects). If loading the pretrained model, the score should be approximately 17.