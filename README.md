# Smart India Hackathon Workshop
# Date: 22/11/2026
## Reference Number: 26009317
## Name: Kishore.K

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
1. Detailed explanation of the proposed solution

The solution is a digital platform that connects farmers directly to buyers and removes the unnecessary layers between them. Instead of selling to a village agent who sells to a mandi trader who sells to a wholesaler and then a retailer, the farmer lists produce on the platform and sells straight to retailers, restaurants, apartment communities, or consumers. A small, fixed platform fee replaces the stacked margins of several middlemen.

Step 1: Farmer registration and listing

A farmer signs up with a phone number and lists the crop, quantity, quality grade, and expected harvest date. The app works in the regional language and supports voice input and WhatsApp or SMS, so farmers with low digital literacy can use it. Photos of the produce help buyers judge quality before ordering.

Step 2: Price transparency

The platform shows live mandi prices, recent trends, and a suggested fair price for the farmer's crop. This gives farmers real bargaining power, because they no longer depend on the agent's quoted rate. An AI model can also forecast prices and demand, so farmers know when to sell and which crops will be in demand.

Step 3: Buyer ordering

Retailers, hotels, and consumers browse listings, see the farmer's price, and place orders. Buyers pay less than they would through the traditional chain, while the farmer earns more. Bulk buyers can place standing orders, which gives farmers predictable income.

Step 4: Aggregation and logistics

Small farmers cannot ship small loads economically, so the platform groups nearby farmers' produce into combined loads. It matches these loads with local transport providers and nearby cold storage or collection points. This is the part that replaces the middleman's real function (moving and storing goods) at a much lower cost.

Step 5: Secure payment

Buyers pay through UPI or the platform's escrow system, and the money is released to the farmer's bank account as soon as delivery is confirmed. This removes delayed payments and cash-handling risk, which are common problems in the traditional system.

Step 6: Margin transparency

Every order shows a clear price breakdown: how much went to the farmer, transport, and the platform. Consumers can see that most of what they pay reaches the farmer. This builds trust and becomes a strong selling point of the platform. A ledger-based record can make these breakdowns tamper-proof if you want to add traceability.

Revenue model

The platform charges a small commission, for example 3 to 5 percent, on each transaction, plus a modest logistics fee. Even with this, the farmer earns noticeably more and the buyer pays less than in the multi-layer chain, so both sides gain.

Expected impact

Farmers receive a larger share of the final price, wastage drops because produce reaches buyers faster, and consumers get fresher goods at lower prices. For the hackathon, you can show this with a simple comparison of the price paid at each stage in the old chain versus the new one.

If you'd like, I can help you next with the system architecture, the pitch deck structure, or the features to prioritize for a working prototype.



2. How it addresses the problem


The problem is that several intermediaries each take a margin before produce reaches the consumer. The platform lets farmers sell directly to retailers, businesses, and households, so the village agent, mandi trader, and wholesaler layers are no longer needed. Each removed layer is a margin that no longer inflates the price.

Increases farmers' earnings

Farmers currently accept low prices because they lack information and have few buyers to choose from. Live price data and a suggested fair price give them real bargaining power, and direct buyers pay closer to the true market value. Standing orders also reduce distress selling, which is when farmers sell cheaply because the crop is perishable and they have nowhere else to go.

Reduces consumer prices

Since stacked middlemen margins disappear, the final price drops even after the small platform fee and logistics cost are added. Faster delivery also means less spoilage along the chain, and that wastage cost is normally passed on to consumers. The result is fresher produce at a lower price.

Replaces what middlemen actually do

Middlemen exist because they provide transport, storage, and market access. The platform does not ignore this. Its aggregation and logistics layer pools small farmers' produce, arranges transport, and uses nearby collection points, so farmers get the same services at a fraction of the cost.

Builds trust through transparency

A big reason farmers depend on middlemen is trust, including quick cash payment. Secure digital payments released on delivery solve this, and the margin breakdown shows everyone exactly where the money goes. This makes the system fair for both farmers and buyers.

Measurable outcome

You can demonstrate the impact with a simple before-and-after comparison. For example, if a farmer gets 40 percent of the consumer price in the traditional chain, show the share rising to 70 percent or more on the platform, while the consumer pays less. That single comparison makes the problem and the solution easy for judges to see.



3. Innovation and uniqueness of the solution


Most existing agri-marketplaces only connect a farmer to a buyer and stop there. This solution is different because it replaces the full function of the middleman, which includes price discovery, aggregation, logistics, and payment, in one connected system rather than offering just a listing app.

The first unique element is the AI-based price guidance. Instead of only showing today's mandi rate, the platform forecasts prices and demand, then tells the farmer what to grow, when to sell, and what price to ask. This shifts the farmer from reacting to the market to planning for it.

The second is the pooled logistics layer. Small farmers cannot afford to ship small loads, which is exactly why they depend on agents. By grouping nearby farmers' produce into combined loads and matching them with local transport and collection points, the platform removes the main reason middlemen exist, instead of simply bypassing them.

The third is margin transparency. Every order shows a clear breakdown of what the farmer, the transport, and the platform each received. A tamper-proof ledger can make this record trustworthy, so consumers can verify that more of their money reaches the farmer. Most platforms hide this information, and here it becomes a selling point and a trust builder.

The fourth is accessibility for real farmers. The platform works through regional-language voice input, WhatsApp, and SMS, so it does not depend on smartphone skills or English literacy. Many solutions fail because the farmers they target cannot actually use them.

Together, these features make the solution a complete replacement for the traditional chain rather than another app layered on top of it. That combination of forecasting, shared logistics, transparency, and easy access is what sets it apart





## Technical Approach
1. Technologies to be used (e.g. programming languages, frameworks, hardware)

The frontend can be built with React Native or Flutter for the farmer app, and React for the buyer dashboard. The backend can use Python with FastAPI or Node.js, with PostgreSQL as the database and Redis for caching live prices.

For AI, Python with scikit-learn or TensorFlow can forecast prices and demand using Agmarknet data. WhatsApp or SMS through Twilio, plus Bhashini or Google Speech-to-Text, gives farmers regional-language access. Razorpay handles UPI payments, and Google Maps or OpenStreetMap supports logistics and route grouping. For the transparent margin ledger, a hash-chained log or Hyperledger can be used, and the system can be hosted on AWS or Render.

Hardware is optional: ESP32 or Raspberry Pi sensors can monitor temperature and humidity in cold storage and transport.


2. Methodology and process for implementation <b>(Flow Charts/Images/ working prototype)</b>


The implementation can be done in four phases. First, research and design: study mandi price data from Agmarknet, interview a few farmers and buyers, and finalise the pilot crop and region. Second, build the core: the farmer listing screen, buyer ordering screen, and a backend with a database.

Third, add the intelligence: a basic price forecasting model, the pooled delivery grouping, and Razorpay test-mode payments. Fourth, test and pilot: run the prototype with sample users, collect feedback, and measure how much of the final price reaches the farmer compared with the traditional chain.

For the working prototype, I suggest showing four screens: the farmer's listing with the suggested fair price, the buyer's order page, the delivery grouping view, and the margin breakdown for a completed order. That is enough to demonstrate the full flow to judges without building every feature.


## Feasibility and Viability
1. Analysis of the feasibility of the idea

The idea is technically very achievable. Every component already exists as a proven, affordable technology: mobile apps, cloud hosting, UPI payments, route grouping, and price forecasting from public mandi data. A working prototype can be built by a small team within the hackathon timeline, and the more advanced features can be added gradually.

Economic feasibility

The model works because the platform replaces several stacked margins with one small fee. Even with a 3 to 5 percent commission plus a logistics charge, farmers still earn more and buyers still pay less. Costs stay low at the start, since cloud services and payment gateways charge based on usage. The main cost is logistics, so starting with a small pilot area keeps it manageable.

Operational feasibility

The hardest part is not the software but the physical movement of produce. Pickup, grading, and delivery of perishables need reliable local transport partners and collection points. This can be solved by starting in one region with one or two crops, partnering with existing farmer groups (FPOs) and local transporters, and expanding only after the pilot works.

Social and adoption feasibility

Farmers may hesitate because they trust their agent, who often provides advance loans and instant cash. The platform addresses this through voice and WhatsApp access, instant UPI payment on delivery, and a pilot run with farmer groups who vouch for it. Buyers like restaurants and retailers are usually willing to switch if quality and supply are consistent.

Legal and regulatory feasibility

Agricultural marketing rules differ by state, and some require trading through licensed mandis. However, government initiatives such as e-NAM and the recent farm marketing reforms support direct and digital sales. The team should check state rules for the pilot region, and follow food safety and payment regulations.

Key risks and how to handle them

The main risks are low farmer adoption, inconsistent produce quality, and delivery delays. These can be reduced through simple regional-language access, basic quality grading with photos, and local collection points. Middlemen may also resist, which is why partnering with them as local pickup agents, rather than fighting them, is a practical option.

Overall assessment

The idea is feasible and scalable if it starts small. A focused pilot with one crop in one region can prove the price improvement for farmers, and that evidence makes it easier to expand.



2. Potential challenges and risks

The biggest challenge is farmer trust. Farmers rely on agents for quick cash and advance loans, so switching feels risky. Regional-language voice access, instant UPI payment on delivery, and a pilot through farmer groups can build that trust.

Logistics is the next risk, since delays or poor handling can spoil perishable produce. Starting with one region and a few crops, using local transport partners and collection points, keeps this manageable.

Other risks include inconsistent quality, resistance from middlemen, and inaccurate price forecasts. Simple grading, giving middlemen a role as paid pickup agents, and showing forecasts as a range rather than a guarantee can reduce these.

Finally, state marketing rules, early funding costs, and data security need attention. Checking local regulations, running a small pilot, and using encrypted payments and storage will cover them.




3. Strategies for overcoming these challenges


To build farmer trust, start with a pilot through existing farmer groups (FPOs) in one region. Offer voice and WhatsApp access in the local language, and pay farmers by UPI on delivery so they get cash as fast as they would from an agent. Early success stories from respected local farmers will do more than any advertising.

For logistics, begin with one or two crops and a small area. Partner with local transporters, set up collection points near villages, and group nearby farmers' produce into shared loads. Add cold storage only once volume justifies it.

To handle quality and supply, use simple grading rules with photo checks, and give farmers ratings so reliable ones get more orders. Pooling produce from several farms also fills supply gaps for buyers.

Instead of fighting middlemen, bring them in as paid pickup agents or collection point operators. They keep an income through a fair service fee, and the platform gains local knowledge and reach.

For forecasting, present prices as a range and improve the model as more transaction data comes in. For regulation, check state marketing rules before launch, work with schemes like e-NAM, and follow food safety and payment norms.

To cover early costs, run a lean pilot, seek agri-startup grants and incubator support, and charge a small commission only once farmers see higher earnings. Encrypted storage, secure payment gateways, and clear consent will protect data and keep trust.



## Impact and Benefits
1. Potential impact on the target audience


Farmers benefit most. They keep a larger share of the final price, get paid instantly by UPI, and can plan crops using demand forecasts, which reduces distress selling.

Consumers get fresher produce at lower prices, with a clear view of how much of their money reaches the farmer. Retailers and restaurants get steady supply and predictable pricing, and transporters and former middlemen gain organised work as paid pickup and delivery partners.

Overall, less food is wasted, rural incomes improve, and the market becomes fairer. For the pilot, you can measure impact by tracking the farmer's share of the consumer price, which could rise from around 40 percent to 60 percent or more.



2. Benefits of the solution (social, economic, environmental, etc.)


Farmers gain income security and dignity, since they are no longer forced to accept whatever an agent offers. Price transparency makes the market fairer, and regional-language voice access includes farmers with low digital literacy. Consumers also gain trust by seeing where their money goes.

Economic benefits

Farmers keep a larger share of the final price, which raises rural incomes. Consumers pay less because stacked middlemen margins disappear. Retailers get predictable supply and pricing, and local transporters and collection point operators gain steady, organised work. Higher farm incomes also circulate in the local economy.

Environmental benefits

Faster delivery and better demand planning reduce food spoilage, which means less wasted land, water, and fertiliser. Pooled deliveries combine small loads, so fewer half-empty trips are made and transport emissions drop. Demand forecasts also help farmers grow what is needed instead of overproducing.

Technological and market benefits

The platform brings digital tools, UPI payments, and data-driven forecasting to farmers who have had little access to them. The data it collects can help planners and policymakers understand prices, demand, and supply gaps, and the model can be extended to more crops and regions.

Overall value

The solution improves farmer income, lowers consumer prices, reduces waste, and builds a more transparent market, which makes it a strong fit for both the hackathon problem and long-term rural development.


## Research and References
1. Details / Links of the reference and research work


INTRODUCTION Minimum Support Price (MSP) is an integral component of Agriculture Price Policy of India. It  targets  to  ensure  support  price  to  farmers  and  affordable  price  to  consumers  through public distribution system (PDS) [7]. The  price  support system was conceptualized during pre-green revolutionperiod as an institutional mechanism for incentivizing farmers to adapt new  technologies  [8,  4].  Later,  Agriculture  Price Commission  was  established  in  the  year 1965, based  on Jha committee recommendations to  suggest  support prices for crops after considering the cost of cultivation to account [6]. Broad objectives of the commission are to ensure  remunerative  prices  to  farmers  and  reasonable  prices  to  consumers  and  promote sustainable use of resources towards socially desirable crop mix [7]. Price incentives in the form  of  support  prices  helped  India  to  increase  food  production  during  green  revolution period.  MSP  also  aims  atprocuring  food  grains  from  food  surplus  statesfor  distribution through PDS  and  maintaining buffer stock  and thus bridge  the demand supply gap [5,  3]. Price incentives in form of MSP are credited for the increase in area under rice and wheatin the  green  revolution  states  like  Punjab  and  Haryana.Agricultural  situation  in  India  has undergone  sea  change  after  the  green  revolution  period,  but  the  agriculture  price  policy hasmore or less  remained  same  [2].  Food  surplus is available in  many  states  andnot  just Haryana, Punjab  and  Andhra  Pradesh;  however,  the  procurement  has largely  confined  to these  regions  [8].  MSP  is  viewed  as  a  safety  net  to  ensure  pricesecurity  for  a  long-term investment decisionto farmers. 


Case Studies
Digital Supply Chain Transformation in Uganda
A digital platform connecting maize farmers with traders via SMS price alerts increased rural
incomes by 2.8% by reducing price deviations and improving market transparency (Poverty
Action Lab, 2025).
Indian Dairy Cooperatives
Cooperatives like Amul succeeded by aggregating milk, standardizing quality and marketing
directly, increasing farmer incomes and improving food safety (PIB, 2024).
Policy and Institutional Frameworks
Cross-sectoral policies are essential, including:
* Investment in rural infrastructure (roads, storage).
* Credit and insurance to reduce farmer risks.
* Support mechanisms for collective marketing.


