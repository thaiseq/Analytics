# Telecom Data Churn Analysis

   The goal of this project is to identify those customers most likely to churn at a fictitious telecom company, that is, the subscribers who are most likely to leave the company. Once identified, it's possible to focus on retention actions, providing adequate intervention to encourage them to stay and minimize customer exit. The dataset for this project was obtained from the [OpenMl](https://www.openml.org/d/40701) public repository. A dataset relating characteristics of account features and usage and whether or not the customer churned. In the context of this project, this is a problem of supervised classification and Machine Learning algorithms will be used for the development of predictive models and evaluation of accuracy and performance. It seeks to find the most appropriate model for the business.

# 1. Churn

  Churn Customer can be defined as a user who is likely to discontinue using the services.  So, the target variable confirm if the customer has churned (1=yes; 0 = no).

# 2. Dataset

   The data included 5.000 users and by the exploratory analysis, it is observed that:

   * 14% of the base are classified as churn.
   * 50% of the customers who called the company more than 3 times are classified as Churn.
   * 10% of those with no international plan are classified as Churn, while only 8% of those with an international plan are Churn.
   
  ### 2.1 Columns
   
   * ID 
      * 'area_code', 'phone_number',


   * Features 
      * 'state',
      * 'account_length', 
      * 'international_plan', 
      * 'voice_mail_plan', 
      * 'number_vmail_messages',     
      * 'total_day_minutes', 
      * 'total_day_calls', 
      * 'total_day_charge',
      * 'total_eve_minutes', 
      * 'total_eve_calls', 
      * 'total_eve_charge',
      * 'total_night_minutes',
      * 'total_night_calls', 
      * 'total_night_charge',
      * 'total_intl_minutes', 
      * 'total_intl_calls', 
      * 'total_intl_charge',
      * 'number_customer_service_calls', 

   * Target
      * 'class'
    
# 3. Modeling and Results

I used 20 features to run my models. I ran 4 classifier models and plotted their ROC curves using k-fold cross validation. 

Their respective AUC (Area Under the Curve) measures are listed below:
    
    Gradient Boosted Trees:
    Random Forest:    
    AdaBoost:
    Logistic Regression: 

Gradient Boosted Trees produced the highest AUC and the following scores:

    Accuracy: 94% labeled correctly
    Precision: 95% labeled as churn actually churned (5% were wrongly labeled as churn)
    Recall: 98% that actually churned were labeled as churn (2% of churn users were labeled as non-churn)
    
    
 # 4. Feature Importance

According to the feature importance analysis produced by the Random Forest algorithm, the following features had the highest predictive power:

    1.
    2.
    3.
    4.
    5.
    
# 5. Conclusion



# 6. Tools

    Python, Sklearn, Pandas, Numpy, matplotlib and seaborn

Code and Notebook

    Jupyter notebook
