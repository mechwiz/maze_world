# Effect of Planning Depth in Predator-Prey Behavior
**Michael Wiznitzer**

Northwestern University: Final Project

## Introduction
Nature is a wonder of its own. When we look at animals, we usually see cute furry creatures that seemingly just do their own thing. After seeing them in the wild, though, you begin to notice how they use their environment to hunt or hide from other animals. For [example], a leapord might hide in a narrow valley as it hunts imapla grazing above it. In order to better understand these predator-prey relationships, [research](https://nxr.northwestern.edu/planning-vertebrates) has been done in the NxR lab to simulate how prey will act (using POMDPs) given various planning depths in order to reach some goal position before a predator kills the prey. My project focuses on turning these simulations into a 3-D honeycomb-styled-world realization where Sphero robots act as the predator and prey that have to navigate in various levels of occluded environments.

####  Objective
The goal of this project is to demonstrate the effect of planning-depth in regards to prey being able to reach some goal position before the predator kills it in a 3-D honeycomb-styled-world environment with various levels of occlusion. This project breaks down into 3 different parts listed below:

- Maze Fabrication
- Sphero Control with ROS
- Image Processing to determine robot location in maze

To read more about each part, see my portfolio post [here](https://mechwiz.github.io/Portfolio/prey.html). This repo's purpose is to highlight all of the differenct modules designed and created for the **Maze Fabrication** part above.

## Maze Fabrication
There are two parts to designing the maze within which the 3-D simulations will occur. The obvious part is designing the full-scale maze which will look something like the picture below based on the specs described in my portfolio post.

<div align="center"> <img src="rough_full_scale_model/imgs/MazeRender1.png" width="700px"/></div>

The full-scale maze will include around 349 hexagonal cells and will be roughly 11ft long by 8.6ft wide by 0.5ft tall. Due to the large size of the maze, it would make sense for the pieces to be modular so that assembly and takedown is relatively straightforward. Furthermore, well designed modular pieces could potentailly lead to being able to construct differently sized mazes to explore even more kinds of predator-prey scenarios.

This leads to the second part of the maze design - building a small-scale version so that testing with the other parts of the project (i.e. controlling the Sphero robots with ROS via Image Processing) can be done. This way, if any modificaitons to the small scale maze needs to be done in the interest of the other parts, they can be incorporated into the full-scale maze design.

### Small Scale Maze Design
The small-scale maze design assembly model and actual laser-cut model are shown side by side below:

<div align="center">
    <img src="small_scale_model/imgs/rendered/small_scale.jpg" width="400px" alt="" /><img hspace="20"/><img src="small_scale_model/imgs/real/small_scale.jpg" width="400px" alt="" />
</div>

The module pieces incorporate are described in the table below.
