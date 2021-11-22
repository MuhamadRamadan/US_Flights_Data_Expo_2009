# US Flights - Data Expo 2009
## by Mohamed Ramadan


## Dataset

> The data consists of flight arrival and departure details for all commercial flights within the USA, from October 1987 to April 2008. This is a large dataset: there are nearly 120 million records in total, and takes up 1.6 gigabytes of space compressed and 12 gigabytes when uncompressed.
As the data is huge, I decided to explore the period from 2007 to 2008. Further, I am going to work on a sample of the data to speed up the computation [link](https://community.amstat.org/jointscsg-section/dataexpo/dataexpo2009).
Also, I have used Carrier information csv file downloaded from [Bureau of Transportation Statistics](https://www.transtats.bts.gov/DL_SelectFields.asp?gnoyr_VQ=FMF&QO_fu146_anzr=Nv4%20Pn44vr45)
> The dataset was cleaned by:
>1. Removing duplicated rows.
>2. Dealing with missing values by various techniques: deleting, filling Zeros, filling values by understanding the feild of the dataset, and also by using interpolation.
>3. Changing Data types


## Summary of Findings

>1. Slight decrease in the proportion of flights during 2008 compared to flights during 2007.
>2. Top five carriers:
    > a. Southwest Airlines Co.(WN)
    > b. American Airlines Inc.(AA)
    > c. SkyWest Airlines Inc. (OO)
    > d. Envoy Air (MQ)
    > e. US Airways Inc.(US)
>Interestingly, Southwest Airlines number of flights is almost doubled compared to American Airlines which comes in the second rank. 
>3. 97.9% of flights were operated while only 2.1% of flights were cancelled.
>4. The most common reason for flights cancellation is **Carrier** with a percent of 40.4% followed by **Weather** with a percent of 39.5%.
>5. Diverted flights percent is very small (0.2 %) compared to non-diverted fligths.
>6. All features (ActualElapsedTime, CRSElapsedTime, AirTime, ArrDelay, DepDelay, Distance) distributions are right-skewed with a lot of outliers. Axis limitation was used to take a closer look at the underlying patterns in the data.  
>7. Flights distances was showing right-skwed distribution with a lot of outliers. After applying log transformation on x-axis, the distribution converted to normal-like distiribution. 
>8. Average distance of not-cancelled flights is higher (700 miles) than average distance of the cancelled flights (600 miles). The flights with more than 1000 distance is more likely to be not cancelled.
>9. **Envoy Air** occupies the first place in the list with 4 % cancellation rate followed by **Mesa Airlines Inc.** while **Frontier Airlines Inc.** comes at the end of the list.  
>10. the common reason of cancelling **Envoy Air** flights was the **Weather** and not **Carrier** as I was expected. **American Airlines Inc.** comes after **Envoy Air** with the number of cancelled flights due to weather.  
While, **Mesa Airlines Inc.** cancelled flights was mainly beacuse of the **Carrier** itself.


## Key Insights for Presentation

> Flight cancellation investigation.