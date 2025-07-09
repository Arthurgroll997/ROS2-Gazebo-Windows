# ROS2 + Gazebo for Windows

When researching about Gazebo and ROS, I noticed it was very difficult to get them up
and running without major complications in the Windows operating system. The easiest way I knew required running a VM with Ubuntu, but it got the Gazebo simulator stuck at 5 FPS, which was undoubtedly impossible to use.

However, I discovered it was possible to run Gazebo in Docker, which I thought could make the
process a lot easier. So, based on a Unix Docker configuration for ROS & Gazebo ([here's the link for the Unix project](https://github.com/mateus-mos/Hands-On-Workshop-TurtleBot-3-Simulation-in-Gazebo)), I created my own version for Windows.

Important note: Before trying to run, make sure to have Docker, Docker Compose & XMing installed, otherwise it won't be possible to run the Gazebo simulator. [Here's the link to XMing in SourceForge](https://sourceforge.net/projects/xming/), and you can find the links to Docker and Docker Compose with a simple Google search.

Steps to run:
1. Run the run.bat file

And that's it! As simple as that! You can also run `docker exec -it <container_name> (the container name in this case would be ros2_humble_gazebo_harmonic)` and then `ign gazebo` to run the simulator.

## Author: Arthur Von Groll dos Santos
