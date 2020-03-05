# listner

---------------Create a ROS Workspace--------------
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
source devel/setup.zsh  ( add the workspace to your ROS environment )
---------------Creating a catkin Package--------------
cd ~/catkin_ws/src
catkin_create_pkg <package_name> [depend1] [depend2] [depend3]
catkin_make
source devel/setup.zsh
------------------------------------------------------------------------
Nodes: A node is an executable that uses ROS to
communicate with other nodes.
Messages: ROS data type used when subscribing or publishing to a topic.
Topics: Nodes can publish messages to a topic as well as subscribe to a
topic to receive messages.
Master: Name service for ROS (i.e. helps nodes find each other)
------------------------------------SERVICE---------------------------
rosservice list         print information about active services
rosservice call         call the service with the provided args
rosservice type         print service type
rosservice find         find services by service type
rosservice uri          print service ROSRPC uri
----------------------------------PARAMETER------------------------
rosparam set            set parameter
rosparam get            get parameter
rosparam load           load parameters from file
rosparam dump           dump parameters to file
rosparam delete         delete parameter
rosparam list           list parameter names
