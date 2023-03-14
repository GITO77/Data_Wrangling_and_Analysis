#  Data Wrangling and Analysis
## by Greatness Okeremeta


## Dataset
>The project makes use of 3 datasets: Enhanced Twitter Archive, Additional Data via the Twitter API and an Image Predictions File which is a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction. The Twitter archive belongs to the user @dog_rates, also known as WeRateDogs. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.


## Project Motivation
>The goal of the project is to wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. There are 6 steps carried out in the project:
- Step 1: Gathering data
- Step 2: Assessing data
- Step 3: Cleaning data
- Step 4: Storing data
- Step 5: Analyzing, and visualizing data
- Step 6: Reporting data wrangling efforts, data analyses and visualizations


## Project procedure
>All three pieces of data were gathered in the wrangle_act.ipynb notebook through different means. Each piece of data was imported into a separate pandas DataFrame at first. Subsequently, they were assessed visually and programmatically for quality and tidiness issues which are documented in the wrangle_act.ipynb notebook also. All the identified issues were cleaned after making a copy of the original data. During cleaning, I used the define-code-test framework to document my actions. The individual pieces of data were merged according to tidy data rules and this resulted in a high-quality and tidy master pandas DataFrame.

> The cleaned master DataFrame was stored in a CSV file named twitter_archive_master.csv. I wrote a 600 word written report called wrangle_report.pdf that briefly describes my wrangling efforts. Subsequently, I compiled another report called act_report.pdf that communicates all the insights and displays the visualizations produced from my wrangled data, this was framed like a blog post.

## Key insights
> The tweets that categorized dogs as 'doggo and puppo' received the most likes on an
average basis more than the other dog types followed by puppos and doggos individually
with pupper being the least desirable dog type. This finding is fully supported by the fact
that the highest retweeted tweet belonged to a doggo while the most favorited tweet
belonged to the puppo dog type.

>  A strong positive correlation was observed between retweet_count and favorite_count
with a correlation coefficient of 0.9. The more a tweet was retweeted, the more it was
liked/favorited.

> Out of all the predicted dog types, the golden retriever emerged as the one with the most
predictions as it had 135 out of the 1453 predictions that were made, it was followed by the
labrador retriever with 91 predictions. The least predicted dog types were the
scotch_terrier, entlebucher, groenendael japanese spaniel, clumber,
standard_schnauzer and silky terrier , with each one having 1 prediction.
