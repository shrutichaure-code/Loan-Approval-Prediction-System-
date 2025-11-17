
Project Title - Loan Approval Prediction System Using Machine Learning

Objective - Our goal is to create an automated machine learning based system that would predict whether a loan application will be accepted or not. This will be based on the applicant’s income, credit history, current status, and loan amount.  Dataset details – Dataset Description. The data set utilized in this project contains the information of applicants taken by the banks for loans. It has credit-related, demographic and financial details along with final loan sanction status.  Attributes Included.

 Personal Information.
 Gender – Male/Female. Marital Status – Married/Unmarried.
 Number of Dependents – 0, 1, 2, 3+. Education – Graduate / Not Graduate.
  Employment Details. Self-Employed – Yes/No.
  Financial Features.  
 Applicant Income – Monthly income of primary applicant. 
 Co-applicant Income – Additional income from co-borrower.
  Loan Amount – Requested loan amount.  
  Loan Amount Term – Repayment duration in months. 
  Credit Information. Credit History – Whether the individual has repaid or not (0 or 1).  
  
  Property Area. Urban, Semi-Urban, Rural.  Target Variable. Loan Status – Approved (1) or Rejected (0).  Dataset Size. Around 600–700 records (typical for this dataset).  Contains both categorical and numerical features. Missing Values.  The missing entries in some columns (Loan Amount, Dependents, Credit History, Gender) were handled with.  Median imputation for numerical features.  Mode imputation for categorical features. Class Distribution.  Slight class imbalance. ~68% approved loans. ~32% rejected loans.  
  
  #  LOAD AND DISPLAY FULL DATASET FILE = "loan prediction dataset.csv" df = pd.read_csv(FILE) print(" Dataset Loaded Successfully!") # Show full dataset instead of top 5 rows pd.set_option('display.max_rows', None) pd.set_option('display.max_columns', None) display(df) print("\n--- DATA INFO ---") print(df.info()) print("\n--- MISSING VALUES PER COLUMN ---") print(df.isnull().sum()) 
  
  Dataset link - https://colab.research.google.com/drive/1xWaE_VyG7E1E9NBJ7mUJqbXI0JuuPUDa - scrollTo=rNfP_nUV4ruX  
  
  Algorithm/model used –
  
  1. Logistic Regression. (Best model) Logistic Regression is a very basic yet powerful statistical model mainly used in a binary classification. It calculates the likelihood of an applicant being accepted or discarded on the basis of factors. It assumes a linear relationship between the features and the log odds of the target. Advantages: Simple, fast, interpretable. Can’t work on non-linear datasets.
  
  2. Decision Tree Classifier. A decision tree is a rule-based model that splits data into branches based on their feature values. It can take note of non-linear patterns and easy to interpret. It works well with categorical data and is intuitive. Prone to overfitting and has high variance.
  
   3. Random Forest  Random Forest is a type of machine learning model that takes outputs from decision trees to produce a final classification or regression value.  It manages complex data, cuts down overfitting and boosts performance. The benefits include accurate handling of noise and robustness to outliers.
   

  Conclusion –
This project shows how using machine learning can speed up the banking system’s loan approval process and make it more efficient. By employing ML models like Logistic Regression, Decision Tree, and Random Forest, the system can predict faster and accurately as compared to traditional manual evaluation, which is often slow, inconsistent and subject to human mistake. Out of all the models used the Random Forest Classifier was the most accurate thus the best choice among all. The model uses important characteristics of the applicants like credit history, income, amount of loan and current employment status to determine whether the applicant will be granted a loan or not. Not only this cuts down the loan officer’s workload but also guarantee more consistent and unbiased outcomes and improve decision-making. To sum up, the Loan Approval Prediction System is scalable, efficient, data-driven, and can greatly boost the operational efficiency of financial institutions. 
    
Future scope –  
A bigger, more diversified dataset can yield more trustworthy predictions. The model can also be integrated into the web or mobile application to approve the loan instantly. Loan officers can enhance their understanding of predictions by adding explainable AI tools. In the future, it can be extended with features like fraud detection and models update in a continuously fashion. 
    
    
References –
    
  [1] E. Hussein Sayed, A. Alabrah, K. Hussein Rahouma, M. Zohaib and R. M. Badry, "Machine Learning and Deep Learning for Loan Prediction in Banking: Exploring Ensemble Methods and Data Balancing," in IEEE Access, vol. 12, pp. 193997-194019, 2024, doi: 10.1109/ACCESS.2024.3509774 
    
  [2] Viswanatha v. Ramachandra Ac "Prediction of Loan Approval in Banks using Machine Learning Approach" in August 2023International Journal of Engineering and Management Research 13(4):7-19 DOI:10.31033/ijemr.13.4.2 
    
  [3] Shinde, A. (2022). Intelligent Loan Assistant using Machine Learning and Data Science. International Journal of Scientific Research in Engineering and Management. https://doi.org/10.55041/0522.12643. 
    
  [4]Anand, Mayank, Arun Velu, and Pawan Whig. "Prediction of loan behaviour with machine learning models for secure banking." Journal of Computer Science and Engineering (JCSE) 3.1 (2022): 1-13. 
    
  [5]Kumar, Arun, Garg Ishan, and Kaur Sanmeet. "Loan approval prediction based on machine learning approach." IOSR J. Comput. Eng 18.3, 18-21, 2016. 
