# HomeService
Source code and files for the Udacity Home Service Robot project
This project depends on the following packages

Import these packages now and install them in the src directory of your catkin workspace. Be sure to clone the full GitHub directory and not just the package itself.

Import these packages now and install them in the src directory of your catkin workspace. Be sure to clone the full GitHub directory and not just the package itself.

[gmapping](https://github.com/OpenSLAM-org/openslam_gmapping): With the gmapping_demo.launch file, you can easily perform SLAM and build a map of the environment with a robot equipped with laser range finder sensors or RGB-D cameras.

[turtlebot_teleop](https://github.com/turtlebot/turtlebot): With the keyboard_teleop.launch file, you can manually control a robot using keyboard commands.

[turtlebot_rviz_launchers](https://github.com/turtlebot/turtlebot_interactions): With the view_navigation.launch file, you can load a preconfigured rviz workspace. You’ll save a lot of time by launching this file, because it will automatically load the robot model, trajectories, and map for you.

[turtlebot_gazebo](https://github.com/turtlebot/turtlebot_simulator): With the turtlebot_world.launch you can deploy a turtlebot in a gazebo environment by linking the world file to it.

Clone the HomeService.zip, unzip it, and copy the files into your catkin_ws/src directory.

test_slam.sh - Will launch the turtlebot in the custom environment and launch a keyboard_teleop node to test the slam performance by manually driving the robot around and observing the map in RVIZ

wall_follower.sh - Will launch the robot within the environment and autonmously navigate using a wall following algorithm to demonstrate mapping the environment.

test_navigation.sh - Will launch the robot in the environment and load the map. Using the Nav goal tool in RVIZ, this can demonstrate the robots ability to navigate to a desired goal position.

pick_objects.sh - Will launch the robot in the environment and send a goal location in order to navigate to a pickup and dropoff location

add_markers.sh - Will launch the robot in the environment and test the marker functionality by publishing a marker at the pickup and dropoff location consecutively.

home_service.sh - Will launch the robot in the environment, publish a marker at the pickup location, send the goal to the robot, once the robot is at the goal, a pause is used to simulate pickup time, and the marker is removed. Then, the robot is sent the goal location. Once the robot reaches the goal location, the marker is published again to represent delivery of the item.
