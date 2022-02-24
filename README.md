# Amazon_Vine_Analysis
The purpose of the project was to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
In this project, I had access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. Out of these datasets I chose music and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there was any bias toward favorable reviews from Vine members in my dataset. The following is an analysis to submit to Sellby stakeholders.

### Tools
  -PySpark for large datasets and to transform and filter data
  -PySpark to perform ETL
  -AWS Simple Storage Service (S3)
  -SQL/pgAdmin
  -Google Colab Notebook

## Results

### Vine vs. non-Vine reviews
  -There were a total of 105969 reviews, as shown. Out of the 105969, 7 of them paid for their membership, whill the other 105962 members did not pay.

<img width="685" alt="Screen Shot 2022-02-23 at 8 16 23 PM" src="https://user-images.githubusercontent.com/86068655/155439058-f63da29b-7d15-46de-895b-2b370c36dbb5.png">


### 5 star reviews: total, paid and unpaid memberships
  -The total number of 5 star reviews were 67568. 0 of those 67568 were paid and 38394 were unpaid 5 star reviews.

<img width="729" alt="Screen Shot 2022-02-23 at 8 16 54 PM" src="https://user-images.githubusercontent.com/86068655/155439456-a10ac343-225d-4033-9829-8a9708dcf91d.png">


### Precentages of paid/unpaid Vine reviews that were 5 star

% of total 5-star Vine reviews of total Vine reviews was 0, nobody had a paid membership who gave a 5 star review.

% of total 5-star non-Vine reviews compared to the total non-Vine reviews was 36%.

% of 5-star non-Vine reviews compared to the total 5-star reviews was 56%.

<img width="855" alt="Screen Shot 2022-02-23 at 8 17 28 PM" src="https://user-images.githubusercontent.com/86068655/155440126-c86baf76-a7cf-43e6-811d-d3c42a9f1b4c.png">

# Summary
Clearly there are skewed results as there no 5 star reviews from paid vine membership. Granted, only 7 people paid for a membership. Explicict bias exists in the data. It would be safe to say that any results taken from this data would be useless because nearly all reviews came from non-Vine members.

A recommendation would be to find trends or deviations from data results that would be considered normal; therefore, we can know whether to accept of reject the use of the data being anayized. 
