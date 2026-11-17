# Smart India Hackathon Workshop
# Date: 17-11-2026
## Reference Number: 26001770
## Name: AAKASH M

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
1. Explanation of the solution

Our idea is a website and mobile app where a farmer or an FPO can put up their produce for sale and a buyer can order it directly. Buyers can be ordinary households, small shops, restaurants, or wholesalers.

A farmer signs up, adds a crop with the quantity, price and a photo, and right beside it sees today’s mandi price for that crop. That way they know if they are asking too much or too little. The buyer searches by crop or by area, orders, pays online and follows the delivery. Shops and wholesalers get a separate bulk order section for large or repeat orders. FPOs can list the combined stock of their members as one lot.

2. How it solves the problem

Right now a farmer sells to a local trader, the trader sells to an agent, the agent sells to a retailer, and everyone keeps a cut. The farmer gets the smallest share and the customer still pays a high price. On our platform the buyer orders from the farmer directly, so the agent and trader steps are not needed. Price data from AGMARKNET lets the farmer see the market rate before agreeing to anything. Transport is arranged through local logistics partners, so the farmer does not have to find a vehicle. The price and order status are visible to both sides, so nothing is hidden. The money that used to go to the middle steps is split between a higher farmer price and a lower buyer price.

3. What is different about it

Existing platforms like e-NAM mostly work between mandis and licensed traders. We are aiming at the direct link between the farmer and the final buyer. A few things we are putting together in one place: price guidance and a demand forecast on the same screen where the farmer lists the crop, delivery routes that combine nearby pickups and drops, an interface in local languages for people who have not used a smartphone much, and support for FPOs so small farmers can sell together in bulk.

## Technical Approach
1. Technologies

The frontend is HTML, CSS and JavaScript, kept light so it runs on cheap phones. The backend is Python with Django, which already gives us login, an admin panel and the REST API we need. Data goes in PostgreSQL (MySQL also works). For demand forecasting we will train a machine learning model in Python on past price and arrival data from AGMARKNET. Google Maps API is used for locations and delivery routes, a payment gateway handles payments, and the whole thing is hosted on a cloud server.

2. Methodology and process

The flow is:

Registration (farmer or buyer) → farmer lists product and price → buyer searches and orders → payment → delivery assigned and route planned → delivery tracking → order completed and rated

The forecasting model runs in the background and tells farmers which crops are likely to be in demand in the coming weeks.

Working prototype: a web app with a farmer dashboard and a customer dashboard, with product listings, order management and delivery tracking.

![alt text](<Screenshot (21).png>)

![alt text](<Screenshot (22).png>)

![alt text](<Screenshot (23).png>)
## Feasibility and Viability
1. Feasibility

Everything we use is open source or has a free tier, and the app works in any phone browser, so building it is realistic. We would start with one district and a few farmers and FPOs, see what breaks, and then expand.

2. Challenges and risks

Many farmers are not comfortable with apps. Village internet is often weak. Getting produce from the farm to the buyer is not easy. Quality is not the same from one farm to another. And some people will worry about paying online to someone they have never met.

3. How we deal with them

For the app problem we keep the screens simple with big buttons, local languages and short tutorial videos, and ask FPOs to help with onboarding. Pages are kept small so they load on slow networks. For transport we tie up with local transporters instead of buying vehicles. Listings go through a basic quality check and buyers can leave ratings. Payments go through well-known gateways, not something we build ourselves.

For revenue, we take a small fee on each transaction, a commission from logistics partners, and charge bulk buyers for extras like priority listing and order reports. Farmers use it free or almost free.

## Impact and Benefits
1. Impact on the target audience

Farmers and FPOs keep a bigger part of the final price and know the market rate before they sell. Consumers and shops get fresher produce, usually cheaper. Bulk buyers get a steady source with clear pricing.

2. Benefits

Economic: more income for farmers, lower prices for buyers, and some new jobs in local transport and packing.
Social: small farmers get access to markets they could not reach before, more people in villages start using digital tools, and there is more trust between buyers and sellers.
Environmental: combined deliveries mean fewer half-empty trips, and better forecasting means less produce gets wasted unsold.

## Research and References
1.e-NAM (National Agriculture Market): https://enam.gov.in
2.AGMARKNET (market price data): https://agmarknet.gov.in
3.Farmer Portal: https://farmer.gov.in
4.Digital India: https://www.digitalindia.gov.in
5.FAO: https://www.fao.org
6.Django Documentation: https://docs.djangoproject.com
