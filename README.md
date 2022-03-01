# Machine Teaching for Human Inverse Reinforcement Learning

This repository primarily consists of 

* Methods of a) selecting demonstrations that effectively summarize the agent's policy to a human by considering human knowledge and human counterfactuals, and b) requesting demonstrations of what the human believes an agent would do in specific environments. See main.py
* Implementations of various MDP testbeds using David Abel's [simple_rl framework](https://github.com/david-abel/simple_rl). 

models/* contains the training and testing demonstrations used in the user study, which were created using Python 3.9.

Required packages include [numpy](http://www.numpy.org/), [matplotlib](http://matplotlib.org/), [pypoman](https://github.com/stephane-caron/pypoman), and [sage](https://doc.sagemath.org/html/en/index.html) to perform computational geometry with polytopes (i.e. BEC regions, see below), and [pygame](http://www.pygame.org/news) if you want to visualize some MDPs.

This repository contains raw code that has not gone extensive cleanup, which will be done upon acceptance of the paper.
