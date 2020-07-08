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
I merged the top 20 most frequently used bigrams, and the top 40 most frequently used grams to our dataset.I used it as a feature for prediction of total_net_revenue.The feature decribes the no of times a title has the corresponding grams or bigrams.

This way, we can measure the relationship of title language on our net revenue. 
Thus, allowing hosts to phrase their listing in the best way possible, in hopes to maximize profits.
Top 6 most used bigrams:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/Screenshot%202020-07-08%20at%206.18.43%20PM.png)


Dataset with top 20 bigrams nad top 40 grams in title listing names:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/Screenshot%202020-07-08%20at%206.19.32%20PM.png)

Measuring Effectiveness of certain words in title listings on total revenue:

private bathroom:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/private_bathroom.png)


cozy:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/cozy.png)

Loft:
![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/loft.png)
Inferences:
These plots suggest that in Queens those that list a title with the words 'private bathroom' appear to bring in a higher Net Revenue.
It also suggests that in the Bronx, those that list a title with the word 'cozy' appear to bring in a higher Net Revenue; while in Manhattan, listings with 'cozy' are not performing as well.
And if I ever lease a place on Airbnb in Manhattan or Brooklyn, I should put 'loft' in the title!

![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/title_effects.png)

![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/brooklyn_model_factors.png)


![alt text](https://github.com/Roshni96/Airbnb_host_revenue_analysis/blob/master/manhattan_model_factors.png)

Conclusions:
The text that you put in your Airbnb DOES matter, and it varies across what region you are located in. It is important to include specific text, espcially if your property contains it.
if you're near Central Park - put that in the title! (Referencing above)
The most impactful factors we are missing - REVIEW RATINGS
If you're a high rated lister, and your property is also highly rated, you are most likely going to succeed in obtaining a larger net revenue.



