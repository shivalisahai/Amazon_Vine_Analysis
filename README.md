# Amazon_Vine_Analysis
Big Data with Hadoop - MapReduce, PySpark &amp; AWS ETL.


### Overview

This challenge involves analyzing Amazon reviews written by members of the paid Amazon Vine program. A dataset of watches reviews is chosen for this analysis. ETL process is performed to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Further analysis is carried out to find any bias toward favorable reviews from vine members in the dataset.


### Tools Used

  - Google Colab Notebook
  - PySpark
  - PostgreSQL & pgAdmin 4
  - AWS RDS
  - VS Code
  

### Results

#### Deliverable-1: ETL on Amazon Product Reviews

AWS RDS database is created with tables in pgAdmin, the watches review dataset is extracted into a DataFrame and four separate dataframes created matching the table schema in pgAdmin.

  - Customers_table DataFrame & SQL Table
  
  <img width="181" alt="customers_df" src="https://user-images.githubusercontent.com/104603128/188931418-98fda9f6-9ac7-4cba-a81b-0ab0b85e3a75.png">


![SQL_Customers_Table](https://user-images.githubusercontent.com/104603128/188931979-7d82baf8-15b1-4f79-aa27-0858c0af5010.JPG)


  - Products_table DataFrame & SQL Table
  
  <img width="213" alt="products_df" src="https://user-images.githubusercontent.com/104603128/188931470-f9952c28-7c57-4933-9370-c98552209106.png">


![SQL_Products_Table](https://user-images.githubusercontent.com/104603128/188932030-52a5e56e-4daa-4449-8e3e-b8e0d59ce807.JPG)


  - Review_id_table DataFrame & SQL Table
  
  <img width="390" alt="review_id_df" src="https://user-images.githubusercontent.com/104603128/188931551-6db3d5d8-9707-470b-8eaf-4451af4b11e6.png">


![SQL_Review_ID_Table](https://user-images.githubusercontent.com/104603128/188932097-6352d5c5-2eb2-4b50-8007-6eb2a310999f.JPG)


  - Vine_table DataFrame & SQL Table
  
  <img width="455" alt="vine_df" src="https://user-images.githubusercontent.com/104603128/188931629-a968b5f2-de55-4e06-8efd-cb6e379a465d.png">


![SQL_Vine_Table](https://user-images.githubusercontent.com/104603128/188932126-f91da780-8d59-4667-80a7-0cd718faabc5.JPG)


#### Deliverable-2: Finding Bias of Vine Reviews

  - Number of vine reviews
  
  <img width="530" alt="PaidReviews" src="https://user-images.githubusercontent.com/104603128/188933739-865f8ea5-33eb-40cb-a450-aacb9911a549.png">


  - Number of non-vine reviews
  
  <img width="548" alt="Unpaid_Reviews" src="https://user-images.githubusercontent.com/104603128/188933813-470ae144-fc27-4093-b7a3-ca9dc24bb531.png">

  - Number of Vine 5 star reviews
  
  <img width="450" alt="5Star_Vine_Reviews" src="https://user-images.githubusercontent.com/104603128/188936044-c335ee1e-f001-4932-9227-d8bea1451a64.png">


  - Number of non-Vine 5 star reviews
  
  <img width="491" alt="5Star_nonVine_Reviews" src="https://user-images.githubusercontent.com/104603128/188936105-aa90e1eb-79c5-41d4-9a93-ae22a8ac8263.png">


  - Percentage of Vine reviews that are 5 star
  
  <img width="443" alt="Percentage_5star_Paid" src="https://user-images.githubusercontent.com/104603128/188936265-625cd1b5-2034-42ce-8f81-88fd7683a44e.png">


  - Percentage of non-Vine reviews that are 5 star
  
  <img width="499" alt="Percentage_5star_Unpaid" src="https://user-images.githubusercontent.com/104603128/188936351-fa73daf7-0a48-4e09-bfed-e0ab2b51f730.png">


### Results

  - The percentage of 5-star reviews in the Vine program is around 32% whereas in non-Vine program it is around 52%. Therefore, a positivity bias is not seen for reviews collected in the Vine program.
  
  - Another analysis could be done to find out any negativity bias in the reviews collected under the Vine program by calculating the percentage of 1-star and 2-star reviews in the Vine program and comparing them similar rated reviews in the non-vine program.
  
  
  
