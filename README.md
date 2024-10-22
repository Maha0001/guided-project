# **Google Capstone project: Providing data-driven suggestions for HR**

## **Project Overview**
This project aims to help the HR department of Salifort Motors identify factors that contribute to employee attrition using predictive analytics. By analyzing historical employee data, we developed a machine learning model to predict whether an employee is likely to leave the company, enabling the HR team to take proactive measures for improving employee retention.

**Objective**: To build a predictive model that accurately classifies employees who are at risk of leaving the company and provide actionable insights to improve retention.

## **Dataset**
The dataset used for this project contains employee records from Salifort Motors, with the following attributes:
- **satisfaction_level**: Employee's self-reported satisfaction (0-1)
- **last_evaluation**: Employee's performance review score (0-1)
- **number_project**: Number of projects the employee is involved in
- **average_monthly_hours**: Average number of hours worked per month
- **tenure**: Number of years the employee has been with the company
- **work_accident**: Whether the employee has had a work-related accident (0/1)
- **left**: Whether the employee left the company (0/1)
- **promotion_last_5years**: Whether the employee was promoted in the last five years (0/1)
- **department**: Employee's department
- **salary**: Employee's salary level (low, medium, high)

You can find the dataset [here](link to dataset).

## **Project Structure**
The project is structured as follows:
- **Data Preprocessing**: Cleaned the dataset by handling duplicates, renaming columns, and engineering features like `overworked` to reflect employees working excessive hours.
- **Exploratory Data Analysis (EDA)**: Visualized relationships between variables such as satisfaction, tenure, and hours worked to understand patterns and potential causes of attrition.
- **Modeling**: Built classification models using Logistic Regression, Decision Tree, and Random Forest to predict employee attrition.
- **Model Evaluation**: Evaluated the models using metrics such as accuracy, precision, recall, F1 score, and AUC score.

## **Installation**
To run this project locally, you will need to install the following libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost
```

## **Usage**
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/HR-Analytics-Capstone.git
    cd HR-Analytics-Capstone
    ```
2. Run the Jupyter Notebook or Python script:
    ```bash
    jupyter notebook HR_Analytics_Prediction.ipynb
    ```
3. Load the dataset and execute the cells for data exploration, preprocessing, and model building.

## **Key Findings**
From our analysis, we identified several factors that influence employee attrition:
- Employees with **low satisfaction levels** and **high working hours** are more likely to leave the company.
- **Tenure** of less than 6 years and **working on 6+ projects** also correlates with higher attrition rates.
- All employees involved in 7 projects left the company, likely due to burnout.
  
The final Random Forest model achieved **96% accuracy** and provided actionable insights for the HR team to reduce attrition.

### **Key Visualizations**
![Satisfaction vs. Attrition](link_to_visualization)
> Visualization shows employees with lower satisfaction levels are more likely to leave.

## **Conclusion**
Using this predictive model, the HR department can identify employees at risk of leaving and implement strategies to improve retention, reducing hiring costs and improving workplace satisfaction.

## **Next Steps**
- Fine-tune the model with additional data such as employee engagement surveys.
- Automate the predictive model and integrate it into the HR system for continuous monitoring.

## **Technologies Used**
- **Languages**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost
- **Tools**: Jupyter Notebook, GitHub

---
