# Yelp Sentiment Analysis vs. Star Ratings

## 📌 Project Overview
The goal of this project is to **capture the sentiment** of Yelp reviews and compare them to the **star rating system** to analyze discrepancies.

## 🔍 Data Collection
To collect the data, I used **SerpApi**:
1. **First API Call** – Retrieves a list of **Place IDs** for coffee shops in **New York City**.
2. **Second API Call** – Loops through each **Place ID** to extract **customer reviews**.
3. The reviews are stored in a **dictionary** and then **normalized** into a `pandas.DataFrame`.

## 🛠 Data Preprocessing
- Converted JSON output into a **structured DataFrame**.
- Changed data types to the **appropriate format** for analysis.

## 📊 Sentiment Analysis
- Imported `nltk` and downloaded the **VADER lexicon**.
- Applied **VADER sentiment analysis** to extract:
  - `Negative`
  - `Neutral`
  - `Positive`
  - `Compound` (main metric for comparison)
- Created **visualizations** to highlight sentiment **misalignment** with star ratings.

## 🔎 Key Takeaways
- Sentiment **does not always correlate** with the **star rating**.
- **VADER lexicon** works via **tokenization** and does not understand **contextual relationships** between words.

## 🚀 Future Improvements
1. **Upgrade Sentiment Model**  
   - Utilize **deep learning models** like **BERT** or **RoBERTa** for **context-aware** sentiment analysis.

2. **Modular Code Structure**  
   - Separate **API calls** and **data cleaning**  from **analysis** into different scripts for **better organization**.

3. **Integrate Named Entity Recognition (NER)**  
   - Use **spaCy** to identify **specific entities**:
     - **Products** (e.g., "coffee", "latte", "espresso")
     - **Employees** (e.g., "barista", "manager")
     - **Locations** (e.g., "Brooklyn", "Manhattan")
   - This would provide **more actionable insights** into **why** a review is **positive or negative**.

---

## ⚡ Next Steps
- **Refine analysis** using **advanced NLP models**.
- **Enhance data visualization** with **interactive dashboards**.
- **Optimize review extraction** for **larger datasets**.

This project lays the foundation for **data-driven business insights** beyond simple sentiment analysis. 🚀  
