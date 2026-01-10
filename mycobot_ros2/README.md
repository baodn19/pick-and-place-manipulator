## Setting up package
- This can't be run in a conda environment
- Version: ROS 2 Jazzy
- Required packages:
```
sudo apt install ros-jazzy-moveit-task-constructor-core
sudo apt install ros-jazzy-controller-manager
sudo apt install ros-jazzy-gripper-controllers
sudo apt install ros-jazzy-ros2-control
sudo apt install ros-jazzy-ros2-controllers
sudo apt install ros-jazzy-moveit-visual-tools
sudo apt install ros-jazzy-moveit-task-constructor-visualization
sudo apt install ros-jazzy-gz-ros2-control
sudo apt install ros-jazzy-moveit-task-constructor-capabilities
```
- Install dependencies:
``` 
rosdep install --from-paths src --ignore-src -r -y
```
