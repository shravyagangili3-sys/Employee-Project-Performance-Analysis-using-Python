### Employee-Project-Performance-Analysis-using-Python

# Employee-Project-Data-Management

[![Python](https://img.shields.io/badge/python-3.13-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/pandas-data%20analysis-brightgreen)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)

---

## Short Description
Automate employee and project data processing, analytics, and reporting using Python and Pandas.

---

## Overview
This repository demonstrates a complete workflow for managing employee and project datasets. It covers:

- Cleaning and transforming project and employee data  
- Handling missing values using running averages  
- Calculating bonuses and updating designation levels  
- Merging multiple datasets into a single comprehensive table  
- Analyzing and filtering data (e.g., total project cost per employee, city-based filters)

Ideal for **data analysts, students, and Python enthusiasts** who want practical examples of data manipulation.

---

## Dataset
Three CSV datasets are included:

1. **project.csv** – Project details:
   - `ID` – Employee ID  
   - `PROJECT` – Project Name  
   - `COST` – Project Cost (missing values handled)  
   - `STATUS` – Project Status (FINISHED, ONGOING, FAILED)  

2. **employee.csv** – Employee information:
   - `ID` – Employee ID  
   - `NAME` – Full Name (split into First and Last Name in processing)  
   - `GENDER` – Employee Gender  
   - `CITY` – Employee City  
   - `AGE` – Employee Age  

3. **seniority.csv** – Employee seniority:
   - `ID` – Employee ID  
   - `DESIGNATION LEVEL` – Numeric seniority level  

---

## Tasks Implemented
1. **DataFrame Creation** – Created project, employee, and seniority datasets.  
2. **Handle Missing Values** – Replaced missing project costs with running averages.  
3. **Split Names** – Divided full names into `First Name` and `Last Name`.  
4. **Merge DataFrames** – Combined all three datasets into `final.csv`.  
5. **Add Bonus** – Added 5% bonus for FINISHED projects.  
6. **Demote Employees** – Reduced designation level for failed projects.  
7. **Add Titles** – Added `Mr.` or `Mrs.` prefix based on gender and removed `GENDER` column.  
8. **Promote Employees** – Increased designation level by 1 for employees over 29 years old.  
9. **Total Project Cost** – Generated `total_project_cost.csv`.  
10. **City-based Filter** – Listed employees whose city contains `"o"`.

---

## Libraries Used
- `pandas` – Data manipulation and analysis  
- `numpy` – Numeric computations  

---

## File Structure
project/
│
├─ project.csv
├─ employee.csv
├─ seniority.csv
├─ final.csv
├─ total_project_cost.csv
└─ Employee_Project_Management.ipynb


---

## Usage
1. Clone the repository:
   ```bash
   git clone <repository_url>
2. Install dependencies:
pip install pandas numpy
3. Run the Jupyter Notebook to execute all tasks and generate final datasets.
