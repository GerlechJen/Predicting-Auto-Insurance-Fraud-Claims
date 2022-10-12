# Predicting Auto Insurance Fraud Claims 

### [Tableau Dashboard](https://public.tableau.com/app/profile/bernie2684/viz/Team6_16651826100420/Predictinginsurancefraud?publish=yes)

## Reason for Selection of Topic
Insurance fraud takes various forms from staged automobile collisions to submission of false invoices for rehabilitation services, and false theft claims just to mention a few. This causes insurance companies to suffer significant financial loss which affects their financial resources to pay legitimate claims. In the long run insurance consumers are the ones who suffer because they are made to pay higher premiums. In Ontario alone, the Insurance Bureau of Canada estimated that the cost of insurance fraud ranges between $770 million and $1.6 billion a year. It can be quite a challenge to determine which claims for insurance are legitimate and which ones are fake.

The reason for selecting this topic is to use machine learning to predict insurance claims that might be a fraud. After obtaining the list of fraudulent claims, the insurance company can take further action and investigate for confirmation. This will help increase the rate at which fraud investigation is carried out by insurance companies.

## Description of Source of Data

Our Dataset is sourced from Kaggle. The 25 columns and description are as below:
1) months_as_customer: It denotes the number of months for which the customer is associated with the insurance company.
2) age: continuous. It denotes the age of the person.
3) policy_number: The policy number.
4) policy_bind_date: Start date of the policy.
5) policy_state: The state where the policy is registered.
6) policy_csl-combined single limits. How much of the bodily injury will be covered from the total damage.
7) policy_deductable: The amount paid out of pocket by the policy-holder before an insurance provider will pay any expenses.
8) policy_annual_premium: The yearly premium for the policy.
9) umbrella_limit: An umbrella insurance policy is extra liability insurance coverage that goes beyond the limits of the insured's homeowners, auto, or watercraft insurance. It provides an additional layer of security to those who are at risk of being sued for damages to other people's property or injuries caused to others in an accident.
10) insured_zip: The zip code where the policy is registered.
11) insured_sex: It denotes the person's gender.
12) insured_education_level: The highest educational qualification of the policy-holder.
13) insured_occupation: The occupation of the policy-holder.
14) insured_hobbies: The hobbies of the policy-holder.
15) insured_relationship: Dependents on the policy-holder.
16) capital-gain: It denotes the monitory gains by the person.
17) capital-loss: It denotes the monitory loss by the person.
18) incident_date: The date when the incident happened.
19) incident_type: The type of the incident.
20) collision_type: The type of collision that took place.
21) incident_severity: The severity of the incident.
22) authorities_contacted: Which authority was contacted.
23) incident_state: The state in which the incident took place.
24) incident_city: The city in which the incident took place.
25) incident_location: The street in which the incident took place.


## Questions to be Answered with the Data 
1) How often poeple file for insurance claim?
2) Decision whether claim is fradulant or not?

## Machine Learning Model
We will be using classification - supervised machine learning model.
![image (1)](https://user-images.githubusercontent.com/104685001/191869886-2b0721a4-bbb1-4ee5-8ff3-37de7e556129.png)

**Machine learning model - Decision Tree Classifier**

**Why we chose Decision Tree Classifier model?**

Decision tree classifer is easy to intepret, understand and visualize.
It can be used for both regression and classification problems.

Our team is trying to build a machine learning model to predict the likelihood of insurance fraud based on the dataset.

**What are the benefits?**

Decision tree helps to quickly identify relationships between variables and the most significant variable.

The output of a decision tree can also be easily understood.

**What are the limitations?**

Decision trees cannot be used well with continuous numerical variables.

A small change in the data tends to cause a big difference in the tree structure, which causes instability.

**Machine learning model - Random Forest Classifier**

**Why we chose Random Forest Classifier model?**

Insurance analysis requires a lot of effort as it contains a high risk of profit and loss.

Customer analysis is the most common studies done for fraud prediction. RFC is a great choice for fraud detection.

**What are the benefits?**

Reduced overfitting in decision trees and helps to improve accuracy.

Flexible to both classification and regression problems.

**What are the limitations?**

Takes longer time to train as it combines a lot of decision trees.

Takes much computational power and resources as it builds many decision trees to combine their outputs.


## Loading CSV file into dataframe
We used the following code to load the CSV file into dataframe
![image](https://user-images.githubusercontent.com/104685001/191875241-f5f1489c-5be1-4cc6-bc94-a80e89b9560f.png)

We have loaded our dataframe into a sql database.
![image](https://user-images.githubusercontent.com/104685001/191875286-cc362854-a94f-4272-9c2e-e4ddc6820915.png)
![image](https://user-images.githubusercontent.com/104685001/191875320-666a378b-a3e8-4ba7-b32a-a3add6df36c7.png)

## Description of Data Preprocessing/Feature Engineering

### Data Preprocessing

- Checking null values.
- Dropping columns.
- Counting the number of frauds and visualizing.

### Feature Engineering:

- Creating dictionaries to change datatypes using map function to convert datatypes.
- Calculation average fraud reported using groupby functions.
- Dropping more columns.

## Tools used for Dashboard
Tableau will be used to visualize our data and share insights

Details on our dashboard will include the following:
- Fraud reported by gender
- Frauds by state
- Fraud reported by age group


## Technology Stack
* Jupyter notebook - To load the dataset into dataframe and subsequently into database.
* Python - Programming language used
* Pandas - Libraries used for creating and cleaning the dataset.
* Postgres - Storing the dataset into tables.

## Team Roles
* Square: Sandeep
* Triangle: Jennifer
* Circle: Bernie
* X: Yuvraj
