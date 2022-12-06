# 314 progress report 2

Team members: Xiaoyan Zheng, Zihan Cao, Hongrui Liu, Eric Liu


## Feature 1: Messy Full Data and Sample Clean Data

  ### Narrative:

As a kaggle competitor, I will expect a messy, incomplete, and inconsistent data set but I would also appreciate some guidance on the direction.

  ### Acceptance criteria:

- Given: I am a kaggle competitor

- When: I first look at a new and messy data set, I may be confused.

- Then: I can perhaps check how the other guys are approaching this data to obtain some hints.

  

- Given: I am a kaggle competitor

- When: I am given policing data with missing entries

 -Then: I should be able to write code that can remove those rows

- Given: I am a kaggle competitor

- When: I am given policing data that is separated into different tables

- Then: I should be able to write code that can concatenate them

  

- Given: I am a kaggle competitor

- When: I am given policing data that is not accurately represented

- Then: I should be able to write code to rename entries to what they should be

  
  
  
  

## Feature 2: Interactive Data Visualization / Dashboard

  

### Narrative:

  

#### Scenario1 - initial data exploration stage:

As a kaggle competitor, I want to graph the relationships between the different factors related to a police stop so that people using the data will have an easy time interpreting it.

  

#### Feature Outline:

The ultimate goal is to explore the relationship between different factors with the reasons for a policy stop. As a result, we will have several interactive graphing functions implemented by Plotly like graphing mean and scatterplot for the participants in the competition to use in order to have a better understanding of the original messy data as well as their cleaned data.

  

### Acceptance criteria:

- Given: I am a kaggle competitor who has cleaned the data

- When: I want to examine the relationship between two features

- Then: I can create different graphs (histogram, scatterplot, etc) to visualize their relationship

  

- Given: I am a kaggle competitor

- When: I have several visual representations of the data

- Then: I will create a dashboard of these visual representations

  

#### Scenario2 - model examination:

As a kaggle competitor, after creating my model, I want to check how good my model is. One example is to compare the y_pred and y_test in a graph.

  

#### Feature Outline:

We plan to create several tool graphing functions to allow the competitors to check their model’s accuracy/ performance.

  

## Feature 3: Database: we would like to use normalization tricks to reduce the size and storage requirement of our dataset, and make the data more accessible.

  

### Narrative:

As a person who is storing and mining the dataset, I want the dataset to take less space in storage and at the same time be easily understandable and accessible, so that when I mine on the dataset (e.g. fit a prediction model), the algorithm can run faster.

  

### Acceptance criteria:

- Given: I have a large dataset with many features and records,

- When: The dataset is not normalized and all features are in the same table,

- Then: I separate some features to other tables and establish relations between tables based on the relationship between those features, thus reducing the size of the dataset in storage.

  
  
  

## Feature 4: A prediction model on the reason and outcome for a police stop based on policy stop records from 2000.1.1 to 2015.12.31 of 6 counties in North Carolina

  

### Narrative:

As a kaggle competition host, we would like the competitors to fit a model that predicts the reason/outcome for a police stop based on the provided data. We will provide 80% of our dataset selected randomly as training data for the competitors, and use the remaining 20% to evaluate their prediction performance, so that we have an accurate and generalizable prediction model.

  
  

### Acceptance criteria:

- Given: A driver is stopped by police in North Carolina

- When: The driver is 30 years old, white, male, etc.

- Then: I should predict the reason/outcome of this stop.

  
  

## Feature 5: Test-driven data analysis

  

### Narrative:

As a kaggle competitor, I want to test whether I have clean data; whether my model has good accuracy, etc. I would first write some test functions, which only pass if my goal is met. Then I will start to implement the actual functions. I would appreciate some test function in advance provided by the host.

  

### Acceptance criteria:

- Given: I have some features that I want to implement on the dataset.

- When: I would like to create a new function that implements the features aforementioned (e.g. cleaning the data)

- Then: I start by writing a test that defines what I would like the function to return under specific conditions, and then write the function that passes the test
