# coffeeshop
After initial assessment of the data, the results are as follows:
claim_id: Contains nominal value. There were 2000 unique claim ids. There is no missing value. All criteria are met.
time_to_close: Contains discrete value. All values are positive, as expected. Both criteria are met.
claim_amount: Contains continuous value. Some values did not round to 2 decimal places. Values do not all match the description.
amount_paid: Contains continuous value. Some values did not round to 2 decimal places. Values do not all match the description.
location: Contains nominal value. There were 4 unique locations, which are “RECIFE”, “SAO LUIS”, “FORTALEZA”, or “NATAL”. All criteria are met.
individuals_on_claim: Contains discrete value. There is a minimum of 1 person, as expected. Both criteria are met.
linked_cases: Contains nominal value. Contains either True or False. Both criteria are met.
cause: Contains nominal value. There are also "VEGETABLES" and " Meat", besides “vegetable”, “meat” and “unknown”. Values do not all match the description.

There is no missing value in columns claim_id, time_to_close, claim_amount, location, individuals_on_claim, and cause. The amount_paid column has 36 missing values. The Linked_cases column has 26 missing values.

To make values match the description, the following actions were taken:
claim_amount: All values are rounded to 2 decimal places.
amount_paid: All values are rounded to 2 decimal places, and missing values are replaced with the overall median amount paid.
cause: "VEGETABLES" is replaced with “vegetable”, and " Meat" is replaced with “meat”.

<img width="539" alt="1" src="https://user-images.githubusercontent.com/122923021/224200141-d76c964c-69ab-4e45-8f49-8d479db96946.png">
As we can see from the bar graph above. Recife has the most observation, which is 885. The observations are not balanced across categories. For example, Recife's observations are almost 4 times as much as that of Natal.

<img width="508" alt="2" src="https://user-images.githubusercontent.com/122923021/224200287-646da369-cca7-4677-823e-e53ee847acf6.png">
As we can see from the histogram above, most of the time to close observations are distributed between 160-180. The distribution is right skewed with some outliers but most of time to close is below 300.

<img width="516" alt="3" src="https://user-images.githubusercontent.com/122923021/224200327-348b0711-c385-4412-aaa9-226fde7ce4e0.png">
As we can see from the scatter plot and the trend line above, the claim amount has a positive correlation with time to close, which means when the claim amount is large, time to close tend to be larger as well. Also, we can tell from the scatter plot above, when the claim amount gets larger, time to close range gets larger too.

The median time to close of the Fortaleza, Natal, Recife, and Sao Luis are 180, 179, 178, and 179, respectively. As we can see through the first box plot below, the time to close among four locations are very similar. Although, there are outliers (as shown in purple circles) among all four locations, in the second graph below, we removed the outliers to better compare the data between each location. All four locations’ interquartile ranges are very close, with Fortaleza having the highest median (i.e. 179) and Recife having the lowest median (i.e. 176).
<img width="607" alt="4" src="https://user-images.githubusercontent.com/122923021/224200367-b8738c80-b130-4f75-b0fb-b3cf9022358f.png">
<img width="610" alt="5" src="https://user-images.githubusercontent.com/122923021/224201016-dfe8a13b-f3cf-471b-b274-cf700be7f287.png">

