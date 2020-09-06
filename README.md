# Self-Driving-Car-Simulator
Course Project to learn and understand Computer Vision

# How_to_simulate_a_self_driving_car
This is the code for "How to Simulate a Self-Driving Car" 

# This code is a work in progress.

## Overview
We're going to use Udacity's [self driving car simulator](https://github.com/udacity/self-driving-car-sim) as a testbed for training an autonomous car. 

## Dependencies

We can install all dependencies by running one of the following commands

We need a [anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html) to use the environment setting.

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```

Or you can manually install the required libraries (see the contents of the environemnt*.yml files) using pip.


## Usage


### Run the model
We are going to use a Simulated Environment created by Udacity on Unity to save time and efforts and focus on the code.
 Link:-(https://github.com/udacity/self-driving-car-sim)

Start up [the Udacity self-driving simulator], choose a scene and press the Autonomous Mode button.  
Then, run the model as follows:

```python
python drive.py model.h5
```

### To train the model

We'll need the data folder which contains the training images.

```python
python model.py
```

This will generate a file `model-<epoch>.h5` whenever the performance in the epoch is better than the previous best.  For example, the first epoch will generate a file called `model-000.h5`.

Feel free to add on.

Regards
