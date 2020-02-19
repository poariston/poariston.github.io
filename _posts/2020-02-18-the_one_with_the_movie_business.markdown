---
layout: post
title:      "The One with the Movie Business"
date:       2020-02-18 23:22:10 +0000
permalink:  the_one_with_the_movie_business
---


### February 2020

Still a work in progress. Still a work in progress. <br><br>
I reached a milestone in my Online Data Science Bootcamp course: the end of the first “module”. The course is split into 5 modules and each one ends with a “project”. What is great about the projects is the relative freedom we are given to make up our own questions and figure out ourselves how to find answers. The topic was the movie business. We started from movie related data coming from websites such as Box Office Mojo, IMDB, Rotten Tomatoes and TheMovieDB.org.<br>
I want to share some of my findings because they were surprising to me, pushed me to reflect on them and investigate a bit further.<br>
I started with a basic question: Is the movie business a profitable business? What kind of average profit can a movie studio expect?<br>
Here are two slides explaining how I tried to respond to that question.<br>

![image1](https://github.com/poariston/poariston.github.io/blob/master/img/profitability1of2.jpg)

![awesome](https://raw.githubusercontent.com/learn-co-curriculum/dsc-mod-1-project-v2-1/master/awesome.gif)

For a short while, I felt good about having calculated a profit ratio rather than just taking the gross income $ amounts. After all, a movie that generated a lot of income may not have made a profit if its cost was high. To calculate the profit ratio, I divided the data labeled “worldwide_gross” by the “production_budget”. Actually, “profit ratio” is not a very good name for it. What I aimed for was to calculate a rate of return for each movie. But an industry where we can expect a rate of return of 3.67 seems too good to be true, and I started wondering whether my approach was not too simplistic.
Indeed, I think there were multiple issues with my approach.
First, I don’t know how the data was collected. I just found 2 columns in a table labelled production_budget and worldwide_gross and I assumed they were respectively the total cost and the total income of the movies. The key word is “assumed”. Before starting to interpret the meaning of these numbers, I would need to know where they are coming from and how they were collected.
Then, I realized that a movie has many potential sources of income: the theatrical run (i.e. cinemas), home entertainment (i.e. DVD and Blu-ray), television deals, Video on Demand (i.e. Netflix, iTunes, etc), and other income streams such as hotels, airlines, merchandising and a cut of music sales. How to relate the label “worldwide_gross” to all these income sources? At this point, it was clear to me that I was lacking subject matter knowledge. I was able to read files, transform them into Pandas dataframes, clean the datasets, join the dataframes, make nice graphs, but I was not knowledgeable about the data I was manipulating. I was trying to extract meaning from data I didn’t know enough about. I hope it will be a lesson for me in the future.
Lastly, I also realized that the cost of a movie was an obscure concept for me. Here are some costs to account for: the original production budget, marketing and advertising, the physical costs of getting the film in cinemas and on shelves, contingent compensation for key talent, and other costs such as overhead, interests and financing costs. So, again, the data labeled “production_budget” was, at best, one cost among many. At that point I discovered that Wikipedia had a full page titled Hollywood accounting about the “opaque or creative accounting methods used by the film, video, and television industry”, which I found a bit demoralizing.
Pondering on my little “project” experience, I need to accept the fact that I was so eager to produce insight from data that I didn’t do the necessary preliminary hard work of understanding the data and learning the necessary subject matter knowledge I needed to give meaning to my work.


References:
Here are some interesting websites where I got some of the information I used in this post.

