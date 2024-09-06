# Reasoning about Counterfactuals when Demonstrating Robot Decision Making to Humans

This repository contains code for methods described in the following paper: 

- Michael S. Lee, Henny Admoni, Reid Simmons **Reasoning about Counterfactuals to Improve Human Inverse Reinforcement Learning**, IROS, 2022,

which introduces a method for teaching robot decision making to humans through demonstrations of the robot's key decisions in a domain. 

In particular, we observe that an informative demonstration is one that differs strongly from the human's expectations of what the robot will do given their current understanding of the robot’s decision making, and we consider human beliefs and counterfactuals over robot behavior when selecting demonstrations accordingly.

The [paper](https://arxiv.org/pdf/2203.01855) and [user study](https://github.com/SUCCESS-MURI/counterfactual_human_IRL_study) used to validate our methods, as well as follow-on work, are available at https://symikelee.github.io/.

## Running the code

Run `main.py` to select a) demonstrations that effectively summarize the robot's policy to a human by considering human beliefs and counterfactuals over robot behavior, and b) tests that ask the human to demonstrate what they believe the robot to do in new situations. 

`models/*` contains the training and testing demonstrations used in the user study, which were created using Python 3.9.

Required packages include [numpy](http://www.numpy.org/), [matplotlib](http://matplotlib.org/), [pypoman](https://github.com/stephane-caron/pypoman), and [sage](https://doc.sagemath.org/html/en/index.html) to perform computational geometry with polytopes (i.e. BEC regions, see below), and [pygame](http://www.pygame.org/news) if you want to visualize some MDPs.

This repository also contains implementations of various MDP testbeds built using David Abel's [simple_rl framework](https://github.com/david-abel/simple_rl). 
