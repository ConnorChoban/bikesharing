# Overview of Analysis

The purpose of this analysis is to examine the Citi Bike rider data in New York City to gain valuable insights into who our primary customers are. We'll use this information to create a preliminary analysis for when we implement the same service in Des Moines. 

## Results

Note: the story for this module can be found here: https://public.tableau.com/app/profile/connor.choban/viz/CitiBikeDataProject-CC/TripData


### Checkout Times for Users

By looking at the chart below, we see that the vast majority of bike users rent their bike for less than an hour, with the greatest amount of users renting for only 0-30 minutes. This means that most customers are only using the bikes for a very short period, and might be using them to cross short distances in the congested neighborhoods of NYC. Thus we should adjust our business strategy accordingly, allowing users to quickly check out a bike, and facilitating multiple rentals per day. 

<img width="1294" alt="Screen Shot 2022-05-28 at 10 43 34 PM" src="https://user-images.githubusercontent.com/99847786/170893065-b1b09ffd-6b41-44f0-ab46-eda13a21d19a.png">

### Checkout Times by Gender

In the chart below, we see that men represent a far greater share of the customer base than women, while the duration of the rental is similar between both sexes. For comparison, for rides lasting 5 minutes, the amount of male users was 108,087 whereas the amount of female users was 33,041, while users of an unknown sex constituted 5,624 riders. This means that men are more than 3x as likely to rent a bike, and in theory would form the bulk of our customer base. However, I find it very unusual that there's such a huge gender gap, and would like to explore this further to understand if there's some cultural dynamic or other factor responsible. 

<img width="1298" alt="Screen Shot 2022-05-29 at 2 32 36 AM" src="https://user-images.githubusercontent.com/99847786/170893067-db886931-5c5d-4eb3-bc2b-bea4ef1f2a33.png">

### Trips by Weekday

In the heatmap below, we can examine the average bike usage by hour and day of the week. We can see two trends emerging from the data. One, the majority of rides during the weekdays are concentrated from 5 AM to 9 AM, and even more so from 4 PM to 8 PM. If we believe that users are renting bikes in order to commute, then it would make sense that the majority of rides are concentrated around these hours as they follow a traditional 9 to 5 work schedule. Also, note that the number of rides is more evenly spread out on Friday. This may be due to workers leaving their jobs early to take advantage of the weekend.

Second, from 8 AM to 8 PM on Saturday and Sunday rentals are more evenly distributed, which may indicate that users are riding for leisure rather than transportation. 

In any case, if there's a need to perform maintenance on the bikes, it would be ideal to avoid these peak hours, and agend repairs for either the early morning, or during the mid-day drop in usage from 10 AM to 12 PM

<img width="1269" alt="Screen Shot 2022-05-29 at 3 17 04 AM" src="https://user-images.githubusercontent.com/99847786/170893069-0dbe9b40-4f40-4c5c-8dbf-6dc3bb0f4de9.png">

### Trips by Gender

From the data in this heatmap, we can arrive to the same conclusions made in the Checkout Times by Gender and Trips by Weekday charts. As we noted before, men are much more likely to rent a bicycle than women, and both sexes tend to rent bikes around the same time of day. What stands out is that in the third panel we can see that users are less likely to inform their gender on the weekends, as there's an uptick in the amount of rides by an unknown gender on Saturday and Sunday.

<img width="1330" alt="Screen Shot 2022-05-29 at 3 23 41 AM" src="https://user-images.githubusercontent.com/99847786/170893072-d6a7e29d-075b-42cb-ae97-a3e06ef69a13.png">


### User Trips by Gender by Day

This chart summarizes the data in the two previous heatmaps but separates subscribers and customers. We can see that new or unsubscribed customers from a greater porportion of renters on the weekends than during weekdays, whereas subscribers tend to form a much greater porportion during the week, with the bulk of rentals ocurring from Monday-Tuesday, and Thrusday-Friday, with a noticeable gap on Wednesday. It might be worth it to investigate why there's a drop in rentals on Wednesday.

<img width="1324" alt="Screen Shot 2022-05-29 at 3 37 43 AM" src="https://user-images.githubusercontent.com/99847786/170893076-4e0bd2ed-549e-4532-962b-51dc9e7eb104.png">

<img width="1172" alt="Screen Shot 2022-05-29 at 10 15 40 PM" src="https://user-images.githubusercontent.com/99847786/170915059-f6cfa7dc-33ce-4613-8e70-9c72b1731f60.png">


### Bike Usage

In the visual below, we can see which bikes are being used the most and which ones are being used the least. This is helpful for us to tell which bikes will need to be maintained and replaced more frequently, and can help us calculate the total cost of maintainence, amortization, and replacement of bicycles. The average amount of total rides per bike is around 200, while some bikes have been used nearly 400 times, and others less than 10. This also helps us to see which areas have the highest demand, although a map would be better for this. 

<img width="1341" alt="Screen Shot 2022-05-29 at 8 43 59 PM" src="https://user-images.githubusercontent.com/99847786/170898722-b50f6fe0-d16b-4fde-8b24-b6133e6b40c6.png">

### Number of Rides by Day

Finally, in the chart below we see the total amount of rides per day. This can help provide valuable insights into which days have the highest demand. I filtered the y axis of the chart so that only values above 50,000 are displayed in order to better viusalize the data. By looking at usage in a bar chart, it can help us see how much of a difference in usage there is in a quantitative form. This way, we can see the stark contrast between certain days of the month. For example, on 08/06 there were 82,515 rentals. The next day, on 08/07, there were only 52,193, so there was a noticeable drop for some reason. We could investigate and try to understand why demand dropped on this day, and adjust our strategy accordingly. 

<img width="1343" alt="Number of Rides by Day" src="https://user-images.githubusercontent.com/99847786/170899732-252e298c-e6b4-4c2d-8a13-e91fa9765d44.png">


## Summary

By analyzing the data, we can come to a few key conclusions. 

- Men are far more likely than women to rent a bicycle, so it would stand to reason to either focus marketing efforts on accomodating men, or conversely focus efforts on attracting more women to rent a bicycle. 

- The majority of rentals happen during weekday morning hours (from 5AM to 9 AM), and afternoon and evening hours (from 3 PM to 8 PM). Thus it may be wise to provide additional bicycles to meet demand, and agend repairs for outside this time block. 

- The majority of rentals are short in duration, with more than half being 20 minutes or less. Therefore, we should adjust our business strategy to accomdate shorter rental periods. 

Two additional visualizations that could be used with this data set could be a map showing which areas have the highest rental rates, such as the one we created in this module. We could also use a heatmap or bar chart to evaluate the relationship between age and the number of users. 
