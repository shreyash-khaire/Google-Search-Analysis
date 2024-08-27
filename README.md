# Python-Google-Search-Analysis

Pytrends API
Pytrends is an unofficial Google Trends API called pytrendsoffers several ways to retrieve information from popular searches from Google Trends. With the aid of the python module, you may speed up the process of automating data retrieval. It is useful to examine and compile a list of the top Google search results for a given topic broken down by geographical location and language.

### Installing pytrends

We must first install this API on our computer before using it.

```python
pip install pytrends
```
### Importing libraries and connecting to Google

Pandas must first be imported in order to generate a dataframe. The function TrendReq from the pytrends.request the library must be imported in order to connect to Google and request the Google trending topics. We will load matplotlib as well, in order to visualize the data.

![Connect to Google](https://github.com/user-attachments/assets/dc2db23f-9e10-44e7-866d-2d282b78b7a3)

`hl` represents the hosting language for accessing Google Trends, we set it to English. 
`tz` represents timezone, we use the US time zone (represented in minutes), which is 360.


### Building payload

To create a list of terms for Google Trends searches, use the build_payload function from pytrends. Additionally, you may define the category and timeframe for data collection.

![Build Payload](https://github.com/user-attachments/assets/a415ce9e-5f7b-4f7a-b03f-176edcb938a0)

### Daily search trends

Let's now look at the top daily search trends globally. The trending_searches() function will be used for this. Simply enter no parameters if you wish to search globally.

```python
# Google Trends data
df=Trending_topics.trending_searches(pn="india")
df.head(10)
```

### Interest over time

![Interest Over Time](https://github.com/user-attachments/assets/328cd286-deee-4ea7-bb3e-63033f4ef8ce)

### Interest by region

Let's look at some of the most often used regional terms around the globe.

![Interest By Region](https://github.com/user-attachments/assets/d4fad8b2-bf12-43fb-a739-ccab24f357d0)

### Top charts

We can obtain the most popular searches each year using this technique. So let's look at the most popular search terms in 2020.

![Top Charts](https://github.com/user-attachments/assets/95c3d6c5-f229-4630-84bc-e499e0cd4f80)

### Related queries

![Related Queries](https://github.com/user-attachments/assets/64d847c7-e74a-4927-b9d0-d282a2ac75fe)

### Keyword Suggestions

Google Trends may provide you with a list of suggested keywords that are related to your primary keyword.

![Keyword Suggestions](https://github.com/user-attachments/assets/ed2aeb07-dec6-4378-8b31-ee552a3f561f)







