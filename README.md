                                            ##Overview of the analysis

We have access to approximately 50 Amazon Vine review datasets in this project. Among them, we chose the baby product review dataset. We used PySpark to perform the Extract, transform the data, connect to an AWS relational database instance and load the transformed data into an SQL database. We used PySpark to review bias toward favorable reviews from members.

Below is an example using ELT process on the Amazon baby products reviews as well as utilizing PySPark platform.

![](https://github.com/smzd/Amazon_Vine_Analysis/blob/main/Resources/vine.png)
Fig: Vine Dataframe


                                                  ##Results
                                                    
 ![](https://github.com/smzd/Amazon_Vine_Analysis/blob/main/Resources/percent.png)
 Fig: Total Ratings
                                                    
•	How many Vine reviews and non-Vine reviews were there?

Total Vine Reviews are 463. Total Non-Vine Reviews are 25079.

•	How many Vine reviews were five stars? How many non-Vine reviews were five stars?

202 Vine reviews were five stars. 12028 Non-Vine reviews were five stars.

•	What percentage of Vine reviews were five stars? What percentage of non-Vine reviews were five stars?

43.62% of Vine reviews were five stars. 47.96% of non-Vine reviews were five stars.


                                               ##Summary
                                                      
A positive bias refers to a tendency to hold positive expectations. Total vine reviews were 1.85%, much smaller than non-vine reviews. When we analyzed the percentage of 5 stars reviews, the numbers are similar; both vine and non-vine reviews are below 50%. We can conclude that there is no evidence of positive bias.

Additionally, we should dig deeper into 1,2,3,4 stars reviews for both Vine and Non-Vine reviews. We can store all 1-5 star data into data frames, utilize summary statistics to get the P value for each star, and plot them accordingly to get more detailed results of the reviews.
