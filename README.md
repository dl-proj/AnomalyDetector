# AnomalyDetector

## Overview

This project is to detect the anomaly parts in the medical images using CNN and GAN.
The deep learning model is trained with normal and abnormal CT scan images for the first time. 
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

## Installation

- Environment

    Ubuntu 18.04, Python 3.6, 

- Dependency Installation

    ```
        pip3 intall -r requirements.txt
    ```

## Execution

- Please go ahead the directory in this project, and run the following command in terminal.

    ```
        python3 app.py
    ```
