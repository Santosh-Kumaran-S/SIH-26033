# Smart India Hackathon Workshop
# Date: 22/11/2026
## Reference Number: 26005061
## Name: Santosh Kumaran S

## Problem Title:
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization:
Ministry of Consumer Affairs, Food & Public Distribution

## Theme:
Agriculture, FoodTech & Rural Development

## Problem Description:
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution:

## Voice-Enabled Smart Agricultural Marketplace:

We propose a **Voice-Enabled Smart Agricultural Marketplace** that connects farmers, Farmer Producer Organizations (FPOs), retailers, wholesalers, consumers and transport providers through an accessible digital platform. The solution is specifically designed to support small-scale farmers and rural users who may not own smartphones or have the digital literacy required to use mobile applications.

Instead of forcing farmers to interact with complex mobile apps, the platform enables them to access marketplace services using a basic keypad mobile phone through toll-free calls, Interactive Voice Response (IVR), and SMS.

### 1. Accessible Farmer Registration Through Basic Mobile Phones
Farmers can register on the platform using a simple phone call to a dedicated toll-free number. The system supports regional languages such as Tamil and provides voice-guided instructions, eliminating the need for smartphones, internet connectivity, app installations or typing skills.

During registration, farmers can provide basic details such as their name, village, phone number and preferred language. Their phone number can serve as their primary identification for accessing marketplace services.

### 2. Voice-Based Crop Listing and Selling
Farmers can list their agricultural produce through a guided voice call. The system prompts them to select the crop, enter the available quantity, specify their expected price and confirm their pickup location using simple keypad inputs or voice responses.

The listing is automatically converted into a digital product entry and made visible to registered buyers on the marketplace. Farmers can update or remove their listings through subsequent calls.

### 3. Direct Farmer-to-Buyer Marketplace
The platform provides a centralized digital marketplace where consumers, retailers, restaurants, wholesalers and FPOs can discover agricultural products directly from farmers.

Buyers can filter produce based on crop type, quantity, location, price and availability. By reducing unnecessary intermediaries, the platform encourages transparent pricing, enables farmers to receive better returns and helps buyers procure fresh produce at competitive prices.

### 4. Automated Buyer Matching and Notifications
An intelligent matching system identifies suitable buyers for each farmer's listing based on location, quantity requirements, crop type, price expectations and demand.

When a matching buyer is identified, the farmer receives a voice call or SMS notification in their preferred language containing the buyer's offer, quantity, price and order details. Farmers can accept or reject the offer using simple keypad responses, making the process accessible without app usage.

### 5. Smart Logistics and Shared Transportation
To address transportation difficulties and high delivery costs, the platform integrates logistics support for agricultural produce.

The system identifies nearby farmers with compatible produce, pickup locations and delivery destinations, and groups their orders whenever feasible. It can connect them with local transport providers and generate optimized collection and delivery routes to reduce travel distance, fuel consumption, delays and transportation expenses.

Farmers can receive pickup schedules and delivery confirmations through voice calls or SMS.

### 6. AI-Powered Demand Forecasting and Price Intelligence
Artificial Intelligence analyzes historical sales, market prices, seasonal patterns, regional demand and buyer activity to estimate upcoming demand for agricultural products.

The system provides farmers with simplified voice-based insights such as:

- Crops with increasing demand in nearby markets.
- Approximate prevailing market price ranges.
- Demand trends that may help farmers plan production.
- Market locations where their produce may receive better demand.

These insights are delivered in simple regional-language messages rather than complex graphs or analytics dashboards.

### 7. Digital Support for Buyers and Administrators
While farmers interact primarily through basic phones, buyers, FPO representatives, logistics providers and administrators can use a smartphone or web dashboard to manage listings, orders, buyer requests, transport coordination, payments and marketplace activity.

This creates a dual-interface system: a simple voice interface for farmers and a full digital interface for other stakeholders.

### 8. Order Confirmation and Trust Mechanism
Once a buyer places an order, the farmer receives an automated voice call or SMS with the order details. Both parties receive confirmation of the agreed quantity, price, pickup schedule and delivery status.

The platform maintains digital records of transactions, buyer and seller activity, order completion and feedback, improving transparency, accountability and trust in the agricultural trading process.

### Expected Impact

- **Improved accessibility:** Farmers can participate in digital commerce without smartphones or advanced digital skills.
- **Better farmer income:** Direct access to buyers reduces dependency on multiple intermediaries.
- **Affordable produce:** Consumers and bulk buyers can benefit from reduced unnecessary supply-chain costs.
- **Efficient logistics:** Aggregated orders and optimized routes reduce transportation costs and wastage.
- **Data-driven agriculture:** AI-based demand and price insights support informed selling and cultivation decisions.
- **Inclusive digital transformation:** Rural farmers can benefit from digital technology using communication devices they already own.

The proposed system transforms a conventional agricultural marketplace into an inclusive, voice-accessible agricultural ecosystem where technology adapts to farmers' needs instead of requiring farmers to adapt to technology.

## Technical Approach:

### 1. System Architecture
The system will be developed using a dual-interface architecture that accommodates both farmers using basic mobile phones and buyers using smartphones or web applications. Farmers will interact through an IVR-based voice communication system, while buyers, FPOs, transport providers and administrators will access a digital marketplace dashboard.

### 2. Farmer Communication Layer (IVR & Telephony)
- Integrate a cloud telephony service to provide a dedicated phone number for incoming and outgoing calls.
- Implement an Interactive Voice Response (IVR) system to guide farmers through marketplace operations using keypad inputs (DTMF) and pre-recorded regional-language prompts.
- Enable farmers to register, list produce, enter quantities, hear price information, accept/reject buyer offers and receive order updates using basic phones.
- Use speech-to-text and text-to-speech services optionally to support voice-based inputs and responses, with keypad navigation as a reliable fallback.
- Deliver SMS confirmations and notifications to farmers for orders, prices and pickup schedules.

### 3. Marketplace Application Layer
- Develop a web-based marketplace for buyers, retailers, wholesalers and consumers to browse produce and place orders.
- Implement farmer listings containing crop name, quantity, expected price, location, availability and contact identification.
- Provide search, filtering, order management and buyer-farmer matching functionality.
- Create a farmer management dashboard for FPOs and administrators to assist farmers who need support with listing or transaction management.

### 4. Backend & API Development
- Develop backend services using Python with FastAPI to handle farmer registrations, product listings, buyer requests, order processing, notifications and logistics.
- Create REST APIs to connect the IVR telephony system, marketplace frontend, AI services and database.
- Implement authentication and role-based access control for farmers, buyers, FPOs, transport providers and administrators.
- Maintain transaction records, listing updates and order status through a centralized backend.

### 5. Database Management
- Use PostgreSQL to store farmer profiles, crop listings, buyer information, orders, location details, logistics information and transaction records.
- Store geospatial information using PostGIS to identify nearby farmers, buyers, collection points and transport routes.
- Maintain historical sales, crop availability, price and demand data to support AI prediction services.

### 6. AI & Machine Learning Integration
- **Demand Forecasting:** Use historical sales, seasonal patterns, market prices and regional demand data to predict upcoming demand for agricultural products.
- **Price Intelligence:** Analyze local market price trends to provide farmers with estimated price ranges and market comparison information.
- **Buyer Matching:** Match farmers' listings with buyers based on crop type, quantity, location, price and delivery requirements.
- **Route Optimization:** Use location data and routing algorithms to group nearby pickups and optimize transport routes, reducing travel distance and delivery costs.

### 7. Logistics & Transportation Module
- Integrate mapping and routing services to calculate distances between farms, collection points, buyers and markets.
- Group compatible orders from nearby farmers to enable shared transportation.
- Generate optimized pickup and delivery sequences based on quantity, vehicle capacity, destination and time constraints.
- Notify farmers and transport providers about pickup schedules and order progress through calls and SMS.

### 8. Notification & Order Management
- Integrate SMS and automated voice calls for farmer notifications.
- Buyers can place orders through the marketplace and farmers can confirm orders through keypad responses.
- Track order stages such as order placed, farmer confirmation, pickup scheduled, in transit and delivered.
- Provide transaction logs and order history for transparency and dispute resolution.

### 9. Deployment & Security
- Deploy backend services and marketplace frontend on cloud infrastructure.
- Use encrypted communication (HTTPS), secure authentication, role-based permissions and protected storage of personal data.
- Implement database backups, API validation, rate limiting and audit logs to protect the platform from misuse and unauthorized access.
- Design backend services to be scalable as the number of farmers, buyers and transactions increases.

### End-to-End Technical Workflow

1. Farmer calls the platform's toll-free number.
2. Telephony service routes the call to the IVR system.
3. Farmer selects a language and marketplace action through voice prompts and keypad inputs.
4. IVR sends the input to the backend through API requests.
5. Backend validates the information and stores the listing in PostgreSQL.
6. AI services identify suitable buyers and analyze market demand.
7. Buyer receives the listing and places an order through the marketplace.
8. Farmer receives a voice call/SMS and confirms or rejects the offer.
9. Logistics module aggregates nearby orders and calculates pickup routes.
10. Order status, pickup instructions and delivery confirmation are communicated to both parties.

**Proposed Technology Stack**

| Component | Technology |
|---|---|
| Farmer communication | IVR, DTMF, SMS, cloud telephony API |
| Voice processing | Regional-language TTS / speech recognition |
| Buyer frontend | React / Next.js |
| Backend | Python, FastAPI, REST APIs |
| Database | PostgreSQL |
| Geospatial processing | PostGIS |
| AI / ML | Python, Scikit-learn, forecasting models |
| Route optimization | OR-Tools, routing / mapping APIs |
| Notifications | SMS API, automated voice calls |
| Cloud deployment | Cloud hosting, Docker |

The architecture prioritizes low-bandwidth communication, accessibility, modular development, scalability and cost-efficient agricultural logistics.

### USER FLOW DIAGRAM:


flowchart TD
    A([Start]) --> B{User Type}

    B -->|Farmer| C[Dial Toll-Free Number]
    C --> D[IVR Voice Menu]
    D --> E[Select Language]
    E --> F{Choose Service}

    F -->|Register| G[Enter Farmer Details]
    F -->|Sell Produce| H[Select Crop]
    F -->|Check Price| I[Request Market Price]
    F -->|Orders| J[Check Order Status]

    G --> K[Backend API]
    H --> L[Enter Quantity and Expected Price]
    L --> M[Confirm Produce Listing]
    M --> K

    I --> K
    J --> K

    K --> N[(Database)]
    K --> O[AI Processing Engine]

    O --> P[Demand Forecasting]
    O --> Q[Buyer Matching]
    O --> R[Price Intelligence]

    P --> S[Marketplace]
    Q --> S
    R --> T[Voice / SMS Response]
    T --> U[Farmer Receives Information]

    S --> V[Buyer Web Application]
    B -->|Buyer| V

    V --> W[Browse Produce]
    W --> X[Place Bulk Order]
    X --> Y[Order Processing Backend]

    Y --> Z[Notify Farmer Through IVR / SMS]
    Z --> AA{Farmer Accepts?}

    AA -->|Yes| AB[Confirm Order]
    AA -->|No| AC[Notify Buyer and Find Alternative]

    AB --> AD[Logistics Module]
    AD --> AE[Aggregate Nearby Orders]
    AE --> AF[Route Optimization]
    AF --> AG[Assign Transport]
    AG --> AH[Pickup and Delivery]
    AH --> AI[Order Completed]



## Feasibility and Viability:

### Technical Feasibility
The solution is technically feasible using existing technologies such as IVR-based telephony, SMS services, cloud infrastructure, AI-based demand forecasting, digital marketplaces and route optimization algorithms. Farmers can interact with the system using basic keypad phones through voice-guided regional-language menus, without requiring smartphones or internet connectivity. A centralized backend can integrate farmer listings, buyer orders, notifications, price analysis and logistics coordination. The initial prototype can be developed using existing APIs and open-source technologies, minimizing development complexity and infrastructure requirements.

### Operational Feasibility
The platform can be implemented initially in a selected agricultural region by onboarding a small group of farmers, local buyers, FPOs and transport providers. FPOs and local agricultural coordinators can help farmers register, verify produce availability, assist with voice-based interactions and facilitate transactions. Existing transport services can be integrated instead of establishing a new delivery fleet, making the system easier to deploy and operate.

### Economic Viability
The platform can operate with a low initial investment by using cloud-hosted backend services, open-source software and pay-as-you-use telephony APIs. Revenue can be generated through a small commission on successfully completed transactions, bulk-order facilitation fees, logistics coordination charges and premium services for large-scale buyers. Direct farmer-to-buyer transactions can improve farmers' selling prices while reducing unnecessary intermediary costs and procurement expenses for consumers and bulk buyers.

### Scalability and Sustainability
The system can initially focus on a single region and a limited number of high-demand crops, allowing its operations and matching algorithms to be evaluated before expanding. Its modular architecture enables additional languages, crops, markets, FPOs, buyers and logistics partners to be integrated gradually. Demand forecasting and shared transportation can reduce unsold produce, inefficient trips and avoidable post-harvest losses, contributing to long-term economic and environmental sustainability.

### Key Risks and Mitigation

| Potential challenge | Mitigation strategy |
|---|---|
| Farmers unfamiliar with IVR | Simple voice prompts, local languages and keypad navigation |
| Poor network connectivity | SMS fallback and retry-based listing submission |
| Low buyer participation | Onboard wholesalers, retailers and FPOs during pilot |
| Inaccurate demand forecasts | Start with market data and continuously refine predictions |
| Transport availability | Partner with existing local transport providers |
| Price disputes | Confirm price, quantity and terms before order acceptance |
| Produce quality inconsistency | Buyer-defined quality standards and verification through FPOs/coordinators |
| High call costs | Short IVR sessions, callback options and optimized call workflows |

### Overall Assessment
The proposed solution is feasible with currently available technology, economically viable through a low-cost pilot and transaction-based revenue model, and scalable through gradual regional expansion. Its key strength is that it does not require farmers to adopt complex digital tools; instead, it makes existing digital marketplace infrastructure accessible through ordinary mobile calls and SMS.

## Impact and Benefits:

### 1. Social Impact
- **Digital Inclusivity:** Enables farmers, especially elderly and digitally inexperienced individuals, to access digital marketplace services using basic keypad mobile phones without requiring smartphones, internet connectivity or digital literacy.
- **Empowerment of Farmers:** Gives farmers greater control over selling decisions, buyer selection, price negotiation and market access.
- **Rural Accessibility:** Provides regional-language voice services, making technology accessible to farmers from rural and underserved communities.
- **Reduced Dependency:** Minimizes dependence on intermediaries for market information, buyer discovery and selling agricultural produce.

### 2. Economic Impact
- **Improved Farmer Income:** Directly connects farmers with consumers, retailers, wholesalers and FPOs, enabling better selling prices and reduced intermediary commissions.
- **Reduced Procurement Costs:** Buyers gain access to agricultural produce at competitive prices by sourcing directly from farmers.
- **Lower Transportation Expenses:** Combines produce from nearby farmers and optimizes pickup routes, reducing individual transportation costs.
- **Expanded Market Opportunities:** Enables small-scale farmers to reach buyers outside their local villages and access larger markets.

### 3. Environmental Impact
- **Reduced Food Waste:** Better demand forecasting and faster buyer matching help reduce unsold agricultural produce and avoidable post-harvest losses.
- **Lower Fuel Consumption:** Shared transportation and optimized collection routes reduce unnecessary vehicle trips and fuel usage.
- **Sustainable Supply Chain:** Encourages efficient distribution of agricultural products through data-driven demand planning and logistics coordination.

### 4. Technological Impact
- **AI-Driven Decision Support:** Provides demand forecasts, market price insights and buyer matching to support informed agricultural selling decisions.
- **Inclusive Technology Adoption:** Demonstrates how AI and digital marketplaces can serve users with limited access to advanced devices.
- **Improved Transparency:** Digitally records listings, negotiated prices, orders and delivery status to improve accountability and trust among stakeholders.

### 5. Key Beneficiaries

| Beneficiary | Benefits |
|---|---|
| Farmers | Better market access, fairer prices, simple voice-based usage |
| Consumers | Competitive prices and access to fresh produce |
| Wholesalers & retailers | Reliable sourcing and easier bulk procurement |
| FPOs | Centralized member produce management and improved sales coordination |
| Transport providers | Better vehicle utilization and more organized pickup requests |
| Environment | Reduced wastage, unnecessary trips and fuel consumption |

### 6. Measurable Outcomes
The impact of the solution can be evaluated through a pilot deployment using the following indicators:

- Percentage increase in average farmer selling price.
- Reduction in transportation costs per kilogram of produce.
- Number of farmers successfully onboarded using basic phones.
- Number and value of direct farmer-to-buyer transactions.
- Reduction in unsold produce and post-harvest wastage.
- Order fulfillment rate and average time required to find a buyer.
- Percentage of farmers able to complete transactions without assistance.

### Overall Impact
The proposed solution creates an inclusive, AI-enabled agricultural supply chain that bridges the digital divide, improves farmer income, reduces procurement and logistics inefficiencies, and promotes sustainable food distribution. By making digital commerce accessible through basic mobile phones, it ensures that even farmers with limited technological knowledge can participate in and benefit from the digital economy.

## Research and References:

The proposed solution is supported by existing research on digital agriculture, mobile-based farmer communication, agricultural marketplaces and IVR-based information delivery. These studies demonstrate the importance of accessible communication systems and provide a foundation for developing an inclusive, voice-enabled agricultural marketplace.

**1. Strengthening Kisan Call Centres in India – ICAR-NAARM (2022)**

This research examines India's Kisan Call Centre system and the use of ICT technologies such as SMS, IVRS, mobile applications and toll-free farmer support services. It provides insights into how telecommunication infrastructure can deliver agricultural information and personalized support to farmers.

**Relevance:** Supports the feasibility of using telephone-based and IVR systems to provide accessible agricultural services without requiring smartphone applications.

**2. Comprehensive Analysis of Kisan Call Centre in Tiruchirappalli District, Tamil Nadu (2024)**

This study examines farmers' usage, awareness and experiences with Kisan Call Centres in Tamil Nadu. It identifies communication limitations, language accessibility issues and the need for improved farmer feedback mechanisms.

**Relevance:** Supports the need for simple regional-language voice interaction and a farmer-centric communication system suitable for rural communities.

**3. AI-Based Market Intelligence Systems for Farmer Collectives in India (2023)**

This research describes the implementation of agricultural market intelligence and sales recommendation systems for farmer collectives. It also documents the use of IVR communication for farmers who lack smartphones, demonstrating how agricultural information and market intelligence can be delivered through voice calls.

**Relevance:** Provides a research precedent for combining agricultural market intelligence, digital sales support and basic-phone communication.

**4. A Hybrid Multi-Modal System Using IVR and WhatsApp – CHI 2021**

This study presents a farmer communication and training system combining IVR for feature-phone users and WhatsApp for smartphone users in rural India. The system was used to deliver agricultural information through multiple communication channels.

**Relevance:** Supports the dual-interface approach in which farmers use basic phones while other stakeholders use digital applications.

**5. Kisan Call Centres: A Decision-Oriented Information System for Farmers – IIM Ahmedabad**

This research examines India's Kisan Call Centre initiative and the use of telecommunications for providing agricultural information, answering farmer queries and supporting decision-making.

**Relevance:** Establishes the value of telephone-based agricultural support systems and demonstrates the potential of communication technology to bridge information gaps between farmers and agricultural service providers.
