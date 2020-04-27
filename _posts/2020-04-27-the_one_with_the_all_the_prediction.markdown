{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "---\n",
    "layout: post\n",
    "title:      \"The One with all the Prediction\"\n",
    "date:       2020-04-27 15:22:10 +0000\n",
    "permalink:  the_one_with_all_the_prediction\n",
    "---\n",
    "\n",
    "\n",
    "### April 2020\n",
    "\n",
    "I reached the second milestone in my Data Science Online Course: the end of the second “module” and its end-of-module project.\n",
    "This time it was about linear prediction and I was tasked with predicting house prices from house characteristics.\n",
    "In Data Science jargon, the characteristics should be called independent variables, predictors or features, and the house price, dependent variable or target variable.\n",
    "The features I ended up using were: \n",
    "* size of the lot,\n",
    "* living area apart from basement,\n",
    "* total living area,\n",
    "* total living area average of the 15 closest houses, \n",
    "* latitude,\n",
    "* construction grade,\n",
    "* number of bedrooms,\n",
    "* number of bathrooms,\n",
    "* number of floors,\n",
    "* whether it was a waterfront house or not.\n",
    "\n",
    "My results ended up being relatively good even if I wished I would have spent more time investigating polynomial regression and interactions between features. \n",
    "But, rather than the performances of my model, I would like to discuss a potential assumption behind all this exercise. \n",
    "Maybe it is not an assumption, maybe it is more of a mindset. \n",
    "I think it is easy to get carried away and believe that it is actually possible to predict a house price only from tangible features like the ones listed above.\n",
    "What I mean is: yes, it is possible to build a prediction model that minimizes the errors for the data we collected. Yes, for a given house, the prediction will be pretty close to the actual selling price. \n",
    "But no, we can't predict exactly the price a given house will be sold in the future.\n",
    "Maybe the project should not describe the target variable as a \"price\", but rather as a \"market value\". \n",
    "My point is that the predictable market value of a house can be different from its price.\n",
    "It seems to me that there is an abundance of intangible reasons that can affect a house price.\n",
    "Just reflecting on my own experience, it is clear I am not very rational when it comes to buying a house (or anything else for that matter). The first house we bought - my wife and I - was a house I completely fell in love with. Did we end up paying a price higher than the predictable market value? I am afraid yes. For our second house, the main factor was the height of the ceilings, I just loved to have high ceilings. The same house with lower ceiling? I don't think I would even have considered it. Arguably, that second example is tangible enough that it could be modeled and if there are enough of us out there who are crazy for high ceilings, then we could make an impact on the market value.\n",
    "The problem is that at the end, the price is the result of a human interaction and there is no way to predict how that is going to turn out.  \n",
    "\n",
    "It reminds me of the concept of \"homo economicus\" where humans are supposed to be 100% rational and focused only on the pursuit of their self-interest. In a world of economic men, the market value of a house could conceivably be the same as its price. But I don't know any person who is 100% rational and if I ever buy a 3rd house, I am pretty sure I will end up paying a price that is different from the predicted market value.\n",
    "\n",
    "As a final note, I think it is clear that having access to a predicted market value has itself an impact on the house market. Let's imagine a prominent website like Zillow changes the formula for all the houses in an area. Let's say all houses get undervalued by 5%, would the actual selling price be affected? I think so.\n",
    "So, I wonder if and how that feedback loop could be modeled. \n",
    "\n",
    "\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.6.9"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
