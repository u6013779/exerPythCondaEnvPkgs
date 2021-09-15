# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.
  * (2021 update: I recommend managing environments as shown in the new Anaconda introduction video. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial) If you want to try creating the environments using the user interface for Anaconda Navigator instead of the command line shown in the Conda What and Why tutorial, that's fine. But watch the Conda What and Why tutorial to understand some of the differences between Conda environments and other types of virtual environments available in Python.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(they let you create specific environments based on what's needed (web development, data analysis, etc.))|
|What is the default package manager in Python?            |(pip)|
|How do you manage environments and packages in Anaconda?  |(Conda or miniconda|
|`conda list`       |(all of the different and default packages installed)|
|`conda env list`       |(a list of environments available)|
|How do you keep your base environment unchanged?       |(install different environments/packages)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(docs.conda.io)|
|`conda create --name XXXX`       |(creates a new environment)|
|`source activate XXXX`       |(activates the new environment to use)|
|`conda install YYYY`       |(installs a new package in a differnt environment)|
|channels in Conda       |(path or location where conda looks for this package)|
|`conda install -c ZZZZ YYYY`       |(allows you to use a specific channel and acess it)|
|`conda config --show channels`       |(shows the channels/paths available)|
|`conda config --add channels ZZZZ`       |(add channels)|
|conda-forge.org       |(community website that has different packages to install)|
|`source deactivate`       |(brings you back to your base/default channel)|
|`conda config --get channels`       |(you can see that all the channels are actually still there, and organized by priority  |

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
# packages in environment at /opt/anaconda3/envs/ai38:
#
# Name                    Version                   Build  Channel
ca-certificates           2021.7.5             hecd8cb5_1  
certifi                   2021.5.30        py38hecd8cb5_0  
libcxx                    12.0.0               h2f01273_0  
libffi                    3.3                  hb1e8313_2  
ncurses                   6.2                  h0a44026_1  
openssl                   1.1.1l               h9ed2024_0  
pip                       21.0.1           py38hecd8cb5_0  
python                    3.8.8                h88f2d9e_5  
readline                  8.1                  h9ed2024_0  
setuptools                52.0.0           py38hecd8cb5_0  
sqlite                    3.36.0               hce871da_0  
tk                        8.6.10               hb0a8c7a_0  
wheel                     0.37.0             pyhd3eb1b0_1  
xz                        5.2.5                h1de35cc_0  
zlib                      1.2.11               h1de35cc_3  
(ai38) reinhardts@Gregorys-MacBook-Air ~ % 




```
* What command would you use to remove the environments you created for this exercise from your computer?

```
#Source deactivate

```
## 2021 Update
Python, Anaconda, and many programming languages are constantly evolving. The video Conda What and Why provides a great explanation of why you may want to use virtual environments for your Python projects, and it provides a nice demonstration of how to work in the command line. However, environment management using Anaconda Navigator is more user friently than ever. I personally will be using Anaconda Navigator to manage environments and packages since it seems easier to see what is going on using the GUI. If you haven't done so already watch the introduction to Anaconda video and pay close attention to the section on using Anaconda Navigator to create environments and install packages. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial


