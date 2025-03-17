# Data-Wrangling-of-FIFA-Data
**Project Title:**
Data Wrangling of FIFA 21 (Football) Dataset

**Description:**
Data collected from various sources—whether through web scraping, databases, or live streams—is rarely clean or structured in a way that is immediately suitable for analysis. Before performing any form of analysis, ensuring the quality and reliability of data through proper validation and cleaning is essential.
Cleaning and preprocessing data from the 2021 version of the FIFA game, which was scraped from a website and is available in its raw format. The dataset contains over 18,000 rows and 75 columns, providing an excellent opportunity to apply various data wrangling techniques. This process ensures the dataset is accurate, consistent, and ready for meaningful analysis.

**Dataset Overview:**
The dataset used for this project is available on Kaggle and contains 18,979 entries and 77 columns. It includes metrics related to player attributes such as name, age, nationality, and club, along with contract details like wages, joining dates, and duration with the team. Additionally, it provides data on player capabilities, including agility, attacking, defending, and goalkeeping skills, as well as overall ratings.
Since the dataset is in its raw format, it serves as an excellent resource for understanding data preprocessing steps and applying various data wrangling techniques.

**Dataset Link:** https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring/data
________________________________________
**Tools & Concepts Explored:**
This project was carried out using Jupyter Notebook, leveraging Python libraries such as Pandas and NumPy for data manipulation and cleaning. The primary concepts explored include:
- Data Cleaning  
- Data Validation and Standardization  
- Feature Engineering  

________________________________________
**Methodology:**
1. Data Loading and Exploration:
The dataset was loaded into a Pandas DataFrame, and an initial exploratory analysis was performed to understand its structure, missing values, and inconsistencies.
2. Data Cleaning:
2.1 Removing Duplicates: Duplicate records were identified and removed to ensure data integrity.
2.2 Fixing Inconsistencies: Inconsistencies in naming conventions, categorical values, and column formats were corrected.
2.3 Handling Missing Values: Missing data was handled using various techniques such as imputation, deletion, or marking them as NaN where applicable.
2.4 Renaming and Dropping Columns: Certain columns were renamed for better readability, while irrelevant or redundant columns were removed.
3. Data Validation and Standardization:
3.1 Fixing Data Types: Ensured that all columns had appropriate data types (e.g., converting date-related columns to datetime format).
3.2 Reordering Columns: Columns were reorganized to enhance the dataset’s readability and logical flow.
3.3 Data Validation: Applied numerical and logical checks to confirm data accuracy. For instance:
•	Ensured that ‘Joined Date’ was earlier than or equal to ‘Contract Start Year’.
•	Verified that ‘Loan End Date’ values were valid based on player status.
•	Cross-checked that statistical total matched expected sums.
4. Feature Engineering:
New features were created to enhance the dataset’s analytical value, such as:
•	Player Experience Feature: Measured as the difference between 'Contract End Year' and 'Contract Start Year'.
•	Performance Per Wage Feature: A ratio of overall rating (OVA) to wage, helping assess player efficiency.
•	Age Bracket Segmentation: Categorized players into different age groups for trend analysis.
•	Position Versatility Feature: Counted the number of positions a player could play based on available data.
________________________________________
**Learnings:**
1.	A Systematic Approach to Data Wrangling is Essential: Cleaning and preprocessing data requires a structured plan to ensure efficiency and accuracy.
2.	Handling Missing & Inconsistent Data is Crucial: Properly addressing missing values and inconsistencies prevents data biases and inaccuracies.
3.	Data Naming & Column Ordering Conventions Improve Readability: Standardized naming and well-organized columns enhance dataset usability.
4.	Understanding Data Deeply Can Lead to Better Refinements: Initial assumptions may change after deeper exploration, necessitating adjustments in the wrangling process.
5.	Validation Rules Strengthen Data Accuracy: Implementing validation checks ensures data correctness, preventing logical inconsistencies.
6.	Each Column Can Have Unique Issues: No single cleaning approach fits all; each column requires specific handling based on its nature and expected values.

