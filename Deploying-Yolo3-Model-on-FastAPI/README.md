# Ungraded Lab - Deploying a Deep Learning model
 
## Introduction
During this code you will go through the process of deploying an already trained Deep Learning model. To do so, we will take advantage of the user-friendly library fastAPI that provides a nice REST API framework.
 
This tutorial is specifically designed to run locally on your machine. This can be done via 2 methods:  using `Python Virtual Environments` or using `Docker`. 
 
Both approaches should yield the same result. If you already have a conda installation available on your computer, we recommend  that you use the virtual environment method. If this is not the case, choose the Docker method as it is easier to set up.
 
As a general note, the commands in this tutorial are meant to be run within a terminal. To begin you need to **clone this repo in your local filesystem and `cd` to the deployment_tutorial directory**.

To clone the repo use this command:
```bash
git clone https://github.com/youssefHosni/Practical-Machine-Learning.git
```

or for cloning via SSH use:
```bash
git clone git@github.com:youssefHosni/Practical-Machine-Learning.git
```

If you are unsure which method to use for cloning, use the first one.

The `cd` command allows you to change directories. Assuming you are at the directory where you issued the cloning command, type the following on your terminal.
```bash
cd working_directory/deployment_tutorial
```
 
## Method 1: Python Virtual Environment with Conda
 
### Prerequisites: Have [conda](https://docs.conda.io/en/latest/) installed on your local machine.
 
You will use Conda as an environment management system so that all the dependencies you need for this tutorial are stored in an isolated environment.
 
Conda includes a lot of libraries so if you are only installing it to complete this lab , we suggest using [miniconda](https://docs.conda.io/en/latest/miniconda.html), which is a minimal version of conda.
 
### 1. Creating a virtual Environment
 
Now we assume that you either successfully installed conda or that it was previously available in your system. The first step is  creating a new developing environment. Let's set a new environment with python 3.8 with this command:
 
```bash
conda create --name deployment-tutorial python=3.8
```
 
After successfully creating the environment, you need to activate it by issuing this command:
 
```bash
conda activate deployment-tutorial
```
 
At this point, you will do all your libraries installation and work in this environment. 
 
### 2. Installing dependencies using PIP 
 
Now use the following command to install the required dependencies:
 
```bash
pip install -r requirements.txt
```
 
This command can take a while to run depending on the speed of your internet connection. Once this step completes you should be ready to spin up jupyter lab and begin working on the ungraded lab.
 
### 3. Launching Jupyter Lab
 
Jupyter lab was installed during the previous step so you can launch it with this command:
```bash
jupyter lab
```
After execution, you will see some information printed on the terminal. Usually you will need to authenticate to use Jupyter lab. For this, copy the token that appears on your terminal, head over to [http://localhost:8888/](http://localhost:8888/) and paste it there. Your terminal's output should look very similar to the next image, in which the token has been highlighted for reference:


![token](https://user-images.githubusercontent.com/72076328/219001245-ad9cc6d9-aaf7-4495-a08a-4eb92711c35d.png)


### 4. Running the notebook
 
Within Jupyter lab you should be in the same directory where you used the `jupyter lab` command.
 
Look for the `server.ipynb` file and open it to begin to run it.

To stop jupyter lab once you are done with the lab just press `Ctrl + C` twice.
 
### And... that's it! Have fun deploying a Deep Learning model! :)
