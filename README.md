# Baxter-Based Mirror Game

CPSC 584 - Human Robot Interaction
Shelly-Ginelle Sicat & Shreya Chopra
Baxter-Based Mirror Game

Playful interactions serve an important role in human development and interpersonal bonding [7]. Accordingly, human-robot interaction investigates on the importance of implementing aspects of social interaction and human behavior onto humanoid robots [5]. However, to implement such traits requires investigation into several aspects of psychology or sociology. As a humanoid developer, it is important to question whether robots need to encompass the same way of thinking as humans. In attempt to contribute to this paradigm we will be investigating on the popular topic of deception. Can robots make one believe something that is not true to gain some personal advantage? Should robots adopt this type of behavior? How would people react to a robot that is purposely attempting to deceive them? This paper investigates on the existing state-of-the-art, an implementation of a Baxter-based mirror game and how we aim to delve deeper into the discussion about humanoids potentially having a mind of their own.

This software project encompasses the communication between human and robot interaction. Utilizing the robot operating system, ubuntu and python; my partner and I were able to create an interface to control the movement of Baxter's arms. This then was used to mirror the actions of a human participant.

### Quickstart
Please run the following commands into ros to execute the program.

<!--Start - Enable and Untuck Baxter-->
cd ~/ros/baxter_ws
./baxter.sh
rosrun baxter_tools enable_robot.py -e
rosrun baxter_tools tuck_arms.py -u

<!--Go to our Project Folder-->
cd CPSC584-Baxter-Final-Project/baxter_examples/scripts

<!--Run This File To Start Game-->
python keyboard_control.py

<!--End - Disable and Tuck Baxter-->
rosrun baxter_tools tuck_arms.py -t
rosrun baxter_tools enable_robot.py -d
