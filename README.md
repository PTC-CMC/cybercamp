# Cybercamp
The cybercamp is rapid overview of molecular simulation and the underlying tools.

## Overview
This repository is designed to provide users the resources to quickly
get up to speed with molecular simulations. This will not only include
information needed to better understand simulations, but it will also
provide specific information for workflow management, "sandboxed" development
environments, python specific scientific packages, etc.  

## Getting Started

### Prerequisites
* [Anaconda](https://www.anaconda.com/download)

	* A python package mangement tool, useful for creating clean, reproducible
development environments

* Command line familiarity

	* Most of the interaction with simulation programs involves some knowledge of
the GNU/Linux, or Unix command line interface.

	* A useful guided tutorial for the command line can be found
[here](https://swcarpentry.github.io/shell-novice/).

* Visualization tools
	*	 Humans are much more adept at visually inspecting data when it
is presented properly. We are not great at reading a large data file 
and developing any meaningful hypotheses/conclusions from a list of 
numbers. We are much better at looking at plot of the data, or 
rendering the trajectory of a molecule evolving in space and time.
	*	 To do this we require molecular visualization tools and data
visualization tools
    * For molecular visualization, a common choice is 
[VMD](http://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=VMD)
    * A common pythonic choice for data visualization is 
[Matplotlib](https://matplotlib.org/) and can easily be installed via anaconda


### Installing
To get a working development environment that uses the `MoSDeF` 
toolkit, `HOOMD-Blue` for simulation, `Matplotlib` for data 
visualization, and `signac` and `signac-flow` for workflow
management, we will use `Anaconda` we installed earlier.

Update `Anaconda` and `conda`

```
conda update conda
```
```
conda update anaconda
```

Add the `mosdef`, `conda-forge`, `glotzer`, `omnia` channels
for `conda` to search through when installing packages.

```
conda config --add channels mosdef
conda config --add channels conda-forge
conda config --add channels glotzer
conda config --add channels omnia
```

Create a new python 3.5 development environment named `simulation35` 
that includes
the packages needed to build systems, run simulations, and
analyze the data.

```
conda create -n simulation35 python=3.5 mbuild foyer hoomd matplotlib signac signac-flow fresnel gsd
```

Activate the environment

```
source activate simulation35
```
## Content

### Computational Basics
The following links provide an overview of the use of the unix/linux shell, Python, and plotting using matplotlib. 
* Introduction to the Unix shell: http://swcarpentry.github.io/shell-novice/
* Introduction to Python:  http://swcarpentry.github.io/python-novice-inflammation/
* Plotting and Programming in Python: http://swcarpentry.github.io/python-novice-gapminder/
* Analysis and plotting Python scripts: https://github.com/PTC-CMC/plotting

### Molecular Modeling and Simulation
* [Introduction to Simulation](intro_to_sim.ipynb)
* [Introduction to Molecular Dynamics](Introduction%20to%20Molecular%20Dynamics.ipynb)
* [Neighborlists and Dangerous Builds](Neighborlists and Dangerous Builds.ipynb)

### Other resources
* Introduction to version control with git: http://swcarpentry.github.io/git-novice/
* Using Jupyter notebooks:
  * http://jupyter.readthedocs.io/en/latest/
  * https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/
  * https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook
* Brief guides on GitHub and git workflows: https://guides.github.com/
* Introduction to version control with git: http://swcarpentry.github.io/git-novice/
* Full list of software carpentry lessons: https://software-carpentry.org/lessons/
* Bevan Lab GROMACS Tutorials: http://www.bevanlab.biochem.vt.edu/Pages/Personal/justin/gmx-tutorials/


## Primary Authors

* **Christopher R. Iacovella**      
* **Justin Gilmer** 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

