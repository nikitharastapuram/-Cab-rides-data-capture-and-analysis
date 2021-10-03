# Cab-rides-data-capture-and-analysis

**PROBLEM STATEMENT**

 ‘YourOwnCabs’ (YOC) is an online on-demand cab booking service. Initially it was doing around 100 rides per day. Owing to a successful business model and excellent service, the company’s business is growing rapidly, and these numbers are breaking their own records every day. YOC’s customer base and ride counts are increasing on a day-by-day basis. 
It is highly important for business stakeholders to derive quick and on-demand insights regarding the numbers to decide the company’s future strategy. Owing to the massive growth in business, it is getting tough for the company’s management to obtain the business numbers frequently, as backend MySQL is not capable of catering to all types of queries owing to large volume data.The company’s major focus is to provide its customers a delightful experience while ensuring zero downtime. Also, business stakeholders should be catered with all the answers that they require that are backed by data. Data-driven decisions play a steroid role for a fast-growing start-up.


**EXTRACTION OF DATA**
Wrote a job to consume clickstream data from Kafka and ingest to Hadoop. (Stream Data)
Wrote a job to ingest the bookings data from AWS RDS to Hadoop. (Batch data)

**TRANSFORMATION**
Created aggregates for finding total bookings date-wise using Spark script.

**SET UP FOR ANALYSIS**
Created a Hive-managed table for clickstream data.
Created a Hive-managed table for bookings data.
Created a Hive-managed table for aggregated data.

**LOAD**
Loaded data into hive tables using HiveQL

**ANALYSIS**
1. Calculate the total number of different drivers for each customer.
2. Calculate the total rides taken by each customer.
3. Find the total visits made by each customer on the booking page and the total ‘Book Now’ button presses. This can show the conversion ratio.
The booking page id is ‘e7bc5fb2-1231-11eb-adc1-0242ac120002’.
The Book Now button id is ‘fcba68aa-1231-11eb-adc1-0242ac120002’. You also need to calculate the conversion ratio as part of this task. Conversion ratio can be calculated as Total 'Book Now' Button Press/Total Visits made by customer on the booking page.
4. Calculate the count of all trips done on black cabs.
5. Calculate the total amount of tips given date wise to all drivers by customers.
6. Calculate the total count of all the bookings with ratings lower than 2 as given by customers in a particular month.
7. Calculate the count of total iOS users.
