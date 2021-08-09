# Environment:

## Goal
The goal of your agent is to maintain its position at the target location for as many time steps as possible. It means that the double-jointed arm needs to touch the ball (target) as many many times as possible

![double-jointed-arm](arm.JPG)

## Game Over
The game ends after 1001 steps

## Rewards:
- double-jointed arm touches the ball: +0.1

## State Action:
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. 

Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

- State: There are 33 features on each State
- Action: There are 4 contunous possible actions to take in each State

## Solve the Task
In order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes

# The Model:
We will create a DDPG Model with:
- Replay Buffer
- Fixed Target 
- OUActionNoise

# Installtion:
Step 1: Activate the Environment
If you haven't already, please follow the instructions in the DRLND GitHub repository to set up your Python environment. These instructions can be found in README.md at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

(For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels.

Step 2: Download the Unity Environment
For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

Version 1: One (1) Agent
Linux: click here
Mac OSX: click here
Windows (32-bit): click here
Windows (64-bit): click here
Version 2: Twenty (20) Agents
Linux: click here
Mac OSX: click here
Windows (32-bit): click here
Windows (64-bit): click here
Then, place the file in the p2_continuous-control/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link (version 1) or this link (version 2) to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)

Step 3: Explore the Environment
After you have followed the instructions above, open Continuous_Control.ipynb (located in the p2_continuous-control/ folder in the DRLND GitHub repository) and follow the instructions to learn how to use the Python API to control the agent.

## Run the Code
run the file Continuous_Control.ipynb
