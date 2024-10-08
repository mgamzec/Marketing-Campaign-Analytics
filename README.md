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

# Summary
1. Dataset
We analyzed a marketing campaign from start to finish. Importing the dataset and used the head(), info(), and describe() methods to assess the contents and quality of the dataset.

2. Preprocessing
Next, practiced feature engineering by creating a new columns and corrected an errors in the data.

3. Marketing metrics
Then looked at high-level metrics like conversion and retention rates.

4. Customer segmentation
After had a handle on the marketing metrics, practiced user segmentation. For example, looking at how different marketing channels reach different age groups.

5. Dip in conversion rate?
Next, you dealt with one of the most common challenges in marketing. Something went wrong in the campaign, and it was your job to identify the problem and assess the impact of the mistake. You successfully found the cause, which was a language mismatch.

6. Analyzed an A/B test
Finally, analyzed an A/B test. How to determine statistical significance and the importance of segmentation in A/B tests to understand the true impact of the change. You found that while the test was a success overall, personalization was not appreciated in certain regions and by certain age groups.
