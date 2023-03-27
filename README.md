# NORLab Robot Descriptions

> Bundled installation and deployment of all robot descriptions for standalone applications

## Installation

```sh
git clone --recurse-submodules git@github.com:norlab-ulaval/norlab-robot-descriptions.git
```

```sh
git clone --recurse-submodules https://github.com/norlab-ulaval/norlab-robot-descriptions.git
```

## Usage

You can install this repo as a ROS2 package or as a standalone repo.
You don't need to create and build in a workspace to use it as a standalone repository.

### ROS2 package

```sh
# Create a workspace and clone
mkdir -p ~/description_ws/src
cd ~/description_ws/src
git clone --recurse-submodules https://github.com/norlab-ulaval/norlab-robot-descriptions.git
cd ..

# Build the descriptions packages
colcon build --packages-up-to backpack_description husky_description marmotte_description warthog_description

# Source and run description launch
ros2 launch <robot>_description description_launch.py
```

### Standalone application

```sh
# Clone
git clone --recurse-submodules https://github.com/norlab-ulaval/norlab-robot-descriptions.git
```
