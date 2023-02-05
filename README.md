## 1.	Overview of the analysis:
This analysis created a binary classifier to predict whether applicants would be successful if funded by Alphabet Soup. 

In this analysis, I created a Neural Network Model, compiled trained and evaluated the data, and developed an initial analysis of the results. In an effort to improve the overall accuracy, I attempted to optimize the model. Results are described below. 

## 2.	Results: 
o	Data Preprocessing
The IS_SUCCESSFUL column was identified as the target variable
The features included the following columns:
1.	Application Type
2.	Affiliation
3.	Classification
4.	Use Case
5.	Organization
6.	Status
7.	Income Amt
8.	Special Considerations
9.	Ask Amt
	The EIN and NAME columns were not considered to be targets or features and were therefore removed from the model.

o	Compiling, Training, and Evaluating the Model
Using the Relu feature for the hidden layers and Sigmoid for the output, the model initially included 2 hidden layers at 8 and 5 neurons respectively. The numbers were kept low in an effort to avoid overfitting the model.

For the initial analysis, the model produced a 73% accuracy level with a loss of about 55%

To optimize the model and attempt to increase overall accuracy, the following was performed as found in the optimization file:
1.	Removed additional categories from the data table to help reduce potential confusion. Variables removed include EIN, Name, Use Case, Organization, Status, and Special Considerations
2.	Increased the number of bins to <700 for application type and <2,500 for application class counts
3.	Increased the neurons in the hidden layers to 10 and 8, respectively

The results of the optimization were similar to the original analysis at 72% accuracy with 56% loss, meaning the optimization process was unsuccessful in achieving greater accuracy. 

## 3.	Summary: 
Overall the model was similar in both use cases with less than 75% accuracy in predicting success. While high, there may still be an additional need to improve the model to achieve greater accuracy. Perhaps additional optimization techniques such as more hidden layers or a different supervised model approach could be applied to see if greater accuracy can be achieved. 
