In this Repository, I had done a Project on Machine Learning classification problem statement. 

**Project Overview:**

Using Pandas library I loaded the dataset.

I am following Machine Learning pipeline for developing this project:

  •	Collect the data
  
  •	Split the data
  
  •	Check the data information
  
  •	Applying all the training operations on test data
  
  •	Handle Missing values/Null Values (if There are any)
  
  •	Checking and handling duplicate columns (if there are any)
  
  •	EDA Part [Exploratory Data Analysis]
  
  •	Separating categorical and numerical feature of the dataset
  
  •	Numerical Dataset: o Checking Normal Distribution o Checking Outliers and Handling them o Transformation Techniques
  
  •	Handle Categorical data
  
  •	Merging numerical and categorical features
  
  •	Applying scaling
  
  •	Selecting best features for both numerical and categorical data
  
  •	Model development
  
  •	check validation
  
  •	Evaluate model
  
  •	check AUC and ROC For selecting Best Model
  
  •	Save the model
  
  •	Read the Model and check once again

**Split the data:**

Splitting the data at this stage to prevent the data leakage. As if we split the data after feature engineering, the Standard Deviation (std) and variance will be changed.
Applying all the training operations on test data

**Check the data information:**

Checking the data info i.e. data type info, shape, missing values, categorical and numerical features, duplicate features etc. In this dataset I found one duplicated feature, hence, I have removed the duplicated feature from train data and applied the same to test data as well.

**Checking and handling duplicate columns (if there are any):**

There is a duplicate feature named as MonthlyIncome. Checked the data and removed it from train as well as test data.

**Handle Missing values/Null Values (if There are any):**

After checking the null values, I found MonthlyIncome and NumberOfDependents features have a good amount of missing values including all the features have 2 missing values. Upon checking the row for those missing values, I found that these two values are in the same row of each feature. Hence, I removed those two rows using pandas drop method. To handle the missing values in MonthlyIncome and NumberOfDependents features, I had compared the normal distribution by filling the missing values by mean, median, mode and random sampling. Since, random sampling method gave the best matching distribution, hence, I had used this and applied this to test data as well.

**Separating categorical and numerical feature of the dataset:**

**Numerical Dataset:**

    o Checking Normal Distribution
    
    o Checking Outliers and Handling them
    
    o Transformation Techniques

**Handle Categorical data:**

I had used LabelEncoder, OneHotEncoder and OrdinalEncoder to handle the categorical data.

**Merging numerical and categorical features:**

After converting the categorical data, I've added it to the numerical data and formed it to complete training and test data.

Applying scaling

Selecting best features for both numerical and categorical data

**Data Balancing:**

Since the data is not balanced, I had used upsampling to balance it.

**Model development:**

To develop the model, I had used below algorithms

      KNN
      
      Logistic
      
      Naive Bayes
      
      Decision Tree
      
      Random Forest
      
      AdaBoost
      
      Gradient Boosting

**After training the model, I got below results:**

      KNN Accuracy: 0.9327378174788348
      
      Logistic Accuracy: 0.9354709686020932
    
      Naive Bayes Accuracy: 0.9269382041197254
    
      Decision Tree Accuracy: 0.9150723285114326
    
      Random Forest Accuracy: 0.9503366442237184
    
      AdaBoost Accuracy: 0.9356042930471302
    
      Gradient Boosting Accuracy: 0.944670355309646

**Evaluate model:**

Since almmost all models have the result in pretty same range. Therefore, to select the best model, I am using AUC & ROC concept to find the FPR and TPR using Grapical represntation and selecting the best model which is Gradient Boosting.

At last I had saved the model and testedd it by giving a random data.

**🛠 Skills**

    1.Python 
    
    2.Machine learning 
    
    3.Statistics
    
    4.Mathematics
    
    5.Numpy 
    
    6.Pandas
    
    7.Matplotlib
    
    8. Seaborn
