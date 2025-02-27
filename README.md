# Task1

For installation, 

If you are using ROS2 Foxy:
https://docs.ros.org/en/foxy/Tutorials/Beginner-CLI-Tools/Introducing-Turtlesim/Introducing-Turtlesim.html

If you are using ROS2 Humble:
https://docs.ros.org/en/humble/Tutorials/Beginner-CLI-Tools/Introducing-Turtlesim/Introducing-Turtlesim.html

If you are using ROS2 Jazzy:
https://docs.ros.org/en/jazzy/Tutorials/Beginner-CLI-Tools/Introducing-Turtlesim/Introducing-Turtlesim.html

When you launch Turtlesim, using the following command

```ros2 run turtlesim turtlesim_node```

When you run ```ros2 topic list``` while the robot simulation is running, you see an output similar to the following:

<img width="470" alt="Screenshot 2025-02-27 at 7 21 01 PM" src="https://github.com/user-attachments/assets/149136bf-62ae-4da2-8236-1d66dd9f36a5" />

Here the topic ```/turtle1/pose``` publishes the odometry of the turtle (i.e. the position, and linear and angular velocities).

Try running the following to see what is being published to this topic

```rostopic echo /robot_base_velocity_controller/odom```

Your task is to create a subscriber that takes the position (x, y) of the robot from this topic. You then have to use these values to calculate the distance of the robot from the origin. Then, using a publisher, publish that value to a new topic.

You need to upload the Python file(s) here as your submission along with the screenshot with the topic being displayed on the terminal.
