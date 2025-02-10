# **ML-Version1**  
This dataset contains user information collected from students using dating apps in India.  
The dataset consists of **500 rows** and **16 columns**.  

---

## **Data Dictionary**  

| Column Name               | Data Type | Description |
|---------------------------|----------|-------------|
| **User_ID**               | int64    | Unique identifier for each user |
| **Age**                   | int64    | Age of the user in years |
| **Gender**                | object   | User's gender (`Male`, `Female`, or `Other`) |
| **Location**              | object   | User's geographic location |
| **Education**             | object   | Highest level of education attained |
| **Occupation**            | object   | User's current job or role |
| **Primary_App**           | object   | Most frequently used app by the user |
| **Secondary_Apps**        | object   | Other frequently used apps |
| **Usage_Frequency**       | object   | How often the user accesses the internet (`Daily`, `Weekly`, etc.) |
| **Daily_Usage_Time**      | float    | Number of hours spent online per day |
| **Reason_for_Using**      | object   | Main purpose of internet usage |
| **Satisfaction**          | int64    | User satisfaction level (1 = low, 5 = high) |
| **Challenges**            | object   | Difficulties faced while searching online |
| **Desired_Features**      | object   | Features users want in an online search system |
| **Preferred_Communication** | object | User’s preferred way of receiving updates |
| **Partner_Priorities**    | object   | Priorities users consider when choosing an online platform |

---

## **Cleaning Steps**  

### **1. Checking for Duplicates** 
-The data set was searched for duplicate rows
- No duplicate rows were found, so no changes were made.  

### **2. Checking for Categorical Inconsistencies**  
- Columns that may have inconsistent values due to capitalization (e.g., `'male'` vs. `'Male'`)  and any other kind of inconsitencies were checked individually  see if any of them possesd those errors. The **Gender, Education, and Occupation** columns were reviewed.  
- No inconsistent values were found, so no changes were needed.  

### **3. Handling Missing Values**  
- The dataset was checked for missing values by summing the null values in each column.  
- Missing values were found in  **Primary_App** , **Secondary_Apps** and **Challenges**  
- All missing values were replaced with **"Unknown"** to ensure consistency.  

### **4. Creating Categorical Columns**  
- All **non-numerical columns** were converted to categorical data types.  
- The only **numerical column** present was **Age**.
- the coloumn **Satisfaction** was also changed to a categorical type due to the nature of its use of numbers to categorise rather than provide statistical information

### **5. Checking for Outliers**
- the age column was reviewed using the IQR and box plot to find and display any out liers
- No outliers wer found
---

This cleaned dataset is now **ready for analysis**.  
