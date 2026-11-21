# Smart India Hackathon Workshop
# Date: 21/11/2026
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
Remove These Lines
1. Detailed explanation of the proposed solution:



 The proposed solution for SIH 26033 is an AI-driven farm-to-fork direct supply and micro-aggregation platform that eliminates the traditional chain of middlemen by connecting farmers and Farmer Producer Organizations (FPOs) directly with bulk buyers and retail consumers. To overcome digital literacy barriers, farmers list their upcoming harvests using regional voice commands powered by India's BHASHINI API, while an integrated computer vision model grades produce quality from simple photos and a dynamic pricing engine pulls live AGMARKNET mandi rates to recommend a transparent fair price that increases farmer earnings while lowering retail costs. Because small farmers cannot afford individual city transport, the platform automatically groups nearby harvests into virtual pools to share full-truckload logistics, supported by AI demand forecasting that alerts farmers to urban demand spikes in advance and route-optimization algorithms that schedule fast, multi-stop village pickups to minimize post-harvest spoilage. Finally, every transaction is secured through an automated UPI split-escrow system that releases instant payouts to farmers upon QR-code pickup and delivery scans, while providing consumers with a traceable QR tag showing the exact farm origin and transparent price breakdown.


 
2. How it addresses the problem:





The proposed solution directly addresses the problem statement by dismantling each bottleneck that allows intermediaries to capture value and inflate retail prices:

* **Eliminating Multi-Tier Markups:** By connecting farmers and Farmer Producer Organizations (FPOs) directly to bulk buyers and retail consumers through a unified marketplace, the platform removes 4 to 5 layers of commission agents, wholesalers, and local aggregators—redirecting their 40–60% margin back to farmers as higher income and to consumers as lower prices.
* **Ending Price Information Asymmetry:** Integrating live **AGMARKNET** mandi prices with an AI dynamic pricing engine ensures farmers know the true market value of their harvest in real time, preventing local middlemen from exploiting them with artificially low farm-gate offers.
* **Solving Smallholder Transport & Scale Barriers:** Through **Virtual Harvest Pooling**, small farmers with limited produce are automatically clustered with nearby farms to share full-truckload (FTL) logistics, giving them the same bulk transport economics as large commercial farms without needing middlemen to aggregate their stock.
* **Reducing Post-Harvest Spoilage & Wastage:** AI demand forecasting aligns harvests with real urban buyer orders in advance, while **milk-run route optimization** dispatches fast, direct farm-to-buyer pickups. Cutting out slow, multi-hop mandi storage dramatically reduces perishable spoilage, which otherwise drives up final retail prices.
* **Replacing Middleman Credit & Trust:** Farmers often rely on intermediaries because they pay cash upfront and buyers distrust unverified farm produce. The platform solves both using **AI visual quality grading** (verifying Grade A/B/C produce upfront) and **QR-triggered UPI split-escrow**, which guarantees instant, risk-free digital payouts to farmers upon pickup and delivery.



3. Innovation and uniqueness of the solution:



  Most existing agri-tech apps simply act as digital classifieds, leaving small farmers stranded with high transport costs, unverified produce quality, and complex interfaces. Your solution stands out to Smart India Hackathon evaluators through five distinct innovations:

* **Virtual Harvest Pooling (Micro-Aggregation Engine):** Instead of forcing a small farmer with 80 kg of produce to pay for an entire truck, the platform dynamically clusters nearby farms harvesting the same crop into a single virtual bulk consignment. This gives marginal farmers the exact same full-truckload (FTL) transport economics as large commercial farms without needing physical warehouses or middlemen.
* **Radical "Open Receipt" Price Transparency via Dynamic QR:** Every crate receives a farm-origin QR code that lets the end buyer see the exact rupee breakdown of their purchase (e.g., how much went directly to the farmer, logistics, and platform fee), alongside harvest timestamps and farm details. This transforms ethical sourcing into a verifiable feature that builds instant consumer trust.
* **Zero-Typing, Vernacular Voice-First UX (BHASHINI Integration):** Rather than relying on English forms that exclude rural farmers, the system uses Government of India's **BHASHINI** multilingual AI APIs so farmers can list crops, check mandi rates, and confirm pickups purely through regional voice commands (Tamil, Hindi, Telugu, etc.) or simple WhatsApp/IVR prompts.
* **AI Visual Grading + QR-Triggered UPI Split-Escrow:** Replacing the trust and credit role of middlemen, a lightweight computer vision model standardizes produce quality (Grade A/B/C) from a short video, while a smart UPI escrow automatically splits and releases instant T+0 payouts directly to the farmer's bank account the moment the logistics driver scans the crate QR at pickup and delivery.
* **DPI-Native & ONDC-Ready Interoperability:** Built to plug directly into India's Digital Public Infrastructure—pulling daily price benchmarks from **AGMARKNET**, verifying farmer profiles via **AgriStack**, and exposing FPO catalogs to **ONDC (Open Network for Digital Commerce)**—the platform avoids building an isolated walled garden and instead scales rapidly across existing national buyer networks.

## Technical Approach
Remove These Lines
1. Technologies to be used (e.g. programming languages, frameworks, hardware):

The proposed solution for SIH 26033 is built using **Python, Dart, TypeScript, and SQL**, combining a cross-platform **Flutter** mobile app for farmers and drivers with a **React.js and Tailwind CSS** web portal for bulk buyers and Farmer Producer Organizations (FPOs). The backend runs on **FastAPI** supported by **PostgreSQL with PostGIS** for geospatial farm clustering, **Redis** for real-time caching, and **Docker** on cloud infrastructure, alongside **WhatsApp Business API** for low-bandwidth feature-phone access. For intelligence and logistics, the system integrates **PyTorch/YOLOv8** for visual produce quality grading, **XGBoost and Prophet** for demand and fair-price forecasting, and **Google OR-Tools** with **Google Maps APIs** for multi-stop route optimization. Finally, it connects directly to India's Digital Public Infrastructure using **BHASHINI** for vernacular voice listings, **AGMARKNET 2.0** for live mandi pricing, **ONDC** for open marketplace interoperability, and **Razorpay Route** for automated UPI split-escrow payments, backed at the field level by standard **Android smartphones, thermal QR label printers, and BLE digital weighing scales** at FPO collection centers.

2. Methodology and process for implementation <b>(Flow Charts/Images/ working prototype)</b>:

The implementation follows a four-phase iterative methodology, beginning with data ingestion where farmers onboard via a Flutter app and list crops through BHASHINI regional voice commands while an ETL pipeline pulls live mandi prices from AGMARKNET 2.0 into PostgreSQL. In the second phase, uploaded produce photos are processed by a YOLOv8 computer vision model to assign standardized quality grades (`Grade A/B/C`), and an XGBoost pricing service calculates a transparent fair-price band between farm-gate and retail rates. The third phase handles geospatial micro-aggregation using PostGIS spatial queries to group nearby harvests within a 5–10 km radius into virtual pools once buyer orders meet vehicle capacity, feeding those coordinates into a Google OR-Tools solver to generate the shortest multi-stop pickup route. Finally, the fourth phase integrates Razorpay Route UPI split-escrow and dynamic QR traceability, automatically releasing 70% payment upon farm pickup scan and the remaining 30% upon buyer delivery—a complete workflow demonstrated in our working prototype through live farm clustering, interactive map routing, and real-time farmer-versus-middleman margin calculation.




## Feasibility and Viability
1. Analysis of the feasibility of the idea:



The proposed solution is technically, operationally, and financially feasible because it relies on mature open-source technologies such as FastAPI, PostGIS, YOLOv8, and Google OR-Tools while plugging directly into India's existing Digital Public Infrastructure—including BHASHINI for vernacular voice input, AGMARKNET 2.0 for live mandi pricing, and ONDC for buyer network interoperability—eliminating heavy R&D and licensing costs. On the ground, operational feasibility is ensured by onboarding farmers through existing Farmer Producer Organizations (FPOs) and utilizing an asset-light logistics model that partners with local third-party mini-truck operators alongside offline-capable apps and WhatsApp/IVR fallbacks for low-connectivity rural areas. Financially, the platform remains self-sustaining through a zero-commission policy for farmers paired with a nominal 2%–3% transaction fee on bulk institutional buyers and logistics partners, ensuring strong unit economics while delivering higher net earnings to farmers and lower prices to consumers.



2. Potential challenges and risks:


The primary challenges and risks include overcoming the initial two-sided marketplace cold-start problem, where low early order density can lead to under-utilized transport vehicles and limited historical transaction data for training AI demand forecasting models. On the ground, adoption faces behavioral and financial friction because smallholder farmers often depend on local middlemen for informal pre-harvest credit and immediate cash, alongside resistance from entrenched mandi networks and limited managerial capacity within local FPOs. Operationally, the platform also risks quality or weight disputes between visual smartphone grading and physical delivery, transit spoilage of perishable crops during multi-stop pickups, intermittent rural internet connectivity, and varying state-level APMC direct-procurement regulations.   



3. Strategies for overcoming these challenges:


To overcome the marketplace cold-start problem, the platform adopts a hyper-local rollout anchored around existing Farmer Producer Organizations (FPOs) and recurring institutional buyers such as hostels and retail chains, while pre-training AI demand models on historical AGMARKNET datasets. Farmers' dependence on middlemen for immediate cash is countered through instant T+0 UPI split-escrow payouts—releasing 70% upon farm pickup scan—and linking verified digital sales records to formal NABARD/Kisan Credit Card micro-credit. Quality and weight disputes are minimized by combining AI visual grading with BLE digital weighing scales and tamper-evident QR crate seals at FPO collection points, while rural connectivity and literacy barriers are solved via offline-first local data syncing, BHASHINI voice/WhatsApp interfaces, and trained FPO village coordinators. Finally, operating through registered FPOs and ONDC-compliant trade protocols ensures smooth regulatory alignment across state APMC frameworks



## Impact and Benefits
Remove These Lines
1. Potential impact on the target audience:

The proposed solution creates a transformative, measurable impact across every participant in the agricultural supply chain. Small and marginal farmers gain a 25% to 40% increase in net earnings by capturing margins previously lost to intermediaries—where growers often receive as little as 33% of the final consumer rupee—while achieving financial independence through instant T+0 UPI escrow payouts, AI demand alerts that prevent distress selling, and inclusive vernacular voice onboarding. End consumers benefit from 15% to 20% lower retail prices, fresher farm-to-fork produce, and full trust through scannable QR tags displaying the exact farm origin and rupee price split. Simultaneously, bulk institutional buyers such as restaurants, supermarkets, and hostels secure reliable, AI-graded harvests at lower procurement costs, while Farmer Producer Organizations (FPOs) and local logistics operators achieve higher asset utilization, verifiable digital credit histories, and optimized delivery routes.



2. Benefits of the solution (social, economic, environmental, etc):


The proposed solution delivers wide-ranging economic, social, environmental, and governance benefits across the agricultural ecosystem. Economically, it boosts smallholder farmers' net earnings by 25% to 40% while lowering consumer grocery prices by 15% to 20% through direct farm-to-buyer trade, shared full-truckload logistics, and instant T+0 UPI split-escrow settlements that accelerate rural cash flow. Socially, it empowers marginal and semi-literate farmers with independent market access via BHASHINI vernacular voice interfaces, strengthens collective bargaining through Farmer Producer Organizations (FPOs), and improves urban household access to fresh, affordable food. Environmentally, AI demand forecasting and milk-run route optimization curb post-harvest perishable spoilage, reduce empty-mile truck trips and carbon emissions, and conserve the water and agricultural inputs embedded in food that would otherwise go to waste. Finally, at a governance level, AGMARKNET 2.0 integration, ONDC interoperability, and scannable price-breakdown QR codes bring radical transparency to food pricing and deter artificial supply-chain hoarding.






## Research and References
1. Details / Links of the reference and research work:


Improper stakeholder practices are considered a primary driver of food loss. This study aims to investigate the consequences of pre- and post-harvest practices on extending the shelf life of agro-food products, identifying which practices yield the highest marginal returns for quality. Using Fractional Regression Models (FRM) and Ordinary Least Squares (OLS), the research analyzed data from 343 Egyptian grape farmers and intermediaries. Key findings at the farmer level include significant food loss reductions through drip irrigation (13.9%), avoiding maturity-accelerating chemicals (24%), increased farmer-cultivated area (6.1%), early morning harvesting (8.7%), and improved packing (13.7%), but delayed harvesting increased losses (21.6%). For intermediaries, longer distances to market increased losses by 0.15%, while using proper storage, marketing in the formal markets, and using an appropriate transportation mode reduced losses by 65.9%, 13.8%, and 7.9%, respectively. Furthermore, the interaction between these practices significantly reduced the share of losses. The study emphasizes the need for increased public–private partnerships in agro-food logistics and improved knowledge dissemination through agricultural extension services and agri-cooperatives to achieve sustainable food production and consumption. This framework ensures robust, policy-actionable insights into how stakeholders’ behaviors influence postharvest losses (PHL). The findings can inform policymakers and agribusiness managers in designing cost-efficient strategies for reducing PHL and promoting sustainable food systems.

Keywords: food handling practices, stakeholders’ training needs, horticultural postharvest loss, good agricultural practices, grapes supply chain, shelf life

1. Introduction
Identifying and addressing the food loss drivers, including improper stakeholder practices, is essential to sustain and maintain the shelf life of agro-food products across the supply chain (SC) for as long as possible [1,2,3]. The Boston Consulting Group (BCG) (Boston Consulting Group https://www.bcg.com/publications/2018/tackling-1.6-billion-ton-food-loss-and-waste-crisis, accessed on 30 April 2025) estimates that by 2030, annual food losses and waste (FLW) (according to the FAO, food loss refers to the share of food lost across the food supply chain before it reaches the final consumer, while food waste represents the share of food wasted by the consumers) will hit 2.1 billion tons, worth USD 1.5 trillion, and decreasing it is crucial to achieve sustainable food system transformation, particularly in developing countries (which import most of their food) [4]. Meanwhile, improper handling and hygiene practices result in food contamination, constantly increasing the percentage of loss across the supply chain [5]. Furthermore, measuring the interaction between socioeconomic factors and stakeholder practices toward reducing the rate of loss across the food supply chain (FSC) plays an essential role in designing an appropriate solution to minimizing the share of lost food at different nodes across the supply chain [6,7]. The marginal benefits of preventing losses should exceed the marginal costs to make the intervention more attractive to relevant stakeholders [8]. Adopting good agricultural practices, including cultivation, harvesting, handling, and postharvest practices, dramatically improves the farmers’ net profit and enables the sustainable use of limited resources in developing countries by reducing the percentage of FLW [9]. Generally, pre-sorting on farms can remove fruits with unacceptable shapes, sizes, and colors during harvesting, grading, and sorting at the farm gate. However, these fruits have the same nutritional value and could be used either fresh or processed to feed humans. Due to their appearance, they are often left in the field [3,10].

The handling practices of agro-food products (such as harvesting, pre-cooling, sorting and grading, packaging, and storing) play a substantial role in preserving quality and extending shelf life [11]. Improper practices or neglecting one of the aforementioned operations lead to quality degradation, especially for perishable and sensitive fruits like grapes. For example, poor harvesting methods, incorrect cooling, and poor storage contribute to the loss of products. Because grapes are very sensitive to temperature, they cannot be kept as a product for long periods. However, the substantial role of agricultural education and extension in disseminating the best farming practices, including postharvest operations for perishable products, is weak in most developing countries [12]. This highlights the urgent need to reform the public agricultural extension institutes to raise small stakeholders’ knowledge, improve their practices and skills, and change their behaviors and attitudes to use limited resources more sustainably [13]. Considering the negative effects of spraying harmful chemicals to promote earlier fruit maturity (color, size, and solidity) or sustain their freshness after harvest, this practice can decrease the fruits’ shelf life and result in food safety problems and negative environmental impacts [14].

Fruits provide essential vitamins and offer high profit margins for small-scale farmers and middlemen. Still, the share of postharvest fruit loss is very high due to a lack of agro-processing facilities and agro-logistic services, especially in developing countries. Varying perishability between different fruit types is a key factor affecting all aspects of this industry; growers must maintain minimum product quality for consumers, which impacts pricing and the percentage of losses [3]. However, farmers and middlemen remain hesitant to adopt the recommended postharvest practices. Efforts to disseminate and encourage stakeholders to adopt these practices can significantly reduce the share of postharvest loss (PHL) in grapes and other fresh fruit and food products (PHL refers to the share of lost or wasted food across the food supply chain, starting from harvesting and extending until the product reaches the final consumer).

Egypt is ranked fourth in the world for table grape production quantity (~1.7 million tons), and growth in this production has significantly increased Egyptian grape exports over the past 15 years [2]. The FAO estimated the share of postharvest loss to be around 18.6%, 5.3%, and 6.7% for the farmers, wholesalers, and retailers in North Egypt, highlighting the critical points of losses, including the harvest, wholesale, and retailer market levels, respectively [2]. Egyptian grape producers and value chain actors are increasingly vulnerable to shifts in global markets due to a lack of marketing information and land fragmentation among small-scale producers. They might delay mature crop harvesting to decrease transportation costs, which significantly increases the loss volume. Small-scale producers lacking export access need new strategies to upgrade the table grape value chain.

The interlink between the grapes supply chain and required post-harvest operations depends on the primary destination market (domestic or export). Furthermore, neglecting these operations (e.g., sorting, packing, grading, etc.) at the farm could lead to an increase in the percentage of food loss at the following downstream stages of FSC [3,15]. Stakeholders’ practices and access to logistics significantly influence the proportion of loss across FSC, and this share varies depending on FSC efficiency, logistics service availability, and stakeholder practices [3,16]. For example, cold transportation and storage services mainly contribute to preserving the product for long periods [2]. Adopting good handling techniques, using appropriate equipment or technology, building capacity, enforcing thorough regulations, and improving marketing can avoid many problems [17]. FLW reduction interventions have garnered more global attention and investment following the global food crisis in 2008, when many countries sought to increase local food self-sufficiency through various strategies, including food loss and waste reduction, particularly in developing countries [2].

Individuals’ preferences are based on the costs, benefits, and risks of the choices in line with their socioeconomic characteristics, so they will only act if the benefit outweighs the costs [18]. In the same way, we assumed (1) the stakeholders will invest to decrease FLW when the value of the saved food outweighs the cost of the intervention (practices or technology) [19]. (2) The interaction between the different proper practices could result in a greater reduction of losses across the supply chain. However, the importance of the correlation between the farmer and middleman characteristics and their practices is emphasized. The previous studies did not analyze the different impacts of the interaction between the stakeholders’ socioeconomic characteristics and their practices toward food loss and waste, which could give an overview of the technical training needed to enhance the capacity of the small farmers and intermediaries to adopt the good agricultural practices, including the best postharvest operations. The current study aims to evaluate and analyze the interaction between stakeholders’ socioeconomic characteristics and their impacts on their practices at the different FSC stages, to determine the appropriate intervention strategies for reducing these losses. The results of this study could help policymakers, agribusiness owners, and international funding donors design sustainable intervention reduction strategies for these losses, achieve a sustainable supply chain, attain environmental preservation, and ensure efficient use of limited resources available.

The recent literature indicates a scarcity of evidence on the impact of stakeholders’ practices as a food loss driver [20]. Furthermore, the majority of earlier FLW research concentrated on calculating the proportion of loss [3,21,22], few studies have investigated the food loss driver, particularly horticultural crops. Furthermore, most of these studies used the macro-secondary data (e.g., food balance sheet, FAO) to estimate the FLW, which neglected the heterogeneity between the stakeholders and the significant role of those small stakeholders in FLW reduction strategies, and they provided only high-level insights about the nature and causes of these losses [23]. Despite the substantial investment in reducing losses, the effectiveness of these interventions remains limited due to a lack of coordination among different FCS actors, the failure to improve infrastructure, and inadequate support for capacity building [24]. Therefore, we aim to measure the interaction between socioeconomic characteristics and stakeholders’ practices, which represents an important step in designing appropriate interventions to minimize this share at different nodes across the FSC.

The novelty of the current work could be highlighted through its theoretical and empirical contribution to a better understanding of the root causes and drivers of FLW at the small stakeholder level. This includes assessing the impacts of socioeconomic characteristics heterogeneity among stakeholders on access to logistics services and its effects on FLW reduction. This study presents evidence-based findings on how socioeconomic characteristics and their interaction with other technological factors influence the percentage of FLW across FSC in developing countries. To analyze the FLW drivers, we started with farmers’ practices during farm operations, then the middlemen handling the product to reach the end users. The following sections include the methodology, data analysis, results, discussion, and conclusion.

2. Materials and Methods
2.1. Theoretical Framework
The reduction of food loss in agricultural supply chains is fundamentally dependent on the intricate interaction of social and economic behaviors demonstrated by farmers and intermediaries. These participants function within a network of incentives, limitations, and relational dynamics that significantly affect post-harvest losses. Grasping this relationship is essential for creating effective interventions [24]. For example, trust between farmers and intermediaries promotes an exchange of market information, where intermediaries disseminate market standards and demand signals, and farmers communicate production difficulties. This openness fosters improved planning and coordination to synchronize harvests with market requirements and minimize mismatch losses [19]. Furthermore, trust and strong networks lower transaction costs, enable collective investment in loss-reducing infrastructure, improve access to credit and information, and strengthen bargaining power, making economically viable solutions more accessible. Long-term relations encourage collaboration, where the intermediaries might provide credit for agro-inputs that mitigate losses (such as cold storage and transportation) or provide technical support; farmers tend to prioritize working with trusted partners, which may improve quality control.

The target-measure-act framework has been employed to analyze and measure the impacts of stakeholders’ or individuals’ practices as a food loss driver. This approach has been approved as a recognized approach for developing a rapid result for FLW reduction [25,26]. This study intends to evaluate the interaction between socioeconomic characteristics and the stakeholders’ practices as food loss drivers across FSC to provide a better understanding of how these factors interact. We target the most important actors across FSC who are responsible for the highest share of FLW (farmers and middlemen). Also, the grapes have been considered the main fruit crop in the investigated area. We measured the impacts of these interactions on the stakeholders by employing the rational choice theory, where the stakeholders’ decisions are based on the interaction between the availability, access, and utilization of the facilities and technologies that reduce FLW, and the socioeconomic characteristics of those stakeholders. Finally, the appropriate interventions have been discussed based on the study’s results, as shown in


