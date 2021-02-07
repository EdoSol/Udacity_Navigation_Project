Project Description
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas. Each episode ends after a given number of steps.
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:
•	0 - move forward.
•	1 - move backward.
•	2 - turn left.
•	3 - turn right.
The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.
Setup
1.	A requirements.txt file containing the necessary packages for this project is included in this repository. Further details can also be found here.
2.	The necessary banana environment to run the project can be downloaded from one of the links below for different operating systems:
o	Linux: click here
o	Mac OSX: click here
o	Windows (32-bit): click here
o	Windows (64-bit): click here
The environment needs to be called within the Jupyter notebook described below. The corresponding location is highlighted accordingly.
(For Windows users) see also this link concerning 32-bit version or 64-bit versions of the Windows operating system.
(For AWS) see also: enabling a virtual screen or use this link to obtain the environment.
3.	The environment file needs to be placed in the repository folder, and unzipped or decompressed.
Solution
The notebook Navigation.ipynb contains the code to set up the environment and the outer episode iteration to solve the reinforcement problem. Our solution uses a (double) deep Q-learning network (only standard feedforward layers) and experience replay.
The agent, the deep Q-Network and memory buffer are implemented in the file dqn_agent.py. The Agent class takes an optional parameter to choose between a standard Q-Network or a Double-Q-Network (see also this paper). The

