# Income-Machine-Learning-Model
For this project, I utilized census data from UC Irvine (Citation: Becker, B. & Kohavi, R. (1996). Adult [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5XW20.). Collected in 1994, this dataset contains information related to employment and income. I selected this dataset to investigate whether, based on its multiple features, I could predict if an individual earns more or less than $50,000 per year.

The raw dataset consisted of 15 columns, with varying data types, and 48,842 rows. Some of these rows were duplicated, and some rows contained missing values. This was the first issue I encountered. I was able to remove duplicate rows, as well as deal with missing values. 

I then had to one hot encode my colums to make it so all the data was the same type for my model. After preprocessing my data and cleaning the dataset, I was left with a total of 108 columns (each categorical column was split into it's own column), and 47,592 rows. 

Approaching my model creation, I initally selected a Logistic Regression Model to predict whether an individual earns more of less than $50,000 per year. To improve the performance of my model and specifically address the risk of overfitting, I implemented regularization techniques and employed cross-validation during the training process. These steps helped ensure that my model generalized well to unseen data instead of simply memorizing the training samples. 


Throughout this notebook, I explored a unique and extremely useful dataset of census data from 1994. I was able to identify problems with the data, such as missing values, duplicate rows, and improper formatting in our target variable values. I corrected these, and built two powerful Machine Learning Models to help me predict if a person makes over $50,000/yr by only using the data that we have avaliable in the census data. My models performed with moderately high accuracy, and did not overfit on the data.
