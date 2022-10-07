

# 314 progress report 1

*Team member: Xiaoyan Zheng, Zihan Cao, Hongrui Liu, Eric Liu*

## **Problem Domain/Statement**

Our group wants to study correlations between factors like gender, age, etc., and the reason/outcomes of police stops in North Carolina. We found an example paper on "racial disparities in police stops" from the link: https://5harad.com/papers/100M-stops.pdf. Our project's data contains stop records from 2000.1.1 to 2015.12.31 of 6 counties in North Carolina. Our goal of this project is to classify the reason/outcomes of a police stop based on the subject's personal information.

We chose this topic because being stopped on the road is one of the most common situations for people interacting with police. Understanding the reasons for the stops can help drivers drive more safely and police work more efficiently.

Potential problem statement: 

> Predict the reason/outcome of a police stop.

A potential alternative: 

> Is there a relationship between the outcome of a police stop and the subject's gender, age, etc.?



## **Scope**

The course modules we are aiming to cover are Data Cleaning, Data Visualization, Data Normalization, SQL/NoSQL Databases.

1. Data Cleaning+Concatenation: The data we found is messy and difficult to understand and data from different counties can be different. We will need to write scripts to clean them and store the data in a common format. 
2. Database: We need to have a database because our data sets are large and have many columns so it may be faster to query for relevant data. Normalizing our data before putting it into our database will also make comparing data much easier later on. 
3. Data Visualization: We will graph various variables against our target (whether a person gets stopped by the police) in various forms in order to get a more understandable picture of their relationship.

We will have one person cleaning the data, one person normalizing the data, one person constructing the database, and one person making charts and graphs from the data. 



## **Timeline**

[**​**](https://wustl-data.github.io/project/progress_report_1#timeline)We will begin with data cleaning. Since the original police stop datasets of North Carolina are recorded by seven counties respectively, we will start by merging them. Afterward, we want to go through data cleaning processes such as transforming dates, concatenating location information into one column, removing punctuations, etc. 

After finishing the data cleaning, we will conduct the data normalization process. For now, we are thinking of separating subject information and results of the stop into different tables and establishing relations between tables to reduce data redundancy.

After data cleaning and normalization, we will visualize the data to explore what could be our features and targets for the model.

## **Anticipated Roadblocks**

Our first step is to merge the data of seven counties into one data set. There are difficulties in merging seven sets, given the inconsistent data columns recorded by different counties. For instance, only one county records stop locations while the other six do not. 

We are also seeing some potential unreliability of data. The README file indicates that the stop time may not be accurate, while for now, we believe the time when the police stops happened could be a potential factor. We may need to think of a way to mitigate the inaccuracy.

Also, one of the seven data sets from North Carolina is State Patrol data. We are unsure if we should include the State Patrol data set in our project since we are also exploring the police stop factors across different counties in North Carolina. A further examination is needed.



# We will participate in the Kaggle Competition.