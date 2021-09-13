# E-commerce Website Performance Analysis

Company Profile: Maven Fuzzy Factory, an eCommerce start-up.
Case Brief: Top Traffic & Channel, Landing Page Testing (Bounce Rates, Conversion rate funnels), Product (Cross-selling products, Refund rates), User (Repeat behaviors) Analysis.

## 1. DATABASE EXPLANATION
Maven Fuzzy Factory Database contains six related tables of eCommerce data:
- Website Activity: website_sessions, website_pageviews
- Products: products
- Orders and Refunds: orders, order_items, order_item_refunds

 and Refunds: orders, order_items, order_item_refunds


## 2. TOP TRAFFIC SOURCE & CHANNEL
### Business Concept
Traffic source analysis is about understanding where your customers are coming from and which channels are driving the highest quality traffic.
Channel Analysis is about bidding efficiently by understanding the value of various segments of paid traffic. 
Paid traffic is commonly tagged with tracking UTM parameters, which are appended to URLs and allow us to tie website activity back to specific traffic sources and campaigns.

### Key Tables & Metrics
Trended session volume by Traffic Source: 
- Trended: year, month of 'created_at' column
- Session volume: total count of 'website_session_id' column
- Traffic Source: defined by 'utm_source, utm_campaign, http_refer' columns
Session - order conversion rate by UTM source and device type: 
- Session - order conversion rate: total count of 'order_id' column divided by total count of 'website_session_id' column
- Utm source & device type: defined by 'utm_source, device_type' columns

## 3. LANDING PAGE TESTING: BOUNCE RATE, CONVERSION RATE
### Business Concept
Landing page testing is setting up A/B experiments on live traffic to see if we can improve bounce rates and conversion rates. 
When we perform conversion funnel analysis, we will look at each step in our conversion flow to see how many customers drop off and how many continue on at each step.

### Key Tables & Metrics
Bounce Rate: defined by the condition that the total count of 'website_pageview_id' of one particular 'website_session_id' equals to 1.
Conversion Rate: Eg: Billing - Order Conversion Rate is the total count of 'pageview_url' column when it's '/thank-you-for-your-order' divided by total count of 'website_session_id' column.

## 4. PRODUCTS: CROSS-SELLING PRODUCTS, REFUND RATE
Business Concept
Cross-sell analysis is about understanding which products are most likely to be purchased together and offering smart product recommendations.
Refund rate helps us to control the quality and detect the problems.

## 5. USER: REPEAT BEHAVIOR
Business Concept
Analyzing repeat visits helps businesses understand user behavior and identify some of the most valuable customers. Businesses track customer behavior across multiple sessions using browser cookies. Cookies have unique ID values associated with them which allows us to recognize a customer when they come back and track their behavior over time.


