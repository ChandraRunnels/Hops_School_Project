# DATA 115 Personal Dataset project on Hops


## Motivation: 
   My motivation is pretty simple I enjoy plants and agriculture. I enjoy driving country roads seeing farms and the different techniques of how different plants are grown in large quantities. I especially enjoy seeing hops plants because they are vines that are suspended upward by 25 foot poles that creates an amazing canopy. I also like beer, and since Washington State is also known for it's hoppy beer I got curious about where the hops come from. That is when I discovered that all of the hops grown in the United States were grown in only 3 states, Washington, Oregon and Idaho. Which got me to thinking, if I wanted to grow an acre of hops, in what state and what type would I need to grow in order for that acre to be the most profitable? 

## Data Process: 
   I found my data at the USDA's website https://usda.library.cornell.edu/concern/publications/s7526c41m where I downloaded the csv files with the data from 2018-2020 production of different types of hops, yield and prices of hops grown in Idaho, Oregon, and Washington. 
   In order to work with the data effectively, I needed to rearrange some columns in the excel worksheets so that each year went to individual columns next to each other in the file. I also erased any cells that had (D) or (NA) because they had no useful information and made the calculations in r difficult. I merged the price per lb information from the Hops Price Table to add price columns for each year. I also erased rows that had more then one type of hop since I wanted to know what the highest grossing singular type was. I then created the Gross Profit column for each year by multiplying the yield per acre column by price column. This gave me the information I needed to work with in order to create the visuals below. 


#Visualization: 
Choose and construct a single visualization to summarize and represent your data.








• Analytical Technique: Apply one of the techniques that we have covered in the course to your
dataset and provide an analysis of the results. You can choose from either among the exploratory data
analysis topics or from the techniques we cover later in the course


<table>
<tr><th>2018 </th><th> 2019 </th></tr> 2020 </th></tr>
<tr><td>

| State | Type | Gross Profit|
| --- | --- | --- |
|Washington|	Bravo TM |	17919.0	|	
|Washington	|Super Galena TM	| 17231.5	|	
|Washington	| Eureka! TM	| 16247.0		|
|Washington	| Apollo TM	|15664.0		|
|Washington|	Ahtanum TM, YCR 1	|15015.0|		
|Idaho	|Zeus 1 |	14649.2		|
|Washington	|Zeus 1|14404.5	|	
|Washington	|Ekuanot R, HBC 366	|14206.5	|	
|Washington|	Azacca TM, ADHA-483|	13700.5	|	
|Washington	|Palisade R, YCR 4	| 13425.5	|


</td><td>

| State | Type | Gross Profit|
| --- | --- | --- |
|Washington|	Bravo TM	|18652.8		|
|Washington|	Eureka! TM|	18490.4		|
|Washington|	Super Galena TM	|16651.8	|	
|Washington|	Ahtanum TM, YCR 1	|16356.0|		
|Washington|	Apollo TM	|15863.0	|	
|Washington|	Zeus 1/	|15196.0		|
|Washington|	Palisade R, YCR 4|	14616.0	|	
|Washington|	Ekuanot R, HBC 366	|14401.4	|	
|Washington|	Azacca TM, ADHA-483	|14157.8	|	
|Idaho|	Zeus 1	|14028.0	|

</td></tr> 

| State | Type | Gross Profit|
| --- | --- | --- |
|Oregon|	Super Galena TM|	16806.0	|	
|Washington	|Super Galena TM	|15816.0|		
|Idaho	Idaho 7 TM	|14163.6	|	
|Oregon	|Amarillo R, VGXP01	|14160.0	|	
|Washington|	Eureka! TM|	13992.0		|
|Washington|	Bravo TM|	13848.0		|
|Oregon	|Liberty|	13734.0		|
|Idaho	Mosaic R, HBC 369|	13543.0|		
|Washington	|Apollo TM	|13488.0	|	
|Washington	|Ekuanot R, HBC 366	|12948.0	|


<tr><td></table>

• Presentation: In the final week of class, you will give a three minute presentation3 about your
dataset and repository


