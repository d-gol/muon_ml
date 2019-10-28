# A simple framework for hyper-parameters optimization

Supports
* Defining hyper-parameters as dictionary
* Creating multiple models using grid search of hyper-parameters 
* Training multiple models
* Evaluating multiple models with predefined metrics
* Perform n-fold cross validation
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
* Stores
 * Models' .json and .h5 files
 * Training and validation history
 * If selected, prediction results on test set input
 * Information about all trained models
 * Model's parameters
 * Loss during training
 * Validation results
