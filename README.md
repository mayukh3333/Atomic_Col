# Atomic_Col

## 1. Introduction
This project studies the thermal model of N-particles system in an isolated square box of length L. Particles are assumed to be spheres of radius R.

Each collision is elastic in nature, particles move in a straight line untill a collision.

To determine the final velocities after collisions we use these equations:

![Equations](https://github.com/mayukh3333/Atomic_Col/blob/master/equation.png?raw=true?raw=true "Title")

                                                                         
This system can also be considered analogous to an ideal gas as there are no intramolecular forces. All collisions are elastic and we will also see the brownian motion of the gas later. 

## 2. Description of Algorithms

1. Simulation takes a list of Particles with intial positions and velocties


2. We check that no particle intially overlaps


3. Check if each particle collides with the wall or any other particle


4. The particle is then advanced in time by dt. Repeat Step 3

