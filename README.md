# Maven Fuzzy Factory Landing Page A/B Test Analysis

## Project Overview
This project analyzes a landing page A/B test for Maven Fuzzy Factory, an e-commerce company selling children’s toys. The goal was to determine whether a new landing page improved user engagement and conversion performance compared to the original homepage.


## Business Problem
The homepage exhibited a high bounce rate, indicating that a significant portion of users were leaving without engaging further. To address this, the business introduced a new landing page for a segment of paid search traffic and required a data-driven evaluation of its effectiveness.


## Objective
- Evaluate whether the new landing page reduced bounce rate compared to the original homepage  
- Assess whether the improvement was statistically significant  
- Determine if increased engagement translated into higher conversion rates  


## Methodology
- Built a **session-level analytical dataset** by combining website sessions, pageviews, and orders  
- Derived key behavioral metrics:
  - Landing page
  - Pageview count
  - Bounce indicator
  - Conversion indicator  
- Filtered the dataset to the valid A/B test segment:
  - `utm_source = gsearch`
  - `utm_campaign = nonbrand`
  - Defined experiment date range  
- Compared control (`/home`) vs treatment (`/lander-1`) using:
  - Bounce rate
  - Conversion rate  
- Performed a **two-proportion z-test** to validate statistical significance  
- Developed a **dashboard** to present insights and recommendations  


## Tools & Techniques
- Microsoft Excel  
- Power Query (data transformation & modeling)  
- Excel formulas (`COUNTIFS`, calculated metrics)  
- Statistical analysis (z-score, p-value)  
- Dashboard design & data visualization  


## Key Metrics
- Bounce Rate  
- Conversion Rate  
- Absolute & Percentage Lift  
- P-value (statistical significance)  


## Key Findings
- The treatment landing page (`/lander-1`) **reduced bounce rate** compared to the original homepage  
- Conversion rate **improved alongside engagement**, indicating positive business impact  
- The bounce-rate improvement was **statistically significant**, confirming reliability of results  
- Performance gains were **stronger on desktop**, while mobile remained relatively weaker  


## Business Impact
The new landing page not only improved user engagement but also contributed to higher conversions, demonstrating measurable value in optimizing the user entry experience.


## Recommendation
- Roll out `/lander-1` for gsearch nonbrand traffic  
- Continue monitoring post-rollout performance to ensure sustained impact  
- Conduct a follow-up A/B test focused on improving mobile experience  


## Limitations
- Analysis limited to a single traffic segment (gsearch nonbrand)  
- Results may not generalize across all acquisition channels  
- Mobile performance indicates further optimization opportunities  


## Files Included
- `Maven Fuzzy Factory AB Test Analysis.xlsx` — Full analysis, data model, and dashboard  
- Dashboard preview — Visual summary of results  


## Key Takeaway
This project demonstrates the end-to-end workflow of:
- transforming raw data into a structured model  
- analyzing controlled experiments  
- validating results statistically  
- translating insights into actionable business decisions  
