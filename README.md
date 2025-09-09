# Tunisian IT Job Market Analysis 2021

This project aims to present insights about the Tunisian IT job market in 2021.  
The analysis highlights the most demanded job positions, salary ranges, and popular technologies used in Tunisia during that year.

![Dashboard Preview](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/8.png?raw=true)

---

## 📌 Project Overview
The goal of this project was to help **Tunisian junior developers and students** understand the local IT market by presenting:
- The most demanded job titles.
- The most frequently used technologies.
- Salary distributions and ranges.

## 📂 Data Source
- The dataset was collected via **Google Forms**.  
- It contains **85 rows**.  
- Data was collected in **2021** and has **not been updated** since.  


## 🧹 Data Cleaning
The original Google Forms dataset was messy and required ~4 hours of cleaning. 
The main steps were:

**1. Date column**  
   - Removed unnecessary parts and converted to a small date format.  

**2. Company name (`nom entreprise`)**  
   - Applied `TRIM` and `PROPER` functions to clean.  
   - Removed invalid/messy cells.  
   - Added a classification column (`Company / Startup / Agency / Other`).  

**3. Job Title (`Poste`)**  
   - Unified naming conventions (e.g., standardized roles with different spellings).  

**4. Technological Stack (`Stack technologique`)**  
   - Cleaned separators and technology names.  
   - Created a new column **`Split Technologies`** where each technology was separated into its own row (for counting usage).  
   - Moved this column to a separate sheet to avoid blank values.  

**5. Experience (`Année`)**  
   - Converted to numeric values representing years of experience.  

**6. Salary (`Salaire`)**  
   - Extracted only numeric values.  
   - Added a new column for **SIVP status** (Yes / No).  
   - Created a new column **`Salary Brackets`**

---

# 📊 Data Visualization

After cleaning the dataset, I used **pivot tables** to explore the data and design the dashboard.  
The pivot tables helped me decide which insights to highlight.  

## 1. Number of Positions by Job Title
![chart 1](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/1.png?raw=true)
👉 Shows which job titles are most common in Tunisia.  
- **Ingénieur d’affaires** and **Fullstack Developer** were the most in-demand roles.  
- Specialized roles such as **DevOps Engineer** and **Data Scientist** had fewer postings.  

## 2. Average Salary by Years of Experience
![chart 2](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/2.png)
👉 Shows how salary increases with experience.  
- Salaries start low (~600–1000 TND) for juniors.  
- A sharp increase is observed after **5–7 years** of experience.  
- Peak salaries were reported around **7–8 years** of experience.

## 3. Average Salary by Job Title
![chart 3](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/3.png)
👉 Compares salaries across different positions.  
- **Database Administrator** and **Devops Engineer** earned among the highest salaries.  
- This highlights the **salary gap** depending on specialization and seniority.  

## 4. Average Salary by Employment Type
![chart 4](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/4.png)
👉 Compares salary averages based on employer type.  
- **Freelance** generally offered lower salaries.  
- **Agency and Startups** provided mid-level salaries.  
- **Consultancies and Companies** paid the most consistent and higher salaries.
- 
## 5. Salary Ranges
![chart 5](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/5.png)
👉 Breaks down salaries into ranges.  
- Most respondents earned **between 2000 and 3000 TND**.  
- A smaller number earned **more than 5000 TND**, representing **senior or niche roles**.  

## 6. Most Demanded Technologies
![chart 6](https://github.com/mounatounakti/Tunisian-IT-Job-Market-Data-Analysis/blob/e1aaff80050962d23a3a5fdfb498797fdb5d3f97/imgs/7.png)
👉 Identifies which technologies appeared most in job postings.  
- **ReactJS** and **JavaScript** were the top technologies.  
- **Angular** and **NodeJS** followed closely.  
- Backend and enterprise tools like **Java**, **Python**, and **.NET** also appeared frequently.  

---

## 📝 Notes
- The dataset represents a **snapshot of 2021** and should **not** be taken as the current state of the Tunisian IT market.  
- The project demonstrates how raw community data can be **cleaned, structured, and transformed** into meaningful insights.  



