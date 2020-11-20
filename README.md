# AnomalyDetector

## Overview

This project is to detect the anomaly action in the recorded video using CNN and GAN.
The deep learning model is trained with normal and abnormal videos for the first time. 
Then the fpr and tpr values according to all the threshold values are obtained while running projects with normal(positive) and
abnormal (negative) then the ROC curve is plotted. Then the optimum threshold value can be obtained.

## Structure

- src
    
    The source code to create the model and estimate its fpr/tpr with the model.

- utils

    * The weights and model for this project
    * The source code to manage the folder and files in the project

- app

    The main execution file
    
- requirements
    
    * All the dependencies for this project
    * When using GPU with CUDA 9.0, the version of some dependencies are as following:
    ```
        tensorflow-gpu==1.12.0
        keras==0.23.2
        matplotlib==2.0.0
        pandas==0.9
        numpy==1.18.1
    ``` 

- settings

    * The  path and name of several directories
    * The  path and name of the model and weights for this project 
    * The path and name of result files(csv, png)
    * The value of max gan loss and min gan loss, and the base value necessary for finding optimum threshold value

## Installation

- Environment

    Ubuntu 18.04, Python 3.6, 

- Dependency Installation

    ```
        pip3 intall -r requirements.txt
    ```
  
    * Note: if using GPU, please refer the requirements section in Structure.

## Execution

- Please go ahead the directory in this project, and run the following command in terminal.

    ```
        python3 app.py
    ```
