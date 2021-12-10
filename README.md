# GamePhysicsWithVulkan

This is a very basic renderer that is meant to be used in conjunction with the [Game Physics In One Weekend book series](https://gamephysicsweekend.github.io/).

When you get the project to build and run, you should see a small sphere on top of a large sphere.  This is the hello world of the book series.

![Hello World](https://github.com/gamephysicsweekend/VulkanRenderer/blob/main/data/images/helloworld.jpg?raw=true)

## Dependencies

1. Download and install Vulkan SDK corresponding to your platform from https://vulkan.lunarg.com/sdk/home

2. Download and install CMake from https://cmake.org/download/

## Get started
```
git clone --recursive https://github.com/LongerZrLong/GamePhysicsWithVulkan
```

## Usage

Scene.cpp is where you should begin writing the code from the book series.  And sprinkled throughout the rest of the code will be comments:

```
// TODO: Add code here
```

This is where you would fill in the code snippets from the texts.

## Controls

The controls for the renderer are very basic.

```
Hold left mouse button to rotate the camera around the origin.
Scroll to zoom.
"R" to reset the scene.
"T" to pause and unpause time.
"Y" to step the simulation by a single frame (only works when the simulation is paused).
```