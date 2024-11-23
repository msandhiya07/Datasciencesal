Data Science Salaries Dataset
This repository contains a dataset of data science salaries across different regions, industries, and roles. It provides valuable insights into the earning trends in the field of data science. The dataset can be used for various purposes such as salary analysis, machine learning model development, and career trend predictions.

Dataset Overview
The dataset ds_salaries.csv includes details about the salaries of data science professionals. It contains the following columns:

job_title: The title of the data science position (e.g., Data Scientist, Data Analyst, etc.).
salary: The annual salary of the data scientist in USD.
location: The geographical location where the job is based (e.g., USA, India, etc.).
experience_level: The experience level required for the job (e.g., Junior, Mid-level, Senior).
education_level: The education qualification required for the role (e.g., Bachelor's, Master's, PhD).
company_size: The size of the company (e.g., Small, Medium, Large).
industry: The industry in which the company operates (e.g., Tech, Finance, Healthcare, etc.).
Getting Started
To get started with the dataset, you can clone this repository to your local machine:

bash
Copy code
git clone https://github.com/msandhiya07/Datasciencesal.git
Usage
You can use the dataset for:

Salary Analysis: Understand trends in data science salaries across different industries, experience levels, and locations.
Data Science Projects: Use the data for practice in data analysis, visualization, and machine learning.
Salary Prediction Models: Build predictive models based on the features in the dataset (e.g., predict salary based on experience and location).
Example: Salary Distribution Visualization
Here's an example of how you might visualize the salary distribution across experience levels using Python and matplotlib:

python
Copy code
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
data = pd.read_csv('ds_salaries.csv')

# Plot salary distribution by experience level
plt.figure(figsize=(10, 6))
data.groupby('experience_level')['salary'].median().plot(kind='bar')
plt.title('Median Salary by Experience Level')
plt.xlabel('Experience Level')
plt.ylabel('Salary (USD)')
plt.show()
Dependencies
To work with the dataset, you can use the following Python libraries:

pandas - for data manipulation and analysis
matplotlib - for plotting graphs
seaborn - for statistical data visualization
numpy - for numerical operations
