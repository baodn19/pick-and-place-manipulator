## Setting up package
- This can't be run in a conda environment
- Required packages:
```
sudo apt install ros-jazzy-moveit-task-constructor-core
sudo apt install ros-jazzy-controller-manager
sudo apt install ros-jazzy-gripper-controllers
sudo apt install ros-jazzy-ros2-control
sudo apt install ros-jazzy-ros2-controllers
```
- Install dependencies:
``` 
rosdep install --from-paths src --ignore-src -r -y
```
