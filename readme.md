# Agnostic model loader

[![Build Status](https://travis-ci.org/isaacmg/model_agnostic_prediction.svg?branch=master)](https://travis-ci.org/isaacmg/model_agnostic_prediction)

This provides any easy model instantiation for Flask, Django, and other production Python projects.
It allows you to easily load models and perform predictions without having to worry about the different types.

## Usage 
To use create a new class that extends your model's backend subclass. You will have to implement `preprocessing` and possibly `create_model` and `process_result` depending on your model (see examples for more info).  

## Project Goals
* Allow users to pre-load model weights from any framework with any save configuration

* Works with common frameworks.

* Same high level functions regardless of backend framework (i.e. preprocess, predict, process_response)

* Provide a standard template which users can extend for their model's specific functionality.

# Examples 

* [CheXNet Keras Deployment on Heroku using model agnostic loader](https://github.com/isaacmg/example_keras_heroku)

* [ResNet50 Example](https://github.com/isaacmg/model_agnostic_prediction/blob/143af897897e675b5cfaff60b6d5212963f8cff8/examples2/example_keras.py#L28)





