## Installing dependencies from source
1. Navigate to `src` in your workspace
2. Clone the packages below
- MoveIt 2:
```
git clone https://github.com/moveit/moveit2.git -b main
vcs import < moveit2/moveit2.repos
```
- MoveIt Task Constructor:
```
git clone https://github.com/moveit/moveit_task_constructor.git -b ros2
```
- Warehouse ROS Mongo:
```
git clone https://github.com/moveit/warehouse_ros.git -b ros2
git clone https://github.com/moveit/warehouse_ros_mongo.git -b ros2
```
3. Install Dependencies
```
cd ~/moveit2_ws
rosdep install -r -y --from-paths src --ignore-src --rosdistro $ROS_DISTRO
```
4. Build the Workspace
- If you have limited RAM, run:
```
export MAKEFLAGS="-j2"
colcon build --executor sequential
```
