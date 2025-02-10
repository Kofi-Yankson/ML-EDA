# ML-version1
 Dataset consists of user information gained from students using dating apps in  india
 Data set consists of 500 rows and 16 columns
### **Data Dictionary**

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

 
#Cleaning Steps
#1.Checking For duplicates
No duplicates were found so no changes where made to target them
#2. Checking for categorization Inconsitencis
 Columns that may have had inconsitent categories due to diffent capitalization such as 'male' and  "Male' where checked individually to  see if any of them possesd those inconsitencies, this consisted of the Gender,Education and Occupation Columns
No inconsistent values were found so no chnages were made to target them
#3.Checking for missing values
The dataset was checked for mmissing values by shoing the sum of null values each column had. the columns that had missing values consiseted of 'Primary_App','Secondary_App' and 'Challenges'
To deal with this each null value was replace with the  value 'Unknown'
#4.Creating categorical columns.
All columns that were not numerical columns were converted to categorical columns, the only numerical column present was 'Age'.
