# Atomic_Col

## 1. Introduction\n
This project studies the thermal model of N-particles system in an isolated square box of length L. Particles are assumed to be spheres of radius R.

Each collision is elastic in nature, particles move in a straight line untill a collision.

To determine the final velocities after collisions we use these equations:

$\begin{aligned}\mathbf {v} '_{1}&=\mathbf {v} _{1}-{\frac {2m_{2}}{m_{1}+m_{2}}}\ {\frac {\langle \mathbf {v} _{1}-\mathbf {v} _{2},\,\mathbf {x} _{1}-\mathbf {x} _{2}\rangle }{\|\mathbf {x} _{1}-\mathbf {x} _{2}\|^{2}}}\ (\mathbf {x} _{1}-\mathbf {x} _{2}),\\\mathbf {v} '_{2}&=\mathbf {v} _{2}-{\frac {2m_{1}}{m_{1}+m_{2}}}\ {\frac {\langle \mathbf {v} _{2}-\mathbf {v} _{1},\,\mathbf {x} _{2}-\mathbf {x} _{1}\rangle }{\|\mathbf {x} _{2}-\mathbf {x} _{1}\|^{2}}}\ (\mathbf {x} _{2}-\mathbf {x} _{1})\end{aligned}$

                                     where the angle brackets indicate dot products
                                     
                                     
This system can also be considered analogous to an ideal gas as there are no intramolecular forces. All collisions are elastic and we will also see the brownian motion of the gas later. 
