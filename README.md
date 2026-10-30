# Smart India Hackathon Workshop
# Date:
## Reference Number:
## Name:

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
1. Detailed explanation of the proposed solution
2. How it addresses the problem
3. Innovation and uniqueness of the solution
1. Detailed explanation
We propose KisanDirect, a mobile-first digital marketplace for three user groups: farmers/FPOs, consumers and bulk buyers (restaurants, retailers, institutions).

Farmers/FPOs list produce by voice or photo in their regional language. They get AI-suggested fair prices and a live buyer demand view.
Consumers and bulk buyers order directly, either as one-off purchases or as subscription baskets, with the farm source shown.
Logistics layer: produce moves from farm to village collection points to local hubs to the buyer. Orders are pooled so vehicles travel full.
AI engine: demand forecasting, price recommendation, and route/load optimisation.
Transparent payments: UPI settlement goes straight to the farmer’s account, with an itemised price breakup (farmer share, logistics, platform fee).
## Technical Approach
Remove These Lines
1. Technologies to be used (e.g. programming languages, frameworks, hardware)
2. Methodology and process for implementation <b>(Flow Charts/Images/ working prototype)</b>
1. Technologies

Frontend: React Native (Android app) plus a React web dashboard for bulk buyers and FPOs; multilingual with speech-to-text.
Backend: Node.js/Express or FastAPI, PostgreSQL (orders, users), Redis (caching), MongoDB (listings).
AI/ML: Python, scikit-learn/XGBoost and Prophet/LSTM for demand and price forecasting; Google OR-Tools for route optimisation; a lightweight CNN (MobileNet) for produce quality grading.
Data sources: Agmarknet/eNAM mandi prices, IMD weather data, historical order data.
Payments and maps: UPI/Razorpay, Google Maps/OpenStreetMap APIs.
Cloud and DevOps: AWS/Azure, Docker, CI/CD, SMS/WhatsApp notifications for low-data users.

2. Methodology and process

Farmer/FPO lists produce (voice/photo)
        ↓
AI quality grading + price suggestion
        ↓
Consumer / bulk buyer places order
        ↓
Order pooling by region + demand forecast update
        ↓
Route optimisation → pickup → collection hub → delivery
        ↓
UPI payment released to farmer (itemised breakup)
        ↓
Ratings + data feedback → improves AI models
<img width="2720" height="2640" alt="kisandirect_technical_flow" src="https://github.com/user-attachments/assets/c0787095-94ca-4ca4-bcce-15002466be45" />

## Feasibility and Viability
Remove These Lines
1. Analysis of the feasibility of the idea
2. Potential challenges and risks
3. Strategies for overcoming these challenges
   1. Feasibility

Technical: all components use mature, open-source tools and public data (Agmarknet, eNAM, weather).
Operational: FPOs (thousands already registered in India) provide ready aggregation points.
Economic: revenue comes from a small commission (2-5%), delivery fees and subscription plans for bulk buyers, which is far below the margin middlemen take.
Alignment: fits the existing digital ecosystem (UPI, ONDC, Agristack) and government schemes for FPOs.

2. Challenges and risks

Low digital literacy and patchy connectivity in rural areas
Perishable goods and last-mile logistics cost
Trust, since farmers may fear non-payment and buyers fear quality issues
Resistance from existing traders
Cold-start problem: a marketplace needs both farmers and buyers at once

3. Strategies to overcome

Voice/vernacular UI, SMS and offline mode, plus village-level “Kisan Mitra” agents
Collection hubs and pooled delivery; partner with existing logistics providers
Escrow-style payments (buyer pays up front, farmer is paid on delivery confirmation) and AI grading with ratings
Start with cooperative FPOs and fixed-demand buyers rather than competing with traders head-on
Pilot in one district, anchor with bulk buyers (hostels, canteens, retailers) first, then expand

## Impact and Benefits
Remove These Lines
1. Potential impact on the target audience
2. Benefits of the solution (social, economic, environmental, etc.)
3. 1. Potential impact on target audience

Farmers/FPOs: higher realised income, price knowledge, less distress selling.
Consumers: fresher produce at lower prices with traceable origin.
Bulk buyers: reliable, predictable supply at negotiated rates.

2. Benefits

Economic: higher farmer share of the consumer rupee and lower retail prices; rural job creation (hub operators, delivery partners).
Social: financial inclusion through direct digital payments; empowerment of small and marginal farmers and women-led FPOs.
Environmental: less food wastage, fewer empty-vehicle trips and lower emissions through optimised routes.
Systemic: data-driven supply planning that reduces price volatility.

## Research and References
Remove These Lines
1. Details / Links of the reference and research work
2. eNAM: National Agriculture Market, enam.gov.in
Agmarknet (mandi price data), agmarknet.gov.in
ONDC: Open Network for Digital Commerce, ondc.org
Agristack / Digital Agriculture Mission, Ministry of Agriculture & Farmers Welfare
Ministry of Consumer Affairs price monitoring (Department of Consumer Affairs)
Scheme for formation and promotion of 10,000 FPOs, Government of India
Google OR-Tools documentation (vehicle routing), developers.google.com/optimization
