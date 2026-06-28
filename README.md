# 💰 Google Play Store Revenue & Install Performance Analysis

> A Data Analytics project that analyzes Google Play Store applications based on installs, revenue generation, app size, Android version compatibility, and pricing models to compare Free and Paid apps across top-performing categories.

---

# 📑 Table of Contents

- <a href="#project-title">Project Title</a>
- <a href="#brief-summary">Brief One Line Summary</a>
- <a href="#overview">Overview</a>
- <a href="#problem-statement">Problem Statement</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools-and-technologies">Tools & Technologies</a>
- <a href="#methods">Methods</a>
- <a href="#key-insights">Key Insights</a>
- <a href="#dashboard-output">Dashboard / Output</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#how-to-run-this-project">How to Run this Project?</a>
- <a href="#results-conclusion">Results & Conclusion</a>
- <a href="#future-work">Future Work</a>
- <a href="#author-contact">Author & Contact</a>

---

<h2 id="project-title">📌 Project Title</h2>

# Google Play Store Revenue & Install Performance Analysis

---

<h2 id="brief-summary">📝 Brief One Line Summary</h2>

A Python-based analytics dashboard that evaluates revenue generation and installation performance of Free and Paid Google Play Store applications across top-performing categories.

---

<h2 id="overview">📖 Overview</h2>

The Google Play Store contains millions of applications operating under different business models. Understanding how Free and Paid applications perform in terms of installations and revenue can provide valuable business insights.

This project cleans and processes Play Store data, calculates estimated revenue, applies business-driven filters, identifies top-performing categories, and visualizes average installs and revenue metrics for Free and Paid applications.

The analysis helps uncover category-level monetization trends and user adoption patterns.

---

<h2 id="problem-statement">⚠️ Problem Statement</h2>

Developers and businesses often struggle to understand:

- Which app categories generate the most revenue.
- Whether Free or Paid apps perform better.
- How app characteristics influence installs and revenue.
- Which categories provide the best monetization opportunities.

This project aims to:

- Analyze revenue generation across app categories.
- Compare Free and Paid applications.
- Identify top-performing categories.
- Evaluate install trends.
- Support data-driven business decisions.

---

<h2 id="dataset">📂 Dataset</h2>

The project uses Google Play Store application data.

### Dataset Features

- App Name
- Category
- Installs
- Price
- Revenue (Calculated)
- Android Version
- App Size
- Content Rating
- Type (Free / Paid)

### Revenue Calculation

```text
Revenue = Price × Installs
```

---

<h2 id="tools-and-technologies">🛠️ Tools & Technologies</h2>

## Programming Language

- Python

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- PyTZ
- Datetime

## Development Environment

- Jupyter Notebook
- VS Code

---

<h2 id="methods">⚙️ Methods</h2>

## 1. Data Cleaning

Performed preprocessing on:

- Installs column
- Price column
- App Size column
- Android Version column
- Duplicate records

### Installs Cleaning

```text
10,000+ → 10000
1,000,000+ → 1000000
```

### Price Cleaning

```text
$4.99 → 4.99
```

---

## 2. Feature Engineering

### Revenue Generation

Created a new feature:

```text
Revenue = Price × Installs
```

### App Length

Calculated:

```text
Length of App Name
```

### Android Version Extraction

Extracted numeric Android version values from text.

---

## 3. Business Rule Filtering

Applications were filtered using:

### Install Threshold

```text
Installs ≥ 10,000
```

### Revenue Threshold

```text
Revenue ≥ 10,000
```

### Android Compatibility

```text
Android Version > 4.0
```

### App Size Filter

```text
Size > 15 MB
```

### Content Rating Filter

```text
Content Rating = Everyone
```

### App Name Length

```text
App Name Length ≤ 30 Characters
```

---

## 4. Category Selection

The top 3 categories were selected based on frequency after filtering.

---

## 5. Aggregation

Calculated:

### Average Installs

Grouped by:

```text
Category + Type
```

### Average Revenue

Grouped by:

```text
Category + Type
```

---

## 6. Visualization

Generated comparative visualizations showing:

- Average Installs
- Average Revenue
- Free vs Paid App Performance
- Category-wise Comparison

---

<h2 id="key-insights">📊 Key Insights</h2>

- Paid apps generate significantly higher revenue despite fewer installs.
- Free apps generally achieve larger user reach.
- Revenue distribution varies across categories.
- Android compatibility and app size influence app performance.
- Top-performing categories dominate both installs and revenue generation.

---

<h2 id="dashboard-output">📈 Dashboard / Output</h2>

## Workflow

```text
Google Play Store Dataset
          ↓
Data Cleaning
          ↓
Feature Engineering
          ↓
Revenue Calculation
          ↓
Business Rule Filtering
          ↓
Top Category Selection
          ↓
Aggregation
          ↓
Visualization
```

---

## 📊 Visualizations Generated

### Average Installs Comparison

Displays:

- Category-wise Average Installs
- Free vs Paid Apps

### Average Revenue Comparison

Displays:

- Category-wise Revenue
- Monetization Performance
- Business Model Comparison

---

## Example Analysis

| Category | Type | Avg Installs | Avg Revenue |
|----------|------|-------------|-------------|
| Category A | Free | High | Low |
| Category A | Paid | Moderate | High |
| Category B | Free | High | Low |
| Category B | Paid | Moderate | High |

---

<h2 id="project-structure">📁 Project Structure</h2>

```bash
Google_Play_Store_Revenue_Analysis/

│
├── task6.ipynb
├── google_play_store_dataset.csv
├── README.md
└── outputs/
```

---

<h2 id="how-to-run-this-project">🚀 How to Run this Project?</h2>

## Clone Repository

```bash
git clone https://github.com/yashrajmohanty03-ai/google-play-store-revenue-analysis.git

cd google-play-store-revenue-analysis
```

## Install Dependencies

```bash
pip install pandas numpy matplotlib pytz
```

## Run Notebook

```bash
jupyter notebook task6.ipynb
```

## Execute All Cells

Run all notebook cells sequentially to:

- Load dataset
- Clean app data
- Calculate revenue
- Apply business filters
- Identify top categories
- Generate comparative visualizations

---

<h2 id="results-conclusion">📈 Results & Conclusion</h2>

## Results

The project successfully:

- Cleaned and transformed Play Store data
- Generated revenue-based metrics
- Applied advanced business filters
- Identified top-performing categories
- Compared Free and Paid applications
- Visualized installs and revenue trends

---
## Output
![image alt](https://github.com/yashrajmohanty03-ai/Ev6/blob/4e7fd6f671151c51388471dcc830724265e4c376/op6.png)

## Conclusion

This project demonstrates how data analytics can be used to evaluate monetization strategies within the Google Play Store ecosystem. By comparing Free and Paid applications across top categories, the analysis reveals important patterns in user adoption and revenue generation, helping developers and businesses make informed decisions.

---

<h2 id="future-work">🔮 Future Work</h2>

Future enhancements include:

- Interactive Plotly dashboards
- Streamlit deployment
- Revenue forecasting models
- Machine Learning-based success prediction
- Sentiment analysis integration
- Power BI dashboards
- Real-time Play Store data integration

---

<h2 id="author-contact">👨‍💻 Author & Contact</h2>

## Yashraj Mohanty

### Areas of Interest

- Data Analytics
- Data Visualization
- Business Intelligence
- Machine Learning

### Contact

- GitHub: https://github.com/yashrajmohanty03-ai
- LinkedIn: https:// linkedin.com/in/yashraj-mohanty
- Email: yashrajmohanty3@gmail.com
---

<p align="center">
⭐ If you found this project useful, consider giving it a star on GitHub!
</p>
