# 🛍️ Customer Segmentation — Indonesian E-Commerce
**Data Mining / Clustering Analysis**

This project performs customer segmentation for an Indonesian e-commerce platform using classical data mining techniques. The analysis identifies distinct customer groups and produces actionable marketing recommendations for each segment.

## Methods Used

| Method | Purpose |
|--------|---------|
| **RFM Analysis** | Score customers on Recency, Frequency, and Monetary value |
| **K-Means Clustering** | Automatic segmentation across multiple behavioral features |
| **Hierarchical Clustering** | Dendrogram-based group structure analysis |
| **PCA** | Dimensionality reduction for 2D visualization |

## Project Structure

```
customer-segmentation/
├── data/
│   └── indonesia_customers.csv         # 100 customers from Indonesian cities
└── notebooks/
    └── customer_segmentation.ipynb     # Full analysis + visualizations
```

## Dataset — `indonesia_customers.csv`

100 customers from major Indonesian cities with the following features:

| Column | Description |
|--------|-------------|
| `city`, `province`, `island` | Customer location |
| `age` | Customer age |
| `gender` | Male / Female |
| `monthly_income_million_idr` | Monthly income (Million IDR) |
| `monthly_spending_million_idr` | Monthly e-commerce spending (Million IDR) |
| `shopping_frequency_per_month` | Number of purchases per month |
| `favorite_product_category` | Fashion, Electronics, Food & Grocery, etc. |
| `shopping_channel` | Online / Offline |
| `loyalty_score` | Platform loyalty score (0–100) |
| `recency_days` | Days since last purchase |

## Getting Started

```bash
jupyter notebook notebooks/customer_segmentation.ipynb
```

## Customer Segments Discovered

| Segment | Profile | Recommended Strategy |
|---------|---------|---------------------|
| 💎 **Premium Spender** | High income & spending, loyal | VIP program, exclusive products |
| 👗 **Young Fashionista** | Young, high frequency, fashion-focused | Flash sales, influencer marketing |
| 🎯 **Deal Hunter** | Moderate spending, discount-driven | Vouchers, bundles, referral rewards |
| 😴 **Passive Buyer** | Low frequency, high recency | Re-engagement emails, win-back offers |

## Output Charts

- 📊 6-panel EDA dashboard (age, income, channel, category, city, loyalty)
- 🥧 RFM segment distribution pie chart
- 🔵 K-Means scatter: income vs spending (color-coded by segment)
- 🌲 Hierarchical clustering dendrogram (30-customer sample)
- 📐 PCA 2D projection with feature loading analysis
- 📋 Final segment profile table + marketing strategy summary

## Requirements

```
pandas
numpy
matplotlib
scikit-learn
scipy
```

## Key Insights

- **Jakarta** dominates the Premium Spender segment (highest income concentration)
- **Bandung & Yogyakarta** skew Young Fashionista (student city demographics)
- **Online shoppers** have 3× higher purchase frequency than offline shoppers
- **Bali** customers uniquely favor Travel & Lifestyle (tourism-driven economy)

---
*Dataset simulated based on Indonesian consumer behavior characteristics, 2023–2024*
