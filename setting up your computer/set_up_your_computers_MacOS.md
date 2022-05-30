# Conda install instructions for MacOS

Below are set of instructions to help you effectively participate 
in this camp: Provided is an introduction to computation and simulations.

- [Download this repository](#download-this-repository)
- [How to open your terminal](#how-to-open-your-terminal)
- [Set up your Anaconda environment](#set-up-your-anaconda-environment)
- [Access an assignment or class in Jupyter](#access-an-assignment-or-class-in-jupyter)
<br />
<br />
<br />


## How to open your terminal

#### MacOS
You can open the terminal application on MacOS by either:
1. Use Spotlight search: press “Command + Space” and search for “terminal”
2. Open Launchpad and look for the “Terminal” app


## Download this repository

This repository contains software and files neccessary for activities in this class, so we ask you to download this repository and put it in a location convienient for later reference. We recommend you put it in your home directory using the commands below:  
```bash
$ cd $HOME
$ mkdir cybercamp2022
$ cd cybercamp2022
$ git clone https://github.com/PTC-CMC/cybercamp.git
$ ls cybercamp
```
<br />
<br />
<br />

## Set up your Anaconda environment

Anaconda is a free, open-source distribution of the Python and R programming language for scientific computing, that aims to simplify package management and deployment. In this class, we will use Anaconda to manage our Python environment. Below are short instructions to set up the Anaconda software for Mac.

#### MacOS  
1. Download miniconda from:   
    https://docs.conda.io/en/latest/miniconda.html   
    (Select the correct installer for **Python 3.8, 64-bit pkg**)
2. Install miniconda from the downloaded file  
3. If you followed the above [instruction](#Download-this-repository) and put this repository at your home directory, you can change into that folder by running
`cd ~/cybercamp2022/cybercamp`
4. Create and activate a new conda environment by typing in the terminal window:
    `conda env create -f environment.yml`  
    If prompted you may need to update your conda environment and rerun the above commands.
5. When the command has successfully executed then type:  
    `conda activate cybercamp38`   
**Note:** You will need this command whenever starting up a new terminal to access the class materias


## Access an assignment or class in Jupyter

1. Type `jupyter notebook` into your terminal
2. The jupyter notebook will be open as one tab in your default browser  
If this doesn't occur automatically, look a the output from your jupyter notebook command. You should see a web link that looks something like `http://localhost:8888/?token=fd014533bc5780c313dfd1803838a89c6a90cdcd75d0cb2b` Copy that link by highlighting it and using command-c. Then, paste the link into the web browser of your choice. We recommend Google Chrome.
3. Click on folders to navigate through them, or on files to open them. Text files will open with a built in text editor. Jupyter notebook files have the extension `.ipynb`. These are the files where you execute python code, and where we'll run our assignments from.



