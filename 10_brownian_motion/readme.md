**Exercise 10.3 Brownian Motion**

Brownian motion is the motion of a particle, such as a smoke or dust particle, in a gas,
as it is buffeted by random collisions with gas molecules. Make a simple computer
simulation of such a particle in two dimensions as follows. The particle is confined to
a square grid or lattice L x L squares on a side, so that its position can be represented
by two integers i, j = 0 ... L - 1. It starts in the middle of the grid. On each step of
the simulation, choose a random direction-up, down, left, or right-and move the
particle one step in that direction. This process is called a random walk. The particle is
not allowed to move outside the limits of the lattice-if it tries to do so, choose a new
random direction to move in.  

Write a program to perform a million steps of this process on a lattice with L = 101
and make an animation on the screen of the position of the particle. (We choose an odd
length for the side of the square so that there is one lattice site exactly in the center.)  

Note: The visual package doesn't always work well with the random package, but
if you import functions from visual first, then from random, you should avoid prob-
lems.

**Modifications:**
- Have your code keep track of the number of times the particle hits the wall during
the random walk, and print the result.
- Instead of making a simulation of the random walk through the lattice, you should
make four plots of the path of the random walk: (1) after $10^3$ steps, (2) after $10^4$
steps, (3) after $10^5$ steps.
