# ME597-Fall2024-tb3-gz
## Instructions:
1. Simply save the turtlebot3_gazebo package to a workspace e.g., 
    ```
    cd ~/ros2
    mkdir -p sim_ws/src
    cd sim_ws/src
    git clone https://github.com/naslab-projects/ME597-Fall2024-tb3-gz.git
    ```
    Rename the package to `turtlebot3_gazebo`
    ```
    mv ME597-Fall2024-tb3-gz turtlebot3_gazebo
    ```

2. In a new terminal build the sim_ws workspace: 
    ```
    cd sim_ws
    colcon build --symlink-install
    ```

3. Add turtlebot3 environment variable to .bashrc file
    ```
    echo "export TURTLEBOT3_MODEL=waffle" >> ~/.bashrc
    ```
4. Run these to install useful packages you will use in the simulator.
    ```
    sudo apt install ros-humble-turtlebot3-teleop
    sudo apt install ros-humble-slam-toolbox
    sudo apt install ros-humble-navigation2
    ```
5. Don't forget to source the workspace whenever you use it
    ```
    cd sim_ws
    source install/local_setup.bash
    ```
