---
layout: post
title:  "Shopify app store analysis"
date:   2020-07-19 00:00:00 +1000
comments: true
---

With coronavirus lock-down v2 (in Melbourne, Australia) I've found myself with a bit of extra time. This extra time, in conjunction with the eCommerce boom has led me to think about how I could help small business owners.

After I came up with a few ideas it was time to do some validation before I started to build anything.

My first goal was to see if there are any notable trends in one of the larger eCommerce app stores / marketplaces. I selected Shopify given its popularity and maturity. 

Now, before I go any further I just want to clarify this is not a research paper! It's just a few hours of work and some wild assumptions.

## My Goal

Before I started, I set a few goals. Here they are:

1. Count the number of apps (both the overall total and each categories totals)
2. Identify the category trends (looking for popular categories e.g. high number of reviews)
3. Check the customer satisfaction trends (looking for categories with unhappy customers e.g. more negative reviews then positive)
4. Avoid manual tasks as much as possible (so I can re-run the analysis on demand)

## Approach

Here is my process (sounds simple, right?):

1. Collect all the data (into a database / csv file)
2. Run the analysis
3. Create a report with some fancy graphs

## Observations

1. It's not possible to know exactly how many installs / customers each app has. 
2. The quantity (and quality) of customer reviews is one way to determine the popularity of an app
2. Apps are sometimes listed in 2 categories (I have included some comments on how this has been handled)
3. I've interpreted positive reviews as being 4 stars or more and negative reviews being 3 stars or less

## The tools

There are many suitable tools & libraries. I've selected a few that I'm familiar with and some others that I wanted to learn. Here is what I used:

1. Python (programming language)
2. Scrapy (web scraping)
3. Pandas (data structure)
4. NumPy (maths)
5. Pyplot (graphing)
6. Jupyter notebook (debugging / sharing the code)
7. GitHub (source control)
8. My brain (for some good and bad ideas)

## The results

There are 4,422 apps and 922 of them have 0 customer reviews. Conveniently that leaves 3,500 apps with 1 or more customer reviews.

### App By Categories

There are 12 top level categories.

<strong>Here are the number of apps by category:</strong>

[![app count by category in Shopify app store](/assets/1-app-count-by-category-in-shopify-app-store.png)](/assets/1-app-count-by-category-in-shopify-app-store.png){:target="_blank"}

### Customer Reviews

There are a total of 428,280 customer reviews. 

<strong>Here are the reviews over time:</strong>

[![review count Shopify app store](/assets/2-review-count-shopify-app-store.png)](/assets/2-review-count-shopify-app-store.png){:target="_blank"}

<strong>Here are the reviews by category:</strong>

[![review count by category in Shopify app store](/assets/3-review-count-by-category-in-shopify-app-store.png)](/assets/3-review-count-by-category-in-shopify-app-store.png){:target="_blank"}

<strong>Monthly reviews by category (Postive >= 4 stars, Negative <=3 stars):</strong>

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Store design.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Store design.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Marketing.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Marketing.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Sales and conversion optimization.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Sales and conversion optimization.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Finding and adding products.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Finding and adding products.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Orders and shipping.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Orders and shipping.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Customer support.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Customer support.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Reporting.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Reporting.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Trust and security.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Trust and security.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Finances.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Finances.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Inventory management.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Inventory management.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Productivity.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Productivity.png){:target="_blank"}

[![xxx](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Places to sell.png)](/assets/4-monthly-review-count--by-cat-in-shopify-app-store-Places to sell.png){:target="_blank"}

## My observations

1. From ~2016 there have been 3 categories that started collecting a lot of customer reviews. I have interpreted this as a sign of demand / popularity. These categories are (1) Sales & Conversion optimization, (2) Marketing, (3) Store Design
2. The 'places to sell category' was relatively even in terms of positive and negative reviews up until mid 2019. Several of the apps had been attracting a lot of negative reviews. 
3. Customer reviews have increased across the board since the early part of 2020. In my opinion (not validated) - it's likely that there are more eCommerce stores & app purchases due to COVID19.
