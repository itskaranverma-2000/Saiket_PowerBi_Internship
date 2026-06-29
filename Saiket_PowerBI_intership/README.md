# 📊 Telco Customer Churn — Power BI Dashboard

A three-part Power BI project built on the **Telco Customer Churn Dataset**, covering the full BI workflow from raw data connection through transformation to an interactive dashboard.

---

## 🗂️ Project Structure

| File | Task | Description |
|------|------|-------------|
| `Task1_DataConnection.pbix` | Data Connection | Import and connect to the Telco Customer Churn Dataset |
| `Task2_DataTransformation.pbix` | Data Transformation | Clean, shape, and enrich data using Power Query |
| `Task3_Dashboard.pbix` | Dashboard | Build an interactive report with KPIs and visual analytics |

---

## 📋 Dataset

**Source:** Telco Customer Churn Dataset (`Telco_Customer_Churn_Dataset`)

### Key Fields

| Field | Description |
|-------|-------------|
| `customerID` | Unique customer identifier |
| `gender` | Customer gender (Male / Female) |
| `Partner` | Whether the customer has a partner (Yes / No) |
| `Dependents` | Whether the customer has dependents (Yes / No) |
| `tenure` | Number of months the customer has been with the company |
| `InternetService` | Type of internet service (DSL / Fiber optic / No) |
| `Contract` | Contract type (Month-to-month / One year / Two year) |
| `PaymentMethod` | Payment method used by the customer |
| `Churn` | Whether the customer churned (Yes / No) |

### Calculated Measure

| Measure | Description |
|---------|-------------|
| `Churn Rate` | Percentage of customers who churned |

---

## 🖥️ Dashboard Overview (Task 3)

The final report is a single-page interactive dashboard containing:

### KPI Card
- **Churn Rate** — headline metric displayed prominently

### Pie Charts
- Customer distribution by **Gender**
- Customer distribution by **Dependents**
- Customer distribution by **Partner**

### Bar Charts
- Customer count by **Contract Type**
- Customer count by **Internet Service**
- Customer count by **Payment Method**

### Column Chart
- Customer distribution by **Tenure (binned)** — reveals how churn risk varies with customer lifetime

---

## 🎨 Theme

Custom dark theme — **Superstore Dashboard by Remi Rouquette**

| Property | Value |
|----------|-------|
| Background | `#0539BC` (deep blue) |
| Visual backgrounds | `#12309C` |
| Font | Segoe UI |
| Accent / Good | `#1D9E75` (green) |
| Warning / Neutral | `#EF9F27` (amber) |
| Bad / Alert | `#E24B4A` (red) |

---

## 🚀 Getting Started

### Prerequisites

- [Microsoft Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) (version **2.155.385.0** or later, June 2026 release)
- The Telco Customer Churn Dataset (CSV or Excel)

### Steps

1. **Clone this repository**
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```

2. **Open in sequence**
   - Start with `Task1_DataConnection.pbix` to understand the data source setup
   - Move to `Task2_DataTransformation.pbix` to review Power Query transformations
   - Open `Task3_Dashboard.pbix` to explore the final dashboard

3. **Refresh the data source**
   - Go to **Home → Transform Data → Data Source Settings**
   - Update the file path to point to your local copy of the dataset
   - Click **Refresh** to reload the data

---

## 🔧 Task Breakdown

### Task 1 — Data Connection
- Connect Power BI to the Telco Customer Churn Dataset
- Enable automatic type detection and relationship import
- Validate data loads correctly into the data model

### Task 2 — Data Transformation
- Apply Power Query transformations to clean and prepare the data
- Create binned tenure groups (`tenure (bins)`) for bucketed analysis
- Ensure data types and column names are consistent

### Task 3 — Dashboard
- Design a KPI card displaying overall **Churn Rate**
- Build demographic breakdowns using pie charts (gender, dependents, partner)
- Create service and contract analysis using bar charts
- Add tenure distribution via a clustered column chart
- Apply the custom dark blue theme for a polished, presentation-ready look

---

## 📁 Repository Structure

```
.
├── Task1_DataConnection.pbix
├── Task2_DataTransformation.pbix
├── Task3_Dashboard.pbix
└── README.md
```

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop** 2.155.385.0 (2026.06)
- **Power Query (M language)** — data transformation
- **DAX** — calculated measure (`Churn Rate`)
- Dataset created from **Power BI Cloud** environment

---

## 👤 Author

**Remi Rouquette**

---

## 📄 License

This project is for educational and portfolio purposes. The Telco Customer Churn Dataset is publicly available and widely used for churn analysis demonstrations.
