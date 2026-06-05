# ROI Lens: Multi-Touch Marketing Attribution & Budget Optimization

## Overview

ROI Lens is a marketing analytics project focused on overcoming the limitations of traditional **Last-Click Attribution** models. The project reconstructs customer journeys, analyzes multi-channel interactions, and applies a **Markov-based Multi-Touch Attribution Framework** to identify the true contribution of marketing channels across the customer conversion funnel.

The objective is to enable data-driven marketing decisions and optimize budget allocation for improved ROI.

---

## Business Problem

Many organizations rely on **Last-Click Attribution**, where 100% of conversion credit is assigned to the final touchpoint before purchase.

This approach:

- Undervalues awareness-stage channels such as YouTube, Instagram, and Influencer Blogs
- Overcredits conversion-stage channels such as Google Search
- Produces misleading ROI measurements
- Leads to inefficient marketing budget allocation

ROI Lens addresses these challenges through customer journey analytics and multi-touch attribution.

---

## Dataset Overview

The analysis combines three datasets:

### touchpoints.csv

Customer interaction history across marketing channels.

| Field | Description |
|---------|-------------|
| User_ID | Unique customer identifier |
| Timestamp | Interaction timestamp |
| Campaign_ID | Campaign identifier |
| Channel | Marketing channel |
| Event_Type | Impression, Click, Add-to-Cart, Purchase |

---

### user_profiles.csv

Customer demographic and behavioral information.

| Field | Description |
|---------|-------------|
| User_ID | Unique customer identifier |
| Segment | Customer persona |
| Trend_Affinity | Customer preference category |
| Geography | Geographic tier |

---

### campaign_spend.csv

Campaign-level marketing spend information.

| Field | Description |
|---------|-------------|
| Campaign_ID | Campaign identifier |
| Brand_ID | Brand identifier |
| Channel | Marketing channel |
| Pricing_Model | CPC / CPM |
| Cost_Rate_INR | Cost rate |
| Total_Budget_Allocated | Campaign budget |

---

## Dataset Statistics

| Metric | Value |
|----------|----------|
| Customer Touchpoints | 566,510 |
| Unique Users | 100,000 |
| Marketing Channels | 5 |
| Purchase Journeys | 5,498 |

---

## Project Workflow

### 1. Data Preparation

- Missing value validation
- Duplicate record checks
- Timestamp standardization
- Journey sorting by user and time

### 2. Customer Journey Analysis

- Purchase journey extraction
- Customer path reconstruction
- Touchpoint analysis
- Common journey identification

### 3. Channel Performance Analysis

- Purchase Rate Analysis
- Cost Per Acquisition (CPA)
- Budget Efficiency Evaluation

### 4. Multi-Touch Attribution

- Transition Matrix Construction
- Transition Probability Analysis
- Markov-based Attribution Framework
- Channel Contribution Assessment

### 5. Budget Optimization

- Attribution-driven channel evaluation
- Marketing spend analysis
- Budget reallocation recommendations

---

## Key Findings

### Customer Journey Insights

- Customers required approximately **5 touchpoints** before purchase
- Multi-channel interactions were common across successful journeys
- Google Search frequently appeared near the conversion stage
- Awareness channels played a significant role in assisted conversions

---

### Attribution Results

| Channel | Last Click Attribution | Multi-Touch Attribution |
|----------|----------:|----------:|
| Google Search | 48% | 72% |
| Influencer Blog | 9% | 60% |
| Instagram | 16% | 52% |
| Marketplace | 19% | 51% |
| YouTube | 8% | 49% |

---

### Key Business Insight

> The problem was not over-crediting Google Search — it was under-crediting the channels that influenced customers before reaching Google.

---

## Budget Reallocation Recommendations

| Channel | Recommendation | Business Rationale |
|----------|----------|----------|
| Google Search | Increase | Strongest conversion performance |
| Influencer Blog | Slight Increase | Hidden assisted-conversion contributor |
| Instagram | Maintain | Strong awareness and consideration role |
| Marketplace | Slight Reduce | Moderate efficiency |
| YouTube | Reduce & Optimize | High spend with weak direct ROI |

### Illustrative ₹10 Crore Reallocation Strategy

| Channel | Allocation Change |
|----------|----------:|
| Google Search | +₹3 Crore |
| Influencer Blog | +₹2 Crore |
| Instagram | Maintain |
| Marketplace | -₹2 Crore |
| YouTube | -₹3 Crore |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Repository Structure

```text
roi-lens-marketing-attribution/
│
├── data/
│   ├── touchpoints.csv
│   ├── user_profiles.csv
│   └── campaign_spend.csv
│
├── ROI_Lens_Multi_Touch_Attribution_Analysis.ipynb
│
├── README.md
│
└── requirements.txt
```

---

## Results

ROI Lens demonstrates how customer journey analytics and multi-touch attribution provide a more accurate view of marketing performance than traditional last-click attribution.

The framework enables organizations to:

- Improve attribution accuracy
- Optimize marketing spend
- Recognize assisted-conversion channels
- Make more data-driven budget decisions

---

## Author

**Priyanshi Maheshwari**

Marketing Analytics | Data Analytics | Business Intelligence
