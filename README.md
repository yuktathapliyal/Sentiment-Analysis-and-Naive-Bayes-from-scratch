# Sentiment-Analysis-and-Naive-Bayes-from-scratch

*****STEPS TO RUN THE CODE*********

All of the required code blocks are included in the notebook and are generally sorted in a way to be run 
sequentially. This readme explains the flow of the code in the notebook:

A. Bernoulli NB implementation from scratch [Naive_Bayes_from_scratch.ipynb]
	* Mount google drive [Cell 2]
		- For this Notebook, the test.csv and train.csv files should be placed in "Colab Notebooks/Project 2" directory in Google Drive, or update the path in Cell 5 to your desired path.
    
	* Import necessary libraries [Cell 1, 4]
	1. Run user-defined method: text_process() [Cell 3] 
	2. Import data and split into xtrain,ytrain,xtest,ytest [Cell 5]
	3. Perform vectorization on the data using CountVecotrizer() by setting text_process() as the tokenizer and limiting the max_features to 1000 [Cell 6]
	4. Calculate probabilities for each class (k) and for each feature (j) for every class (k) [Cell 7, 8]
	5. Make predictions for test samples [Cell 9]
	6. Run K-Fold Cross Validation [Cell 10]


B. Testing Various Classifiers for Kaggle Competition: [Kaggle_models.ipynb]

	* Import necessary libraries [Cell 1]
	* Upload the train.csv and test.csv files and run definition of get_wordnet_pos() [Cell 2]
	1. Run Cell 3 to get a comparison of 9 models
	2. Run Cell 4 and 5 for hyperparameter search for Multinomial NB
	3. Run Cell 6 for hyperparameter search for Linear SVC
	4. Run Cell 7 for hyperparameter search for Random Forests
	5. Cell 8, 9 and 10 should be run to get insight of 3 tested stacking classifiers
