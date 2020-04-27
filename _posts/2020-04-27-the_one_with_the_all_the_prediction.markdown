---
layout: post
title:      "The One with all the Predictions"
date:       2020-04-27 15:22:10 +0000
permalink:  the_one_with_all_the_predictions
---


### April 2020

I reached the second milestone in my Data Science Online Course: the end of the second “module” and its end-of-module project.<br>
This time it was about linear prediction and I was tasked with predicting house prices from house characteristics.<br>
In Data Science jargon, the characteristics should be called independent variables, predictors or features, and the house price, dependent variable or target variable.<br>
The features I ended up using were:

* size of the lot,
* living area apart from basement,
* total living area,
* total living area average of the 15 closest houses,
* latitude,
* construction grade,
* number of bedrooms,
* number of bathrooms,
* number of floors,
* whether it was a waterfront house or not.

My results ended up being relatively good even if I wished I would have spent more time investigating polynomial regression and interactions between features.<br>
But, rather than the performances of my model, I would like to discuss a potential assumption behind all this exercise.<br>
Maybe it is not an assumption, maybe it is more of a mindset.<br>
I think it is easy to get carried away and believe that it is actually possible to predict a house price only from tangible features like the ones listed above.<br>
What I mean is: Yes, it is possible to build a prediction model that minimizes the errors for the data we collected.<br>
Yes, for a given house, the prediction will be pretty close to the actual selling price.<br>
But no, we can't predict exactly the price a given house will be sold in the future.<br>
Maybe the project should not describe the target variable as a "price", but rather as a "market value".<br>
My point is that the predictable market value of a house can be different from its price.<br>
It seems to me that there is an abundance of intangible reasons that can affect a house price.<br>
Just reflecting on my own experience, it is clear I am not very rational when it comes to buying a house (or anything else for that matter).<br>
The first house we bought - my wife and I - was a house I completely fell in love with.<br>
Did we end up paying a price higher than the predictable market value? I am afraid yes.<br>
For our second house, the main factor was the height of the ceilings, I just loved to have high ceilings.<br>
The same house with lower ceiling? I don't think I would even have considered it.<br>
Arguably, that second example is tangible enough that it could be modeled and if there are enough of us out there who are crazy for high ceilings, then we could make an impact on the market value.<br>
The problem is that at the end, the price is the result of human emotions and human interactions and there is no way to predict how that is going to turn out.

It reminds me of the concept of "homo economicus" where humans are supposed to be 100% rational and focused only on the pursuit of their self-interest.<br>
In a world of economic men, the market value of a house could conceivably be the same as its price.<br>
But I don't know any person who is 100% rational and if I ever buy a 3rd house, I am pretty sure I will end up paying a price that is different from the predicted market value.

As a final note, I think it is clear that having access to a predicted market value has itself an impact on the house market.<br>
Let's imagine that a prominent website like Zillow changes the formula for all the houses in an area. Let's say all houses get undervalued by 5%.<br>
Would the actual selling price be affected?<br>
I think so. So, I wonder if and how that feedback loop could be modeled.<br><br>

PS: For reference, here is the github repository with my work and all the predictions:
[https://github.com/poariston/LinearRegression_HousePricePrediction](https://github.com/poariston/LinearRegression_HousePricePrediction)<br>

