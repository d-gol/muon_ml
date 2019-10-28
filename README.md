# A simple framework for hyper-parameters optimization

Supports
* Defining hyper-parameters as dictionary
* Creating multiple models using grid search of hyper-parameters 
* Training multiple models
* Evaluating multiple models with predefined metrics
* Perform n-fold cross validation
* Creates folder structure where the results are stored
* Stores
..* Models' .json and .h5 files
''* Training and validation history
''* If selected, prediction results on test set input
''* Information about all trained models
''''* Model's parameters
''''* Loss during training
''''* Validation results
