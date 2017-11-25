# Self Driven Future
My_self_driving_car_project

Author: Rishab Sharma (rishab-sharma)

## Overview

This is the code for my project where I used Udacity's [self driving car simulator](https://github.com/udacity/self-driving-car-sim) as a testbed for training an autonomous car. 

## Demo Video

[![Self Driving car](https://img.youtube.com/vi/YJBRLkoVijE/0.jpg)](https://www.youtube.com/watch?v=YJBRLkoVijE&t=9s)

## Dependencies

You can install all dependencies by running one of the following commands

You need a [anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html) to use the environment setting.

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```

Or you can manually install the required libraries (see the contents of the environemnt*.yml files) using pip.


## Usage


### Run the pretrained model

Start up [the Udacity self-driving simulator](https://github.com/udacity/self-driving-car-sim), choose a scene and press the Autonomous Mode button.  Then, run the model as follows:

```python
python drive.py model.h5
```

### To train the model

You'll need the data folder which contains the training images.

```python
python model.py
```

This will generate a file `model-<epoch>.h5` whenever the performance in the epoch is better than the previous best.  For example, the first epoch will generate a file called `model-000.h5`.



