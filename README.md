# tight-binding-lattice-simulation
Python implementation and diagonalization of  tight-binding model on a translationally invariant lattice

This repository contains the Python implementation and numerical simulation for the diagonalization of a simple one-dimensional (1D) tight-binding model. The code simulates a quantum particle hopping on a translationally invariant lattice, calculates its energy dispersion, evaluates the system's Green's functions, and visualizes the analytical vs. numerical error margins.

## Project Overview

In condensed matter physics, the tight-binding model describes the properties of electrons conducting in a crystalline lattice of atoms. This project provides a robust framework to:
* Set up the Hamiltonian matrix for a 1D translationally invariant periodic lattice.
* Perform numerical exact diagonalization to extract energy eigenvalues and eigenvectors.
* Calculate the analytical and numerical Green's functions ($G_{10,10}$ and $G_{20,10}$) to measure error propagation.
* Visualize the real, imaginary, and absolute squared error values.

## Key Features

- **Exact Diagonalization:** Uses optimized NumPy routines to solve the 1D lattice Hamiltonian matrix.
- **Green's Function Calculation:** Computes local and non-local Green's functions to check model consistency and boundary conditions.
- **Error Analysis Integration:** Built-in calculation of mean errors and absolute differences (e.g., Mean Error for $|G_{10,10}|^2$).
- **3D & 2D Data Visualization:** Employs Matplotlib to plot multi-dimensional physics metrics and quantum states.

## Prerequisites

To run this simulation, you need Python 3.x along with the following libraries:

```bash
pip install numpy matplotlib
