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
