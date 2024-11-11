# Fetch---Data-Analyst

1. Explore the Data
   - Review the unstructured csv files and answer the following questions
       - I reviewed the unstructed csv files using python and pandas library in a jupiter notebook to be able to analyze/understand and explore the data.  
   - Are there any data quality issues present?
       - There are data quality issues present with the cvs files. Some that I have encountered were missing values, incorrect data types, duplicates, and outliers. I have included my code in this repository. Where I have loaded the three csv files and checked for data quality issues and also check the structure of each file. I have found columns with significant missing values where it can be interpreted as incomplete data. I also found duplicate rows where it can cause data error/acturacy. In viewing the files there is inconsistent data entries such as "zero" instead of 0 which it should be standardized.
   - Are there any fields that are challenging to understand?
       - Yes, there are fields that are challenging to understand such as unclear data in non-numeric fields, for instance in "LANGUAGE" there is a mixed of language codes, in "GENDER" there is an unclear value and in "FINAL_QUANTITY" there is an inconsistent data like "zero". There is also ambiguous field like "FINAL_SALE which include missing entries in which this can affect actuacy in data it need a consistent format.
    
2. Provide SQL queries
   - Closed-ended questions:
       - What are the top 5 brands by receipts scanned among users 21 and over?
           - I answered this question in the jupiter notebook. In this query I was able to identify the top 5 brands by the number of receipts scanned among users who are 21 years or older. With "Age_Users" I first filtered users who are at least 21 years old or older using their birthdate. I then counted the total number of receipts scanned by users that also meet the age criteria. From this query it is important to understand which brands are popular among users. This helps maketing opportunities and allow us to make data decisions. The top 5 brands by receipts scanned among users 21 and over are nerds candy, trident,tostitos, suave, and none. 
       - What are the top 5 brands by sales among users that have had their account for at least six months?
             -  I answered this question in the jupiter notebook. In this query I was able to identify the 5 top brands by saless among users that had their account for at least six months. My SQL query ensures thats only users who had their account for at least 6 months are considered and it will calculate the top 5 brands based on the sale volumes. From focusing on this subset i was able to have a clearer view of lon term user prederences and brand loyalty. The top 5 brands by sales among users that have had their account for at least six months are CVS, great value, crest, oral-b, and nabisco. 
    
    - Open-ended questions:
        - Who are Fetch’s power users?
            - When answering this question I assumed that power user is high engagement levels which is users with frequent spending and highest total spending. I assumed that the dataset included total spending and number of transactions associated with each user. In order to help me find these users, I was able to run a query on transaction data to rank users by their total spending and transaction count. I answered this question in the jupiter notebook. The Fetch's power users are:
                - ID                   Total_Spend
                - 0  643059f0838dd2651fb27f50        75.99
                - 1  62ffec490d9dbaff18c0a999        52.28
                - 2  5f4c9055e81e6f162e3f6fa8        37.96
                - 3  5d191765c8b1ba28e74e8463        34.96
                - 4  6351760a3a4a3534d9393ecd        27.74
                - 5  64dd9170516348066e7c4006        26.52
                - 6  62c09104baa38d1a1f6c260e        20.28
                - 7  61a58ac49c135b462ccddd1c        19.92
                - 8  6661ed1e7c0469953bfc76c4        18.60
                - 9  5b441360be53340f289b0795        18.32
