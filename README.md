# 📱 Mobile Phone Market Analytics Dashboard

> A 4-page Power BI dashboard that benchmarks smartphones across brands, specs, camera resolutions, and multi-currency pricing — helping consumers, analysts, and retailers navigate the global mobile market.

---

## 📌 Problem Statement

The smartphone market is flooded with hundreds of models across dozens of brands, making it difficult to:
- Compare models and brands on specs like RAM, camera, battery, and processor
- Understand pricing across different regions and currencies (INR, USD, AED, PKR, CNY)
- Identify which brands offer the most models and best value for specific specs
- Find the right phone based on budget and feature preferences

This dashboard makes all of that comparison immediate and interactive.

---

## 🖥️ Dashboard Pages

| Page | Description |
|------|-------------|
| **Overview** | Brand landscape — number of models per company, RAM distribution, front/back camera breakdown, processor variety |
| **Camera Resolution Details** | Full spec table with model, front camera, back camera, and company |
| **Price Analysis** | Multi-currency pricing (INR, USD, AED, PKR, CNY) by model and company |
| **Features vs. Price Comparison** | Filterable comparison table by RAM, screen size, battery, weight, processor, and launch price |

---

## 🔍 Key Features

- **Multi-currency pricing** — launch prices shown in INR, USD, AED, PKR, and CNY simultaneously
- **Company + year slicers** — filter all visuals by brand and launch year
- **Camera resolution analysis** — dedicated table showing front & back camera specs per model
- **Features vs. Price** — interactive comparison table with slicers for RAM, price range, and currency
- **Bookmark navigator** — smooth navigation between pages

---

## 🛠️ Tech Stack

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Report design and visual layout |
| **DAX** | Average launch price per currency, model counts, distinct processor count |
| **Power Query (M)** | Multi-currency data normalization, spec parsing |

---

## 📊 Key DAX Measures

```dax
Avg Launch Price (INR) = AVERAGE('Mobiles'[Launched Price (INR)])

Avg Launch Price (USD) = AVERAGE('Mobiles'[Launched Price (USD)])

Distinct Processor Count = DISTINCTCOUNT('Mobiles'[Processor])

Number of Models = COUNTROWS('Mobiles')
```

---

## 📊 Dataset Fields

`Company Name` · `Model Name` · `RAM (GB)` · `Front Camera` · `Back Camera` · `Processor` · `Screen Size` · `Battery Capacity` · `Mobile Weight` · `Launched Year` · `Launched Price (INR/USD/AED/PKR/CNY)`

---

## 💡 Business Impact

- Helps **consumers** find the best phone within their budget across brands and specs
- Enables **retail analysts** to benchmark brand pricing strategies across global markets
- Supports **procurement teams** in telcos/retailers with competitive spec-price intelligence
- Useful for **tech journalists and reviewers** doing structured multi-brand comparisons

---

## 📁 File

| File | Description |
|------|-------------|
| `Mobile_Dataset.pbix` | Power BI report file |

---

## 🚀 How to Use

1. Download `Mobile_Dataset.pbix`
2. Open in **Power BI Desktop**
3. Start on **Overview** to explore the brand landscape
4. Use **Price Analysis** to compare models in your local currency
5. Use **Features vs. Price Comparison** with slicers to find your ideal phone

---

## 👤 Author

**Tejas Bafna** — Data Analyst | Power BI Developer  
📧 tejasbafna311@gmail.com · [LinkedIn](www.linkedin.com/in/tejas-bafna) ·
