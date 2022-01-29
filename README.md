# obstacles

Modular URDF primitives for generating customizable obstacle courses

![stairs](https://user-images.githubusercontent.com/59701038/151646314-924e6191-f6c6-4284-abcb-8eca5f8e1f5d.png)

## Usage

- See the `urdf/examples` folder for a demo of how to assemble an obstacle using primitives
- Primitives (eg. staircases) are defined as self-contained macros that can be called in another file
- To call a macro, first include its filename, and then use `<xacro:macro_name_here ... />` tag
- Obstacle courses can be defined outside of this package, since `<xacro:include .../>` can find any package that has been built in the current workspace
- The easilest way to visualize obstacles is using the URDF preview tool from the ROS VSCode extension, otherwise a launch file with rviz also works
