# DATA 115 Personal Dataset project on Hops


## Motivation: 
   My motivation is pretty simple I enjoy plants and agriculture. When I am driving country roads it's fun seeing farms and the different techniques of how different plants are grown in large quantities. I especially enjoy seeing hops plants because they are vines that are suspended upward by 25 foot poles that creates an amazing canopy. I also like beer, and since Washington State is also known for it's hoppy beer I got curious about where the hops come from. That is when I discovered that almost all of the hops grown in the United States were grown in only 3 states, Washington, Oregon and Idaho. Which got me to thinking, if I wanted to grow an acre of hops, in what state and what type would I need to grow in order for that acre to be the most profitable? 

## Data Process: 
   I found my data at the USDA's website https://usda.library.cornell.edu/concern/publications/s7526c41m where I downloaded the csv files with the data from 2018-2020 production of different types of hops, yield and prices of hops grown in Idaho, Oregon, and Washington. 
   In order to work with the data effectively, I needed to rearrange some columns in the excel worksheets so that each year went to individual columns next to each other in the file. I also erased any cells that had (D) or (NA) because they had no useful information and made the calculations in rstudio difficult. I merged the price per lb information from the Hops Price Table to add price columns for each year. I also erased rows that had more then one type of hop since I wanted to know what the highest grossing singular type was. I then created the Gross Profit column for each year by multiplying the yield per acre column by price column. This gave me the information I needed to work with in order to create the visuals below. After the data manipulation I uploaded this CVS file https://github.com/chanzy314/Hops_School_Project/blob/main/Hop%20Data%20with%20Prices.csv to rstudio and made my evaluations. 


## Analytical Technique: 

The biggest thing I learned while doing this assignment was to map out what I was planning to do. While I was working with the data, I had assumed the the greatest yield per acre automatically meant the greatest profit and failed to take in consideration the price. Which is why I made the new column in my data set. 

<table>
<tr><th> 2018 Price/lb </th><th>2019 Price/lb </th><th>2020 Price/lb </th></tr>
<tr><td>

| State | Price |
| --- | --- |
|ID|	5.30|
|OR	|5.40	| 
|WA| 5.50	| 


</td><td>

| State | Price |
| --- | --- |
|ID|	5.25|
|OR	|5.50	| 
|WA| 5.80	| 

</td><td>

| State | Price |
| --- | --- |
|ID|	5.80|
|OR	|6.00	| 
|WA| 6.00	| 

</table>

This is evident in the scatterplot below for 2019 gross profit lines.

![image](https://user-images.githubusercontent.com/61097093/115101153-aefea700-9ef6-11eb-99ae-31738decfba7.png)

With the year 2020 having the most equality in price of the three years I assumed that would be the best data to find the best profit per plant. This turned out not to be the case due to enviromental conditions. Washington state had massive wildfires that destoyed fields across the state. The top yield per lbs in 2019 was 3216 lbs vs 2801 lbs in 2020. That's about a 13% decrease. Which explains the profit "jump" for Idaho and Oregon even though those states still made less then the previous years top contributors. 

![image](https://user-images.githubusercontent.com/61097093/115972749-19ba6e80-a505-11eb-81fe-367b0a066593.png)

With this in mind I checked the previous years enviromental factors for the other states to make sure there were no other inconsistencies. At this point I realized that my first instinct to check yield per acre for each plant would be my best chance to finding the most profitable plant, keeping in mind that 2020 will have skewed values.  

Below are the 3 years by the top ten yield producers.
<table>
<tr><th> 2018 Top Ten </th><th>2019 Top Ten </th><th>2020 Top Ten</th></tr>
<tr><td>

| State | Type | Yield Per Acre|
| --- | --- | --- |
|WA|	Bravo TM	|3258		|
|WA|	Super Galena TM|	3133|		
|WA|	Eureka! TM	|2954		|
|WA|	Apollo TM	|2848		|
|ID|	Zeus 1/	|2764		|
|WA|	Ahtanum TM|	2730	|	
|WA|	Zeus 1/|	2619		|
|WA|	Ekuanot R|	2583	|	
|ID|	Super Galena TM|2493|		
|WA|	Azacca TM, ADHA-483|	2491|	


</td><td>

| State | Type | Yield Per Acre|
| --- | --- | --- |
|WA|	Bravo TM	|3216	|	
|WA|	Eureka! TM|	3188|		
|WA|	Super Galena TM|	2871|		
|WA|	Ahtanum TM|	2820		|
|WA|	Apollo TM	|2735		|
|ID|	Zeus 1/	|2672		|
|WA|	Zeus 1/	|2620		|
|OR|	Super Galena TM |2580|		
|ID|	Idaho 7 TM	|2562		|
|WA|	Palisade R|	2520	|

</td><td>

| State | Type | Yield Per Acre|
| --- | --- | --- |
|OR|	Super Galena TM|	2801|		
|WA|	Super Galena TM|	2636	|	
|ID|	Idaho 7 TM|	2442		|
|OR|	Amarillo R |	2360	|	
|ID|	Mosaic R |	2335		|
|WA|	Eureka! TM	|2332		|
|WA|	Bravo TM	|2308		|
|OR|	Liberty	|2289		|
|WA|	Apollo TM	|2248	|	
|WA|	Ekuanot R |	2158	|

<tr><td></table>

## Visualization: 

I created another excel spreadsheet from the information above to use in rStudio to make my visualization. This time I used the mean of the yield per acre from 2018-2020 from the top 10 plants in order to find the highest yielding plant. 

![image](https://user-images.githubusercontent.com/61097093/115976637-d1ab4400-a524-11eb-97ab-d39885d2a362.png)


## Conclusion:

If you were to grow an acre of hops and you wanted the highest profit for that acre, as of now the greatest yields per state are Bravo in Washington, Super Galena in Oregon and Zues 1 Idaho.      



