#  Pricing Strategy Design for Zach’s Garage using Gabor-Granger Analysis

This repository presents a **data-driven pricing analysis** for Zach’s Garage, a grassroots live music venue in Chicago. The study applies the **Gabor-Granger method** to estimate ticket price sensitivity and simulate different pricing strategies that balance **financial sustainability** with Zach’s mission of inclusivity and community engagement.

---

##  Business Context
- **Venue**: Zach’s Garage – grassroots, inclusive live music space.  
- **Mission**: Support local artists & keep concerts accessible to all income levels.  
- **Problem**: Despite popularity (10k+ fans, frequent sellouts), Zach faces a **$3,000 monthly deficit** plus rising costs (safety, legal, equipment).  
- **Challenge**: Design a **long-term pricing strategy** without alienating students or low-income fans.  

---

##  Objectives
1. Identify the **revenue-maximizing ticket price**.  
2. Estimate the **price point at which attendance halves**.  
3. Determine the **break-even ticket price** to cover costs.  
4. Explore **free admission for youth (≤21)** and optimal adult pricing.  
5. Assess **youth discounts** versus free entry for long-term inclusivity.  

---

##  Methodology
- **Pricing Method**: Gabor-Granger pricing model.  
- **Survey Data**: Likelihood of attendance at ticket prices $1, $3, $5, $8, $12, $20.  
- **Conversion**: 5-point likelihood scale mapped to attendance probabilities.  
- **Tool**: Enginius Pricing Optimization (logit model with strong fit: BIC = 689.19, R² = 0.3873).  
- **Market Size**: 3,000 attendees per month (250 per event × 12 events).  
- **Costs**: $3,000/month fixed operating deficit.  

---

##  Findings

###  Optimal Flat Pricing
- Best single-price strategy: **$3.31 per ticket**.  
- Forecast: ~1,439 attendees/month.  
- Revenue: ~$4,768 → Gross Profit: ~$1,768.  

###  Attendance Drop-Off
- At ~$3, attendance falls from 250 to ~125 per event.  
- Price sensitivity becomes steep beyond this threshold.  

###  Break-Even Pricing
- Break-even at ~$1.45–$1.50 per ticket.  
- Just enough to cover monthly $3,000 costs.  

###  Free Entry for Youth
- Adults optimally priced at ~$3.57.  
- Revenue: ~$3,659 → Profit: ~$659.  
- Attendance: ~2,024 (including 1,000 youth free).  

###  Youth Discounts
- Youth tickets at **$2.60** → adds ~$1,167 profit.  
- Combined strategy: ~$1,826 profit, ~1,474 total attendees.  
- Slightly more profitable than flat pricing (+3.3%).  

---

## Strategic Recommendations
- **Option 1: Tiered Pricing**  
  - $2.00 for adults, $1.00 for youth.  
  - Balanced sustainability + inclusivity.  

- **Option 2: Flat-Rate Pricing**  
  - $1.50 uniform ticket.  
  - High attendance, breakeven guaranteed.  

- **Option 3: Adults Only**  
  - Youth free, adults $2.00.  
  - Minimal profit, strong inclusivity, and community growth.  

**Conclusion**: Unless Zach shifts toward profit maximization, **community-first models (Options 1 or 2)** are most aligned with his mission. These ensure sustainability while preserving inclusivity and long-term brand equity.  

---

##  Repository Contents
- `PRICING STRATEGY DESIGN USING GABOR-GRANGER ANALYSIS.pdf` → Full project report contains my findings and analysis 
- `CASE STUDY.pdf` → Case study brief and scenario analysis  
- `README.md` → This file  

---

##  Tools & Techniques
- **Gabor-Granger Analysis** → Price sensitivity testing  
- **Enginius Pricing Optimization** → Model fitting, revenue simulation  
- **Scenario Analysis** → Flat, tiered, discounted pricing  
- **Segmentation** → Adult vs. youth strategies  

---

##  Conclusion
The Gabor-Granger analysis shows Zach can achieve sustainability with **modest ticket prices** while staying true to his mission of inclusivity. Flat or tiered pricing ensures financial stability, community engagement, and long-term growth of Zach’s Garage as a hub for grassroots music.  

---

##  References
- De Bruyn, A. (2016). *Zach’s Garage Case Study*. DecisionPro.  
- Gabor, A., & Granger, C. (1966). *Price Sensitivity of Consumers*.  
- Lilien, G. L., Rangaswamy, A., & De Bruyn, A. (2017). *Principles of Marketing Engineering and Analytics*.  
