# Atomic_Col

## 1. Introduction\n,
"\n",
    "This project studies the thermal model of N-particles system in an isolated square box of length L. Particles are assumed to be spheres of radius R.\n",
    "\n",
    "Each collision is elastic in nature, particles move in a straight line untill a collision.\n",
    "\n",
    "To determine the final velocities after collisions we use these equations:\n",
    "\n",
    "\\begin{aligned}\\mathbf {v} '_{1}&=\\mathbf {v} _{1}-{\\frac {2m_{2}}{m_{1}+m_{2}}}\\ {\\frac {\\langle \\mathbf {v} _{1}-\\mathbf {v} _{2},\\,\\mathbf {x} _{1}-\\mathbf {x} _{2}\\rangle }{\\|\\mathbf {x} _{1}-\\mathbf {x} _{2}\\|^{2}}}\\ (\\mathbf {x} _{1}-\\mathbf {x} _{2}),\\\\\\mathbf {v} '_{2}&=\\mathbf {v} _{2}-{\\frac {2m_{1}}{m_{1}+m_{2}}}\\ {\\frac {\\langle \\mathbf {v} _{2}-\\mathbf {v} _{1},\\,\\mathbf {x} _{2}-\\mathbf {x} _{1}\\rangle }{\\|\\mathbf {x} _{2}-\\mathbf {x} _{1}\\|^{2}}}\\ (\\mathbf {x} _{2}-\\mathbf {x} _{1})\\end{aligned}\n",
    "\n",
    "                                     where the angle brackets indicate dot products\n",
    "                                     \n",
    "                                     \n",
    "This system can also be considered analogous to an ideal gas as there are no intramolecular forces. All collisions are elastic and we will also see the brownian motion of the gas later. "
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## 2. Description of Algorithms\n",
    "\n",
    "1. Simulation takes a list of Particles with intial positions and velocties\n",
    "\n",
    "\n",
    "2. We check that no particle intially overlaps\n",
    "\n",
    "\n",
    "3. Check if each particle collides with the wall or any other particle\n",
    "\n",
    "\n",
    "4. The particle is then advanced in time by dt. Repeat Step 3\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Initialization of the system"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "The velocity distribution of the particles are specified by the temperature, which is proportional to the average kinetic energy of particles: \n",
    "$$ \\dfrac{1}{2}m \\bar v^2 = n kT $$\n",
    "For simplicity, we set nk=1 here. Then the average velocity is calculated by:\n",
    "$$ \\bar v = \\sqrt {\\dfrac{2T}{m}} $$\n",
    "To initialize of multiple partilce system, we do sampling from 2-D Maxwell-Boltzman velocity distribution:\n",
    "$$ f(v_{x},v_{y}) =  \\dfrac{m}{2 \\pi T} exp[{-\\dfrac{m(v_x^2 + v_y^2)}{2T}}] $$\n",
    "The expectation value is zero and the standard deviation $\\sigma$ of both $v_x$ and $v_y$ is $\\sqrt{\\dfrac{T}{m}}$"
   ]
  }
