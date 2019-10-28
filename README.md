# muon_ml

A simple framework for hyper-parameters optimization of deep learning models.
The idea is to provide a model architecture using Keras and a dictionary of parameters.
Then multiple models are created using grid search.
Models can be trained, evaluated, and in the end a user should be able to select the best hyper-parameters by focusing on chosen metrics.

## Features
* Defining hyper-parameters as dictionary
* Creating multiple models using grid search of hyper-parameters 
* Training multiple models
* Evaluating multiple models with predefined metrics
* Perform n-fold cross validation
* Storing
  * Models' .json and .h5 files
  * Training and validation history
  * If selected, prediction results on test set input
  * Information about all trained models
  * Model's parameters
  * Loss during training
  * Validation results
* Creating a folder structure where the results are stored
  * experiment_name
    * CV_0
      * results_overview.csv
      * model_0
        * model_0.h5
        * model_0.json
        * model_0_history.json
        * model_0_evaluation.csv
        * model_0_predictions.csv
        * [model_0_predictions_scaled.csv]
      * model_1
        * ...
      * ...


## Example
Provided example is a convolutional neural network targeted for particle detection in a 3D CERN detector (HGCAL). The goal is to find a sufficiently small CNN to be able to run on an FPGA with low-latency (orders of micro seconds). This framework is used to automatically select parameters for optimization and find the best model. 


## To be improved

* A rather rigid structure, every time a model needs to be defined within the code, should be more user-friendly
* Provide support for training on multiple GPU's
* Divide one GPU to support multiple models training if possible
