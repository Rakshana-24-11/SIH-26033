# Smart India Hackathon Workshop

**Date:** November 25, 2026

**Reference Number:** 26018017

**Name:** Rakshana Priya P A

---

## Problem Title
**SIH 26033: Multiple intermediaries reduce farmers' earnings and increase consumer prices.**

## Problem Creater's Organization:    
Ministry of Consumer Affairs, Food & Public Distribution  

## Theme:  
Agriculture, FoodTech & Rural Development  

---

## Problem Description

**Expected Solution:** Create a digital marketplace that:
* Connects farmers/FPOs directly with consumers and bulk buyers.
* Provides logistics support.
* Uses AI for demand forecasting and route optimization.

**Benefits:**
* Better prices for farmers.
* Lower prices for consumers.
* Reduced supply chain inefficiencies.

---

## Proposed Solution

### 1. Detailed Explanation of the Proposed Solution
We propose **Farmer Near Me**, an AI-powered hyperlocal digital marketplace and community platform that directly connects registered local farmers and Farmer Producer Organizations (FPOs) with nearby consumers and bulk buyers.

* **Hyperlocal Discovery & Fair Ranking:** Using real-time geolocation, the app displays nearby registered farmers, their produce, and transparent farm-gate prices. A built-in review and rating system highlights top-rated farmers for crop quality, while **newly registered farmers (without ratings yet) are prioritized at the top of discovery suggestions** so they get fair visibility and initial orders.
* **Streamlined Two-Option Fulfillment System:** At checkout, buyers choose between two simple options:
  1. **Self-Pickup (Zero Delivery Fee):** Buyers pay no delivery charges and receive an in-app navigation route directly to the farmer’s farm or pickup point.
  2. **Home Delivery (Automated Farmer-Preference Routing):** When a buyer selects delivery, the system automatically checks the farmer's fulfillment preference:
     * *If the farmer offers self-delivery:* The order is assigned to the farmer, who earns 100% of the delivery charge.
     * *If the farmer does not have delivery capability:* The system automatically dispatches the nearest online gig delivery partner (operating on a flexible model—no physical reporting hub required; drivers simply turn on location, log in, accept nearby pings during their day, and receive instant payouts per delivery).
* **Dual AI Assistants (Farmer & Buyer Co-Pilots):**
  * **Farmer AI Assistant:** Provides hyperlocal AI weather forecasts and actionable crop/harvest advisories, alongside a conversational AI chat box (with regional language/voice support) to answer farming, pricing, and platform queries.
  * **Buyer AI Assistant:** An interactive AI chat box where buyers can ask questions about the nutritional value, freshness, and usage of the produce they plan to buy, get smart shopping suggestions, and discover dishes they can cook with those ingredients.
* **Farm-to-Table Social Media Feed:** An interactive community feed where both farmers and buyers can share posts, photos, traditional recipes, dishes made from fresh produce, and the health/cultural importance of local crops—driving organic engagement and trust.

### 2. How It Addresses the Problem
* **Eliminates Middlemen:** Direct farmer-to-buyer transactions remove commission agents and wholesale brokers, ensuring farmers keep the full value of their harvest while buyers get fair prices.
* **Seamless Last-Mile Logistics:** Independent gig drivers act strictly as transport carriers rather than price-inflating middlemen, ensuring buyers always get doorstep delivery even when small farmers lack vehicles.
* **Reduces Spoilage & Boosts Demand:** AI weather alerts help farmers time harvests, while the Buyer AI chat and social recipe feed educate consumers on how to use seasonal local crops—increasing sales velocity and minimizing waste.

### 3. Innovation and Uniqueness of the Solution
* **New-Farmer Boost Algorithm:** Solves the "cold-start problem" in marketplace ratings by featuring new farmers first alongside proven top-rated farmers.
* **Zero-Friction Smart Dispatch:** Buyers aren't bogged down by logistics complexity—they simply pick *Delivery* or *Pickup*, and the backend dynamically routes based on farmer capability and gig-driver proximity.
* **Social Commerce + Dual AI Integration:** Combines a hyperlocal agri-marketplace with a recipe-driven social feed and dedicated AI assistants tailored separately for agricultural production (weather/crop queries) and household consumption (nutrition/cooking ideas).

---

## Technical Approach

### 1. Technologies to be Used
* **Frontend (Mobile App):** Flutter or React Native (cross-platform Android/iOS with regional multilingual and voice-input support).
* **Backend & APIs:** Node.js (Express) or Python (FastAPI) for real-time order routing, social feed APIs, and instant UPI payouts.
* **Database & Media Storage:** PostgreSQL with PostGIS (geospatial radius queries and ranking logic), Redis (real-time gig-driver location tracking), and AWS S3 / Firebase Storage (social feed images/videos).
* **Generative AI & ML:** LLM APIs (e.g., Gemini API) for the Farmer & Buyer AI chat assistants and recipe recommendations; Weather APIs + ML models for localized weather insights, demand forecasting, and Google OR-Tools for route optimization.
* **Maps & Navigation:** Google Maps Platform (Geolocation, Turn-by-Turn Pickup Routing, and Delivery Distance Matrix).
* **Payments:** Razorpay / UPI Intent API for automated instant split-settlements to farmers and gig drivers.

### 2. Methodology and Process for Implementation

<img width="357" height="714" alt="WhatsApp Image 2026-11-25 at 6 27 14 PM" src="https://github.com/user-attachments/assets/535c74e9-5d05-4c2b-b340-289451e915a5" />
<img width="357" height="714" alt="WhatsApp Image 2026-11-25 at 6 27 15 PM" src="https://github.com/user-attachments/assets/371ca586-e640-4523-944d-06acc95d1a63" />

1. **Onboarding & Verification:** OTP-based registration for farmers (Kisan/FPO verification) and gig delivery workers (KYC and vehicle verification).
2. **AI-Assisted Listing & Social Engagement:** Farmers check AI weather advisories, list daily harvest stock, and share crop stories/recipes on the social feed.
3. **Discovery & Buyer AI Consultation:** Buyers browse nearby farms (ranked with new farmers prioritized alongside top-rated ones), consult the Buyer AI chat for dish ideas, and add items to cart.
4. **Smart Fulfillment & Payout:**
   * *Pickup:* App generates the optimal map route to the farm.
   * *Delivery:* Backend checks farmer delivery preference -> assigns to farmer OR pings nearest online gig driver within 3–5 km -> triggers instant UPI payout upon delivery.
---

## Feasibility and Viability

### 1. Analysis of the Feasibility of the Idea
* **Technical Feasibility:** Built on mature geospatial, UPI, weather, and LLM APIs that operate reliably on standard smartphones.
* **Operational Feasibility:** Asset-light model requiring zero warehouses or dark stores; utilizes existing local farmers and flexible part-time gig workers.
* **Economic Viability:** Monetized through a nominal platform fee on bulk/retail transactions while keeping core listings, AI weather alerts, and social features free for farmers.

### 2. Potential Challenges and Risks
* **Digital Literacy & Language Barriers:** Farmers may find typing queries or creating social posts difficult.
* **Low Gig-Driver Density in Remote Villages:** Fewer active delivery partners in deeply rural areas compared to towns and cities.
* **Spam or Misleading Social/Review Content:** Fake reviews or off-topic posts on the community feed.

### 3. Strategies for Overcoming These Challenges
* **Voice-First Regional AI Interface:** Allow farmers to speak to the AI assistant and post produce/recipes using voice-to-text in their native language.
* **FPO Hub Aggregation & Farmer Self-Delivery:** Leverage farmers with local vehicles and village FPO collection points to cover rural last-mile deliveries.
* **Verified-Purchase Reviews & AI Moderation:** Restrict ratings strictly to completed orders and use automated AI moderation to keep the social feed focused on food, farming, and recipes.

---

## Impact and Benefits

### 1. Potential Impact on the Target Audience
* **Farmers:** Higher profit margins (20%–40% increase) by selling directly, climate resilience through AI weather alerts, equal opportunity for newcomers via discovery boosting, and extra delivery income.
* **Consumers & Bulk Buyers:** Access to fresh, traceable local produce at lower prices, paired with AI meal inspiration and transparent farmer ratings.
* **Local Youth / Gig Workers:** Flexible, zero-commitment local earning opportunities with instant per-trip payouts.

### 2. Benefits of the Solution
* **Economic:** Keeps agricultural wealth inside local communities and generates decentralized gig employment.
* **Social:** Builds direct trust between farmers and families through shared food culture, recipes, and transparent reviews.
* **Environmental:** Hyperlocal farm-to-home routes drastically reduce carbon emissions from long-distance transport and cut post-harvest food waste.

---

## Research and References

Aditya, K.S., Subash, S.P., Praveen, K.V., Nithyashree, M.L., Bhuvana, N. andSharma, A. (2017.)Awareness about Minimum Support Price and Its Impact onDiversification Decision of Farmers in India.Asia and the Pacific Policy Studies, 4(3): 514-526.
