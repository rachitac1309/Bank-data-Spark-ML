# Bank-data-Spark-ML
Classification model to predict wheather to approve loan or not.

A bank wants to leverage machine learning techniques to improve its data analysis capabilities and make informed decisions. Specifically, the bank aims to use Spark ML to develop a predictive model that can accurately predict whether a customer will default on their loan payments or not. This model will help the bank assess the creditworthiness of new loan applicants and minimize the risk of default.


# Dataset Description

Data from a banking institution's direct marketing efforts is being used. On phone conversations, the marketing efforts were based. In order to determine if the product (bank term deposit) would be subscribed ('yes') or not ('no'), it was sometimes necessary to make many contacts with the same client.

The dataset has the following attributes

1.seqId: This attribute is an integer that represents a unique identifier for each record in the dataset. It is used to track individual entries and does not provide any meaningful information about the customers or their characteristics.

2.age: This attribute is an integer that represents the age of the customer. It indicates the customer's age in years.

3.job: This attribute is a string that represents the occupation or job of the customer. It provides information about the type of work the customer is engaged in.

4.maritalStatus: This attribute is a string that indicates the marital status of the customer. It can take values such as "single," "married," or "divorced."

5.education: This attribute is a string that represents the educational background of the customer. It provides information about the highest level of education attained by the customer.

6.default: This attribute is a string that indicates whether the customer has defaulted on their loan payments. It takes the value "yes" if the customer has defaulted and "no" if they have not defaulted.

7.balance: This attribute is a double that represents the account balance of the customer. It indicates the amount of money the customer has in their account.

8.housing: This attribute is a string that indicates whether the customer has a housing loan. It can take values such as "yes" or "no."

9.loan: This attribute is a string that indicates whether the customer has a personal loan. It can take values such as "yes" or "no."

10.contact: This attribute is a string that represents the contact communication type with the customer. It provides information about the method used to contact the customer, such as "cellular" or "telephone."

11.day: This attribute is an integer that represents the day of the month on which the customer was last contacted.

12.month: This attribute is a string that represents the month in which the customer was last contacted.

13.duration: This attribute is a double that represents the duration of the last contact with the customer, measured in seconds.

14.campaign: This attribute is a double that represents the number of contacts performed during this campaign for the customer.

15.pdays: This attribute is a double that represents the number of days that passed after the customer was last contacted from a previous campaign.

16.previous: This attribute is a double that represents the number of contacts performed before this campaign for the customer.

17.poutcome: This attribute is a string that represents the outcome of the previous marketing campaign. It provides information about the success or failure of the previous campaign.

18.opened_new_td_act_yes_no: This attribute is a string that indicates whether the customer has opened a new term deposit account. It can take values such as "yes" or "no."

These attributes provide information about the customers, their demographics, loan details, contact history, and previous marketing campaign outcomes, which can be used for various analyses and predictive modeling tasks.

# ML Spark Model steps involved

Installed Java Development Kit (JDK) and Apache Spark. 

Imported the necessary libraries and set up the Spark session.

Loaded the dataset into a Spark DataFrame.

Explored the data by checking the schema, printing sample rows, and calculating descriptive statistics.

Performed data cleaning and transformation tasks, such as dropping unnecessary columns, replacing negative balances with zeros, and handling missing values.Conducted EDA by analyzing the distribution of the target variable and creating visualizations for different categorical variables.Created a correlation heatmap to understand the relationships between numerical features.

Split the data into training and testing sets.Built a pipeline for data preprocessing, including vector assembling, feature scaling, string indexing, one-hot encoding, and label indexing.Configured a logistic regression model and included it in the pipeline. Trained the pipeline on the training data.

Evaluated the model's performance by calculating accuracy and error rates on both the training and testing datasets.Calculated additional evaluation metrics, such as precision, recall, and F1 score. Analyzed the true positives, true negatives, false positives, and false negatives for both the training and testing datasets.
