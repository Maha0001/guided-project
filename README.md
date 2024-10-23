# Google Capstone**HR Analytics: Employee Retention Insights**

## **Project Overview**
This project aims to provide data-driven insights to help Salifort Motors' HR department improve employee satisfaction and reduce turnover. By analyzing employee data, this project identifies key factors influencing employee retention and offers actionable insights for enhancing workplace satisfaction and productivity.

**Objective**: Analyze employee data to identify trends, correlations, and insights regarding employee retention, without building predictive models.

## **Dataset**
The dataset consists of employee records, with the following features:
- **satisfaction_level**: Self-reported job satisfaction level [0–1]
- **last_evaluation**: Score of employee’s last performance review [0–1]
- **number_project**: Number of projects an employee contributes to
- **average_monthly_hours**: Average number of hours worked per month
- **tenure**: Number of years with the company
- **work_accident**: Whether the employee had a work accident (0/1)
- **left**: Whether the employee left the company (0/1)
- **promotion_last_5years**: Whether the employee was promoted in the last 5 years (0/1)
- **department**: Employee’s department
- **salary**: Employee’s salary level (low, medium, high)

Total rows: **14,999**  
Columns: **10**  

## **Project Structure**
- **Data Cleaning**: Renamed columns for consistency, handled missing values, and removed duplicates.
- **Exploratory Data Analysis (EDA)**: Visualized key trends in employee satisfaction, project workload, working hours, and tenure to uncover factors influencing attrition.
  
## **Installation**
1. Download or clone the repository:
    ```bash
    git clone https://github.com/Maha0001/guided-project.git
    cd guided-project
    ```
2. Use a Python environment with the necessary libraries installed:
    ```bash
    pip install pandas matplotlib seaborn numpy
    ```

3. Load and explore the dataset using `salifort-motors-project.ipynb`.

## **Key Findings**
- **Overwork**: Employees who work on more projects and longer hours show a higher likelihood of leaving the company.
- **Tenure**: Employees with a tenure of 4+ years and those who worked on 7 projects all left the company, indicating potential burnout.
- **Satisfaction**: A direct correlation was found between low satisfaction levels and high attrition rates.
- **Department Analysis**: No significant department-specific trends were found in relation to attrition, though the most affected departments were sales and technical.
  
## **Visualizations**
- **Boxplot**: Distribution of monthly hours by the number of projects worked on.
- **Scatterplot**: Employee satisfaction versus monthly hours, indicating burnout.
- **Histograms**: Tenure and project workload comparison between employees who left and those who stayed.
- **Correlation Heatmap**: Shows relationships between variables like satisfaction, evaluation scores, and hours worked.

## **Conclusion**
The analysis indicates that employees at Salifort Motors are overworked, and this leads to high attrition. Addressing work-life balance and offering better incentives (like promotions or higher salaries) may improve retention rates.
