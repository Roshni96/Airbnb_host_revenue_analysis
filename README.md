# Airbnb_host_revenue_analysis
Maximising profits for airbnb host using NLP and Machine Learning

I measured the financial performace of each listing using KPI's- no of reviews,minimum nights and price of listing.
The response variable is total_net_revenue=[number_of_reviews] x [price (USD)] x [minimum_nights].

Count of Listings by Borough:

![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/plot_listings_by_borough.png)

Manhattan contains the most amount of listings; additionally, it looks like it is the most expensive.

Next,Brooklyn appears to be next popular; however,with a more reasonable distribution of price listings. High - Very High seem to only take up 20% of the population.

Queens has only 5000 listings, and appears very cheap.

Lastly, the Bronx & State Island do not appear very popular for Airbnb.


Count of Listings by Room Type:

![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/count_of_listings_roomtype.png)

Worcloud of HIgh Priced Airbnb listings:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/wordcloud_high.png)

We can see that title names that contain 'loft','village','central park' are more likely to be highly priced.

Worcloud of Low Priced Airbnb listings:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/wordcloud_low.png)

We can see that title names that contain 'cozy','private','bedroom' are more likely to be low priced.

I used NLP to break out the Titles of the Listings into grams and bigrams.
I merged the top 20 most frequently used bigrams, and the top 40 most frequently used grams to our dataset.

This way, we can measure the relationship of title language on our net revenue. 
Thus, allowing hosts to phrase their listing in the best way possible, in hopes to maximize profits.
