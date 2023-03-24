# Double Pendulum Simulation

A Python script that simulates the motion of a double pendulum using physics.

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)

## Overview

This script allows you to visualize the complex motion of a double pendulum system. By defining the initial conditions of the system, the script calculates and plots the motion of the pendulum.

![Recorded GIF](https://github.com/PolybitRockzz/double-pendulum/blob/main/demo.gif)

## Installation

To run this script, you need to have Python 3 installed. You can download Python 3 from the official website: https://www.python.org/downloads/

You also need to install the following packages:
- Matplotlib
- Scipy

You can install these packages using pip:

```
pip install matplotlib scipy
```

Finally, run the `double_pendulum.py` script.

## Usage

The simulation starts with a double pendulum in a static position. The first mass is held in place while the second mass is released. The simulation then shows how the double pendulum moves over time based on the laws of physics.

## Explanation

The `double_pendulum.py` script contains the `Pendulum` and `Animator` classes. The `Pendulum` class contains methods for calculating the position and movement of the double pendulum using polar coordinates. The `Animator` class contains methods for animating the movement of the double pendulum on a 2D plane.

Check out this website for reading the physics explanation for the double pendulum:
https://physicspython.wordpress.com/2019/02/11/double-pendulum-pt-1/

## Example

Here is an example of how to use the script:

```
import scipy as sp
from double_pendulum import Pendulum, Animator

pendulum = Pendulum(theta1=sp.pi, theta2=sp.pi - 0.01, dt=0.01)
animator = Animator(pendulum=pendulum, draw_trace=True)
animator.animate()
```

This will create a double pendulum with initial angles of `π` and `π-0.01` radians and a time step of `0.01` seconds. The animation will include the trace of the second mass.

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/PolybitRockzz/double-pendulum/blob/main/LICENSE) file for details.