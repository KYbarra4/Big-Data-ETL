# Music Data ETL

## Extract

- Uses PySpark to connect to and load the AWS datasets into DataFrames
- The correct parameters are used to read in the data into a DataFrame

![spark1](https://user-images.githubusercontent.com/113717031/224580759-95e63269-4b2d-45e5-8ade-d82f51dfb827.png)

- The first 10 rows of the DataFrame is displayed
- The number of rows for the DataFrame is displayed

![spark2](https://user-images.githubusercontent.com/113717031/224580876-a93d5e47-7bf1-40ad-85d4-7faf1d6c3a79.png)

## Transform

- The "review_id_df" DataFrame is created with the appropriate columns and data types
- Null values are removed

![spark3](https://user-images.githubusercontent.com/113717031/224580963-2b2bbbe7-944f-4a54-9d5e-161958101644.png)

![spark4](https://user-images.githubusercontent.com/113717031/224580976-0bc8e6ee-4bda-495b-aa38-8e8168ae3c7a.png)

- The "products_df" DataFrame is created and the the duplicate values are dropped
- The "customers_df" DataFrame is created and displays the number of times a customer reviewed a product grouped by the "customer_id"

![spark5](https://user-images.githubusercontent.com/113717031/224580987-f5352b9b-8999-4be5-b760-c635e4eab85e.png)

- The "vine_df" DataFrame is created that has the "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns

![spark6](https://user-images.githubusercontent.com/113717031/224581000-c7cb561f-c4f9-4cbe-a7ce-ccc5e0f722bc.png)

## Load

- The four DataFrames for each dataset are successfully loaded into an RDS instance

![spark7](https://user-images.githubusercontent.com/113717031/224581446-36f2acc2-bf09-49cc-83c8-262fb14f50a8.png)
