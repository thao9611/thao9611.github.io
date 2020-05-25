---
layout: post
title:  "When A/B testing isn't realiable"
date:   2018-12-31 21:36:38 -0500
categories: Exploring
---
This isn’t what I have learnt. This is simply what I have read and summarized by my understand.

## Budget Effect 

Even those two targets share the same setting and similar traffic flow, the new target may perform better due to the budget. As you may want to limit the impact of the treatment in the event of failure, the testing population (audience size) may be much smaller. That’s why with the same budget amount, your strategy may work well with 5% population but fail when it comes to 100%. So to avoid this case, you may wanna ramp up slowly, 5% then 20%…

## Cannibalization

A case to demonstrate this problem of A/B testing is this: Suppose you’re a marketplace like Airbnb, eBay, or Etsy. You want to make it easier for marketplace sellers (people renting out their homes or selling items) to price their items, so you launch an A/B test where 50% of sellers see an algorithmic price suggestion and 50% of sellers don’t. Of course, you can’t run the test against users because you don’t want users see different prices. Sounds reasonable right, yet how do you measure the effectiveness of your pricing algorithm? The algorithm may increase the revenue compared to the baseline, yet what’ll happen when we launch the algorithm to all sellers? Can we still see the increase? This is because your unit of control is the seller, but your metric (revenue) depends on users as well. In this case, the testing group steals users from the control group ( that’s why we call it cannibalization). And the metric not only goes up in case of the testing but also goes down in case of the baseline ( over-counting). In this case, I think revenue isn’t the wrong metric to compare two targets, yet it won’t be the best option in long term if you wanna launch it to the whole population.

## Novelty and learning effect

In short, if you are introducing a new feature to users, then they may be interested at fist, then the CTR may increase. Also, new feature may require time to figure out its usage, so the full effect won’t be seen after a few weeks.

