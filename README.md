# [Coursera's Introduction to Machine Learning by Andrew Ng](https://www.coursera.org/learn/machine-learning) 
# Python Programming Assignments

![](machinelearning.jpg)

This repositry contains the solutions to the python versions of the programming assignments for the [Machine Learning online class](https://www.coursera.org/learn/machine-learning) taught by Professor Andrew Ng. This is perhaps the most popular introductory online machine learning class. In addition to being popular, it is also one of the best Machine learning classes any interested student can take to get started with machine learning. An unfortunate aspect of this class is that the programming assignments are in MATLAB or OCTAVE, probably because this class was made before python become the go-to language in machine learning. The Python machine learning ecosystem has grown exponentially in the past few years, and still gaining momentum. 

These assignments work seamlessly with the class and do not require any of the materials published in the MATLAB assignments. The assignments use [Jupyter Notebook](http://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/what_is_jupyter.html), which provides an intuitive flow easier than the original MATLAB/OCTAVE assignments.

## Downloading the Assignments

To get started, you can start by either downloading a zip file of these assignments by clicking on the `Clone or download` button. If you have `git` installed on your system, you can clone this repository using : 

    clone https://github.com/vrn25/Coursera_ML/.git
    
Each assignment is contained in a separate folder. For example, assignment 1 is contained within the folder `Exercise1`. Each folder contains two files: 
 - The assignment `jupyter` notebook, which has a `.ipynb` extension. All the solutions are included in it.
 - A python module `utils.py` which contains some helper functions needed for the assignment. Functions within the `utils` module are called from the python notebook. No separate modification is required
 
## Requirements 

These assignments has been tested and developed using the following libraries: 

    - python==3.6.4
    - numpy==1.13.3
    - scipy==1.0.0
    - matplotlib==2.1.2
    - jupyter==1.0.0
    - jupyter-client==5.0.1
    
I recommend using at least these versions of the required libraries or later. Python 2 is not supported. 
    
## Python Installation

It is highly recommended to use anaconda for installing python. [Click here](https://www.anaconda.com/download/) to go to Anaconda's download page. Make sure to download Python 3.6 version.
If you are on a windows machine:
 - Open the executable after download is complete and follow instructions.
 - Once installation is complete, open `Anaconda prompt` from the start menu. This will open a terminal with python enabled.
 
 If you are on a linux machine: 
 
 - Open a terminal and navigate to the directory where Anaconda was downloaded. 
 - Change the permission to the downloaded file so that it can be executed. So if the downloaded file name is `Anaconda3-5.1.0-Linux-x86_64.sh`, then use the following command:
 
      `chmod a+x Anaconda3-5.1.0-Linux-x86_64.sh`
 
 - Now, run the installation script using `./Anaconda3-5.1.0-Linux-x86_64.sh`, and follow installation instructions in the terminal.
 
 
Once you have installed python, create a new python environment will all the requirements using the following command: 

    conda create -n machine_learning python=3.6 scipy=1 numpy=1.13 matplotlib=2.1 jupyter
 
After the new environment is setup, activate it using (windows)

    activate machine_learning
   
or if you are on a linux machine

    source activate machine_learning 

Now we have our python environment all set up. The notebook can be launched from the terminal by the following command

    jupyter notebook

This should automatically open a tab in the default browser. To start with assignment 1, open the notebook `./Exercise1/exercise1.ipynb`. 

## Python Tutorials

If you are new to python and to `jupyter` notebooks, no worries! There is a plethora of tutorials and documentation to get you started. Here are a few links which might be of help:

- [Python Programming](https://pythonprogramming.net/introduction-to-python-programming/): A turorial with videos about the basics of python. 

- [Numpy and matplotlib tutorial](http://cs231n.github.io/python-numpy-tutorial/): We will be using numpy extensively for matrix and vector operations. This is great tutorial to get you started with using numpy and matplotlib for plotting.

- [Jupyter notebook](https://medium.com/codingthesmartway-com-blog/getting-started-with-jupyter-notebook-for-python-4e7082bd5d46): Getting started with the jupyter notebook. 

- [Python introduction based on the class's MATLAB tutorial](https://github.com/mstampfer/Coursera-Stanford-ML-Python/blob/master/Coursera%20Stanford%20ML%20Python%20wiki.ipynb): This is the equivalent of class's MATLAB tutorial, in python.


## Caveats and tips

- In many of the exercises, the regularization parameter $\lambda$ is denoted as the variable name `lambda_`, notice the underscore at the end of the name. This is because `lambda` is a reserved python keyword, and should never be used as a variable name.

-  In `numpy`, the function `dot` is used to perform matrix multiplication. The operation '*' only does element-by-element multiplication (unlike MATLAB). If you are using python version 3.5+, the operator '@' is the new matrix multiplication, and it is equivalent to the `dot` function. 
