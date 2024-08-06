---
layout: post
title: "Shopify app store trends"
date: 2020-07-19 00:00:00 +1000
excerpt: "Using customer feedback to find a new startup idea"
---

During Melbourne's second coronavirus lockdown, I found myself with some spare time.

The recent eCommerce boom got me thinking about new business ideas.

Before jumping into validation and development, I aimed to identify notable trends in the types of eCommerce marketplace apps people are using.

I chose the Shopify App Store due to its popularity and maturity.

Please note, this analysis is not a comprehensive research paper—just a few hours of work.

## My Goal

Before I started, I set a few goals. Here they are:

1. Count the number of apps and the category totals
2. Identify the category trends
3. Idenity customer review trends
4. Automate as much as practical (so I can run this analsys again at a later time)

## Some of my thoughts

1. The total number of reviews an app has is a (rough) measure of popularity
2. The customer ratings of an app might show where there are opportinities to better service the community
3. For simplicity, I will consider 4-5 star reviews (our of 5) as positve and 1-3 star review (out of 5) as negative

## The tools

There are many suitable tools & libraries. I've selected a few that I'm familiar with and some others that I wanted to learn. Here is what I used:

1. Python (programming language)
2. Scrapy (web scraping)
3. Pandas (data structure)
4. NumPy (maths)
5. Pyplot (graphing)
6. Jupyter notebook (great for data anlyitics and debugging)
7. GitHub (source control)

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

## Summary / observations

1. From ~2016 there have been 3 categories that started collecting a lot of customer reviews. I have interpreted this as a sign of demand / popularity. These categories are (1) Sales & Conversion optimization, (2) Marketing, (3) Store Design
2. The 'places to sell category' was relatively even in terms of positive and negative reviews up until mid 2019. Several of the apps had been attracting a lot of negative reviews. 
3. Customer reviews have increased across the board since the early part of 2020. In my opinion (not validated) - it's likely that there are more eCommerce stores & app purchases due to COVID19.
