---
layout: post
title:      "The One with the Chained Indexing"
date:       2020-02-16 23:22:10 +0000
permalink:  the_one_with_the_chained_indexing
---


### February 2020 


Three months ago, I started the Online Data Science Bootcamp course offered by Flatiron School. With this first blog post, I wanted to share an experience that has helped me.

I think it is a very sweet moment when you find on the web someone who has written about the exact same question that you have been wondering about. I like that feeling of validation and shared concern. Sometimes, it happens to me with the public Q&A section of stackoverflow.com, when I find the question that I was asking myself. However, I feel an even stronger satisfaction when I find an entire blog post answering one of my questions. 

Here is my best example so far. It is related to chained indexing. I heard about this concept for the first time through the automatic ‘SettingWithCopy’ warning message that you may have encountered while coding with Pandas in a jupyter notebook. Here is the warning:

“
…\Anaconda3\envs\learn-env\lib\site-packages\pandas\core\indexing.py:205: SettingWithCopyWarning: 
A value is trying to be set on a copy of a slice from a DataFrame

See the caveats in the documentation: http://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
”

When you follow the link, you get to a page of the Pandas User Guide warning you about chained indexing.
The first time I read this page, I found it confusing. 
It is only when I read the following blog post that I really understood it (thanks to my Flatiron teacher who found it for me!):
https://medium.com/dunder-data/selecting-subsets-of-data-in-pandas-part-4-c4216f84d388
I found the post clear, complete, and it made sense to me. 

Here is my understanding:

The SettingWithCopy warning is triggered by the following Pandas sequence:
1. First subset selection (some columns in a Pandas dataframe for instance)
2. Second subset selection (some lines in a Pandas dataframe for instance)
3. Assignment of new values to the resulting subset.

Chained indexing means two subset selections immediately following each other in the same line of code (steps 1 and 2 together). 

The warning message is a Pandas message, but chained indexing is a concept that applies both to Python and Pandas.

Doing two subsequent subset selections (whether in one line of code or 2) is dangerous because after the first selection, we don't always know whether it is a copy or a view of the original object that gets created. 

If the first selection resulted in a copy, then a new object was created and the assigned value (in step 3) will be assigned to the copy not the original.

If the second selection resulted in a view, then no new object was created and the assigned value (in step 3) will be assigned to the original object.

So, we end up in a situation with an unpredictable result and not knowing what the user wanted to accomplish.

There are 2 ways to fix this issue:
1. If you want to modify the original object, avoid the succession of 2 selections by using exactly one indexer (.loc or .iloc for pandas). 
2. If you don’t want to change the original object, make a copy of the subset of the original object, before assignment of new values.

But this is much better explained in the blog I was talking about. Thanks to its author: Ted Petrou. 

I hope you will find it helpful too.




