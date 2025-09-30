#  Customer Lifetime Value Strategy for Python Logistics

This repository contains a project analyzing **customer valuation and targeting strategies** for Python Logistics, a trucking company serving supermarkets. With limited trucking capacity, Python Logistics must identify its most valuable customers, allocate resources efficiently, and design differentiated strategies using **RFM analysis, choice models, and customer lifetime value (CLV) estimation**.

---

##  Business Context
Python Logistics operates a mixed fleet:
- **Large trucks** → transport goods from warehouses to retail stores.  
- **Small trucks** → handle home deliveries for online orders.  
- Products: **Perishables** (vegetables, meat, dairy) & **Non-perishables** (paper goods, coffee, personal care).  
- **Challenge**: Limited number of trucks → need to prioritize the most profitable supermarket chains.

**Key Goals**
1. Identify most valuable supermarket customers.  
2. Allocate limited trucking resources efficiently.  
3. Treat customers differently when designing marketing and service strategies.  

---

##  Objectives
- Apply **RFM (Recency, Frequency, Monetary) model** to rank supermarket chains.  
- Use **choice models** for granular targeting and probability-based segmentation.  
- Develop a **transition matrix + discounting approach** to calculate Customer Lifetime Value (CLV).  

---

##  Methodology & Models

###  RFM Model – Scoring Criteria
- **Recency**: How recently orders were placed (perishable orders prioritized).  
- **Frequency**: Orders per store in the chain (adjusted for chain size).  
- **Monetary**: Logistics revenue (weighted by order profitability; perishable deliveries > dry goods).  

**Scoring (1–5 scale)**  
- Recency: 0–7 days = 5, >30 days = 1  
- Frequency: ≥1.5 orders/store = 5, <0.5 = 1  
- Monetary: ≥$100,000 = 5, <$25,000 = 1  

 This ranking highlights **high-value, time-sensitive, and profitable chains** for priority truck allocation.  

---

###  Choice Models – Granular Targeting
- Logistic regression / multinomial logit used to predict probability of future profitable engagement.  
- Inputs: Recency of perishable orders, frequency per store, high-margin delivery revenue.  
- Outputs: **Choice score** per customer → probability-driven ranking.  

**Targeting Strategy**
- **Top deciles** → Priority allocation + personalized marketing.  
- **Middle deciles** → Service incentives.  
- **Lower deciles** → Minimal engagement.  

---

###  Customer Lifetime Value (CLV) via Transition Matrix
- **Transition matrix** → Models probability of customers shifting across segments (Gold → Silver → Lost).  
- **Absorbing state**: "Lost" = no future revenue.  
- Apply **discount rates** to adjust future revenues → present value of expected profits.  
- Enables **risk-adjusted CLV estimation** and long-term strategic planning.  

---

##  Key Findings
- RFM provides a **baseline scoring system** for supermarkets.  
- Choice models deliver **probability-driven targeting** → more precise than RFM alone.  
- Transition matrix + discounting allows **forward-looking CLV estimates** → helps optimize customer retention and growth.  

---

##  Strategic Implications
- Align trucks and resources with **highest-value supermarket partners**.  
- Use CLV insights to **prioritize long-term profitable relationships**.  
- Reduce wasted logistics capacity by **de-prioritizing low-value chains**.  
- Support **differentiated marketing strategies** for each customer group.  

---

##  Repository Contents
- `report/CUSTOMER LIFETIME VALUE STRATEGY REPORT.pdf` → Full report  
- `CLV CASE STUDY` → Contains the questions and scenario of the case study    
- `README.md` → This file  

---

##  Tools & Techniques
- **RFM Model** → Customer ranking  
- **Choice Models** → Logistic regression, multinomial logit  
- **Transition Matrix** → Segment evolution modeling  
- **Discounting** → Net Present Value of customer revenue streams  

---

##  Conclusion
This project demonstrates how Python Logistics can combine **RFM scoring, choice models, and CLV estimation** to maximize truck utilization, allocate resources effectively, and strengthen partnerships with its most profitable customers. The framework is adaptable to any logistics company seeking to improve **customer prioritization and lifetime value management**.  

---

##  References
- Lilien, G. L., Rangaswamy, A., & De Bruyn, A. (2017). *Principles of Marketing Engineering and Analytics* (3rd ed.). DecisionPro.  
- Iacobucci, D., & Churchill, G. A. (2018). *Marketing Research: Methodological Foundations* (12th ed.). CreateSpace.  
- Lilien, G. L., Kotler, P., & Moorthy, K. S. (2007). *Marketing Models*. Trafford.  
- IBM SPSS Statistics Documentation.  
