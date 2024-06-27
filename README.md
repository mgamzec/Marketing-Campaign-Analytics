![image](https://github.com/mgamzec/Marketing-Champaign-Analytics/assets/62151645/ea76a014-e13b-40ec-a4f0-de67ce5349f1)
# Marketing-Champaign-Analytics

## Was the campaign successful?
As a data professional, you will often find yourself translating business questions into measurable outcomes. One of the most common questions you might be asked is, "Was the campaign successful?". At first, this might feel like an intimidating question. There are so many ways one could measure campaign success! That said, there are a few kinds of metrics you will find yourself using over and over again. For a marketing team, campaign success is typically measured by conversion rate. This is to say, of all the people who came into contact with your marketing campaign, how many bought the product? Depending on the business, this could mean that a person made a purchase or subscribed to your service. In addition, many subscription businesses care about retention. Once a user has signed up for a subscription, are they still a subscriber one, three or twelve months in? This metric can be particularly difficult to measure because it requires patience. We can't know 90-day retention rates until 90 days have passed since a user initially subscribed.

## Conversion rate
Conversion rate is the percentage of people that we market to who ultimately convert to our product. In this course, we will be focusing on a subscription service and will be talking about conversion in terms of subscriptions.

![image](https://github.com/mgamzec/Marketing-Champaign-Analytics/assets/62151645/bc6b430e-eeac-4df2-bee8-cefe2f8c6fd9)


## Calculating conversion rate using pandas
To calculate the total number of people who converted, we slice the DataFrame to include only the rows where "converted" equals True and then count the unique user_ids using nunique(). Next, we calculate the total number of people we marketed to. We can do this by counting all the unique user IDs in our dataset. Now that we have the total number of users and users who subscribed, we can calculate conversion rate by dividing subscribers by total.

## Retention rate
Retention rate is the percentage of people that remain subscribed after a certain period of time. In this course, we will focus on 1-month retention.
![image](https://github.com/mgamzec/Marketing-Champaign-Analytics/assets/62151645/2e5668f3-1c97-4a39-85af-77508bc0bd09)


## Calculating retention rate
To determine retention rate, we first calculate the total number of users who remain subscribers after one month. This information is available in the column "is_retained". We now slice the DataFrame to include only rows where the user was retained, that is, where is_retained equals True and count the unique user_ids. We can reuse our "subscribers" calculation from the conversion rate calculation, as the number of total users who originally subscribed remains the same. Finally, we divide the number of users who were retained by the number of users who subscribed to calculate the retention rate.
