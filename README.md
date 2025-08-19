# ✈️ Flight Delay Analysis & Prediction

A Machine Learning project analyzing flight delay patterns in the US and building models to predict whether a flight will be delayed, and by how many minutes.

---

## 🧾 Dataset

* **Source**: [US Department of Transportation (BTS)](https://www.transtats.bts.gov/DL_SelectFields.aspx?gnoyr_VQ=FGJ&QO_fu146_anzr=b0-gvzr)
* **Time Period**: January to April 2025
* **Original Raw Data Files**: Due to large file sizes, the raw `.csv` files are not uploaded here.
* **Access Raw Files**:
  You can download all four raw files (Jan–Apr 2025) from my Google Drive here:
  👉 [Download from Google Drive](https://drive.google.com/drive/folders/1Iq9rTBLEFpqbo_CkC5MfbC6_7obv2g5M?usp=sharing)

---

## 🔧 Tech Stack

* **Platform**: Google Colab
* **Languages**: Python (Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn)
* **Tools**: SQL (via `pandasql`), GitHub for version control
* **Planned Extension**: Streamlit app for interactive demo, Deep Learning for multivariate prediction (future scope)

---

## 📊 Exploratory Data Analysis (EDA)

### 1. Flight Volume Distribution

* **Observation**: The dataset contains millions of flights over 4 months.
* **Insight**: Daily flight counts fluctuate, with Fridays and Sundays seeing the highest traffic.

### 2. Delays vs. On-time Flights

* **Observation**: The majority of flights are on-time.
* **Insight**: However, delays form a significant minority (\~20–25%), enough to cause real-world impact.

### 3. Carrier-wise Analysis

* **Observation**: Airlines differ in delay rates. Some carriers show higher average delay times.
* **Insight**: Operational efficiency and traffic management play a major role.

### 4. Airport Performance

* **Observation**: Major hubs (e.g., ATL, ORD, DFW) handle the largest number of flights.
* **Insight**: Busy airports naturally face more delays due to congestion and air traffic.

### 5. Delay Reasons Breakdown

* **Observation**: Delays are categorized into **Weather, NAS (Air Traffic), Security, Carrier, and Late Aircraft**.
* **Insight**: Carrier-related and late aircraft delays are the most frequent, while security delays are rare.

### 6. Heatmap (Correlation)

* **Observation**: Strong correlations between departure delay and arrival delay.
* **Insight**: If a flight departs late, it is very likely to arrive late too.

### 7. Distribution of Delay Duration

* **Observation**: Most delays are short (<30 min), but there are outliers with 4–6 hours.
* **Insight**: Outliers can heavily affect averages; hence median is a better measure.

### 8. Temporal Trends (Monthly/Weekly/Hourly)

* **Observation**: Delays spike during **evening hours** and are lower in early mornings.
* **Insight**: Congestion builds up later in the day, leading to compounding delays.

---

## 🚧 Work in Progress

This is part of a multi-day ML project with tracked progress and daily updates in GitHub.
Future enhancements include deep learning modeling and a Streamlit deployment.
