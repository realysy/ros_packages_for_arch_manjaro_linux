## About this repository

Here provides ros packages for Arch Linux or Manjaro Linux, so that you don't have to build from source yourself.

This is not an official repository by [ROS](https://www.ros.org). 

I've got through the head-scratching experience, so I put my final package here hoping it being helpful. If your have another ROS version built done, welcome to PR.


## About ros package version

* `ros2-humble-2022.11.23-1-any.pkg.tar.zst`: built from [aur/ros2-humble](https://aur.archlinux.org/packages/ros2-humble) (corresponding Github rep: [m2-farzan/ros2-humble-PKGBUILD](https://github.com/m2-farzan/ros2-humble-PKGBUILD)), if your want to build yourself, try `yay -Sy ros2-humble`. Thanks for the work from @m2-farzan.


## How to install the package

Take `ros2-humble-2022.11.23-1-any.pkg.tar.zst` for example, if you want to install in Arch Linux or Manjaro Linux (I'm using Manjaro), try:

```bash
# 1. install dependencies (you can try to install the package directly, it will tell you what are missed)
sudo pacman -Sy base-devel
yay -Sy ros2-arch-deps
yay -Sy ros2-pyqt5-sip-compat
yay -Sy sip4

# 2. install the package
sudo pacman -U ros2-humble-2022.11.23-1-any.pkg.tar.zst

# 3. no error should happen above!

# 4. enjoy
source /opt/ros/humble/setup.bash   # if you are using bash
source /opt/ros/humble/setup.zsh    # if you are using zsh
ros2 -h

```


## ROS tutorials

* [ROS2/humble/Tutorials](https://docs.ros.org/en/humble/Tutorials.html)



