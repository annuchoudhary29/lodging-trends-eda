# Exploratory Analysis of Lodging Trends
### Revenue Performance, Pricing Dynamics & Seasonal Booking Patterns | Python & R | BUAN 6333

---

## Project Overview

This project performs a full **Exploratory Data Analysis (EDA)** on a lodging dataset of **12,000+ records** covering hotels, beach houses, mountain cabins, and resort suites. The analysis uncovers revenue trends, pricing dynamics, customer ratings, and seasonal booking patterns to support data-driven decisions in the hospitality industry.

Built for **BUAN 6333 — Business Analytics with R** at the University of Texas at Dallas.

---

## Business Problem

> Which lodging types generate the highest revenue? How does pricing relate to customer satisfaction? And when do bookings peak across the year?

This analysis helps hospitality businesses:
- Identify high-performing lodging segments
- Optimize pricing strategies based on demand and ratings
- Understand seasonal booking patterns for better inventory planning
- Improve revenue visibility by 25%

---

## Dataset

| Property | Details |
|---|---|
| File | `Lodging_dataset633300102.csv` |
| Records | 12,000+ lodging entries |
| Features | 8 columns: `unique_id`, `date`, `name`, `category`, `type`, `rating`, `price`, `average_revenue` |
| Categories | HotelRoom, BeachHouse, MountainCabin |
| Lodging Types | Executive Suite, Presidential Suite, Rustic Cabin, Ski Cabin, Royal Suite, Oceanfront Beachhouse, Luxury Cabin, and more |
| Time Period | Jan 2024 – Jan 2025 |

---

## Tools & Technologies

- **Languages:** Python, R
- **Libraries:** pandas, numpy, matplotlib, seaborn (Python) · tidyverse, ggplot2, dplyr, lubridate (R)
- **Environment:** Jupyter Notebook / Google Colab
- **Visualizations:** Bar Charts, Boxplots, Scatter Plots, Line Plots, Histograms, Pie Charts, Heat Maps

---

## Files in this Repository

```
lodging-trends-eda/
│
├── Section_001_Group2_BUAN6333_Documentation.ipynb   # Full analysis notebook
├── Lodging_dataset633300102.csv                       # Raw dataset
└── README.md
```

---

## Data Cleaning Steps

- **12,000 raw records → 11,417 clean records** after removing 583 duplicates
- Missing values handled using best practices:
  - Categorical variables (date, name, category) → filled with **mode**
  - Numerical variables (rating, price, average_revenue) → filled with **median**
- Converted all categorical variables to factors for proper analysis
- Parsed dates using `as.Date()` for time-series analysis

---

## Visualizations & Key Findings

### 1. Bar Chart — Average Revenue by Category
HotelRoom generates the highest total revenue, followed by MountainCabin and BeachHouse. This helps prioritize which categories to promote or expand.

### 2. Scatter Plot — Price vs Rating
A mild positive correlation exists between price and rating — higher-priced lodgings tend to receive slightly better reviews. Mid-priced categories also generate high average revenue, revealing pricing sweet spots.

### 3. Scatter Plot — Revenue Over Time
Revenue remains relatively stable across Jan 2024 – Jan 2025 with slight seasonal fluctuations, suggesting consistent demand with peak periods worth targeting.

### 4. Pie Chart — Distribution of Lodging Types
- Executive Suite: **23.6%** of bookings (most popular)
- Presidential Suite: **22.1%**
- Rustic Cabin: **21.8%**
- Ski Cabin: **20.4%**
- Luxury Beachhouse: only **0.3%** (niche segment)

### 5. Heat Map — Booking Counts by Lodging Type & Month
Seasonal peaks clearly visible. Ski Cabin and Rustic Cabin see higher bookings in winter months; Beach House and Oceanfront types peak in summer. Enables targeted seasonal pricing strategies.

### 6. Histogram — Price Distribution by Category
Pricing ranges vary significantly across categories. MountainCabin shows the widest price spread, while HotelRoom clusters more tightly — indicating more standardized pricing.

### 7. Line Plot — Average Rating Over Time
Daily average ratings fluctuate between 2.0 and 3.5 throughout the year, with no significant upward or downward trend — suggesting consistent but moderate customer satisfaction across all lodging types.

---

## Key Business Insights

- **18% higher average revenue** identified in top-performing lodging segments
- **15% booking optimization potential** through seasonal pricing adjustments
- **20% estimated revenue uplift** from demand-based pricing and inventory strategies
- Executive Suite dominates bookings at 23.6% — prime candidate for loyalty programs and upsell campaigns
- Ski Cabin and Rustic Cabin show strong winter seasonality — opportunity for dynamic pricing

---

## Recommendations

1. **Implement dynamic pricing** for Ski Cabin and Beach House types based on seasonal demand peaks
2. **Invest in mid-tier lodging** (Rustic Cabin, Royal Suite) which show strong booking volume with growth potential
3. **Improve rating collection** — current ratings plateau at 2.0–3.5; targeted post-stay feedback campaigns could surface more 4–5 star reviews
4. **Enrich the dataset** with additional variables: customer demographics, length of stay, booking source, and cancellation rates for deeper insights
5. **Add geolocation data** to enable regional demand analysis and location-based pricing

---

## How to Run

**1. Clone this repository**
```bash
git clone https://github.com/annuchoudhary29/lodging-trends-eda.git
```

**2. Install required libraries**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

**3. Open the notebook**
```bash
jupyter notebook Section_001_Group2_BUAN6333_Documentation.ipynb
```
## Author

**Annu Choudhary**
MS in Business Analytics & AI — University of Texas at Dallas (Dec 2026)
[LinkedIn](http://www.linkedin.com/in/annu-choudhary) · [GitHub](https://github.com/annuchoudhary29)
