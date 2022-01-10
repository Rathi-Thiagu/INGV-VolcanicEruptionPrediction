Dataset 3 (Raw sensor data)
Step 1: Import the training and test data from the below link(Except for Google Cloud files)
		https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe/data

Step 2: Training the algorithms on this dataset needs TPU instance. Create an account in Google Cloud platform(or any other services). 
        Its a free account and first time users will get a credit which will be sufficient to train models on this dataset.  

IGNV_MLP_Raw1.ipynb 
This file creates the training and test datasets by loading the complete sensor data.The file can be run locally (CPU) by setting 
the couter value in create_training_dataset function to 2000 (considers only 2000 datapoints for training)
If hardware optimization is done using a TPU then counter can be set to 4431(entire dataset).
The same follows for create_testing_dataset function.

VolcanoCNN_GoogleCloud.ipynb
This file can be run only using TPU. After every cell execution, the memory of the variables in the previous cell need to be released manually to avoid OOM.
We were able to successfully train the algorithm but got OOM exception while making predictions with the testing data.

VolcanoRNN_GoogleCloud.ipynb
This file can be run only using TPU. After every cell execution, the memory of the variables in the previous cell need to be released manually to avoid OOM.There was not enough memory to train the dataset even after discarding previously used variables.

Gen&Iter_TrainTest_CNN.ipynb 
This file can be run locally for the dataset generation. However we were able to train for only 5 epochs. 