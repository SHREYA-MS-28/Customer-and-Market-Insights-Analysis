#  Analysing Customer Behaviour in a Multichannel Gift Retailer  

##  Project Overview  
This project analyzes **100,051 customer records** from a national multichannel gift company (Retail, Internet, and Catalog channels) between **2001–2007**. The aim was to understand **channel loyalty, store trade area effects, gifting behaviour, and seasonal purchasing patterns**.  

By applying **multinomial predictive modelling, RFM analysis, clustering, and STP frameworks**, the study provides actionable insights to strengthen customer loyalty, reduce seasonal dependence, and optimize marketing strategies across channels.  

---

##  Methodology  
- **Data Preparation**  
  - Cleaned and imputed missing demographic/psychographic data (age, income, store distance).  
  - Created new features: lifetime spend by channel, RFM scores, gifting intensity.  
  - Capped outliers and flagged VIP customers.  

- **Analytical Approaches**  
  1. **Channel Loyalty & Switching**  
     - Transition matrix (2004 → 2007) + Multinomial Logistic Regression.  
     - Found **Retail customers most loyal (88.3%)**, while Internet had highest switching (25%).  
  2. **Trade Area Analysis**  
     - RFM + ANOVA across distance bins (0–10 km → 31+ km).  
     - Customers closer to stores spent **$28 more in Retail**, while distant customers preferred Catalog.  
  3. **Gifting Segmentation**  
     - K-means clustering (k=4, silhouette = 0.514).  
     - Segments: *Casual Gifters, Catalog Champions, Online Experimenters, Digital Power Buyers*.  
  4. **Seasonality & STP Strategy**  
     - Logistic regression predicting Spring buyers.  
     - Segments: *Fall-only, Spring-only, Mixed, Inactive*.  
     - Found Spring buyers skewed younger, urban, and digital-first.  

---

##  Key Findings  
- **Channel Dynamics:** Retail loyalty strongest, Internet showed highest switching between Catalog and Retail.  
- **Geographic Impact:** Store distance significantly influenced channel preference and spend.  
- **Segmentation:** Clear behavioural clusters emerged, with **Digital Power Buyers** driving the most value.  
- **Seasonality Risk:** Nearly **47% of customers buy only in Fall/Christmas**, but Spring offers major untapped growth potential.  

---

##  Recommendations  
1. **Nurture Loyalty by Channel** – Retail: exclusive in-store perks; Internet: personalization & subscriptions; Catalog: integrate digital touchpoints.  
2. **Target by Distance** – Nearby: in-store events; Distant: bundled offers & free delivery thresholds.  
3. **Engage Gift Segments** – Tailor messaging: *Casual Gifters (low-barrier promos), Digital Gifters (personalized online), Catalog loyalists (trust-based), Omni-channel VIPs (exclusive rewards)*.  
4. **Boost Spring Sales** – Seasonal campaigns (Easter, Mother’s Day), proximity targeting, and loyalty incentives to convert Fall-only buyers.  

---

##  Files in this Project  
- `Dataset-2.CSV` → Raw customer dataset (2001–2007).  
- `ANALYSING CUSTOMER BEHAVIOUR REPORT.pdf` → Full detailed report contains all my analysis and findings. 
- `ANALYSING CUSTOMER BEHAVIOUR PRESENTATION.pdf` → Presentation about my findings. 
- `Description and Documentation.pdf` → Dataset metadata and business context.  

---

##  Tools & Techniques  
- **Languages:** R, Python  
- **Methods:** Logistic Regression, Multinomial Models, RFM, K-Means Clustering, ANOVA, Transition Matrices  
- **Frameworks:** CRISP-DM, STP (Segmentation–Targeting–Positioning)  
- **Visualization:** ggplot2, PCA plots, segmentation charts  

---
