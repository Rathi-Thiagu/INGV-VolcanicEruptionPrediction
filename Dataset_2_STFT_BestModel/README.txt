Dataset 2 ( Short Time Fourier Transform (STFT) for feature Extraction)
Import the training and test data from the below link
		https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe/data
Step1: Give the path for train.csv , sample_submission.csv in the INGV-Dataset_STFT_Pickle.ipynb
Step2: Upon running this files the following pickle files will be created
			X_train_T2.pickle
			y_train_T2.pickle
			X_test_T2.pickle
Step3: Now you can try running the models on Dataset 2 by importing the pickle files

STFT Source Code Reference : 
https://www.kaggle.com/amanooo/ingv-volcanic-basic-solution-stft

We have taken only the feature extraction using stft part from the above source. 

Ensemble Reference: 
https://machinelearningmastery.com/model-averaging-ensemble-for-deep-learning-neural-networks/

We referred the above source for implementing ensemble technique.