# Data Analysis Projects

End-to-end exploratory data analysis and machine learning on 10 real-world Indian and global datasets — built with Python, Pandas, Plotly, and Scikit-learn.

---

## Projects

### 1. Netflix Content Analysis
Analyzed Netflix's full content library to uncover what gets made, where, and for whom.
- 69.7% of Netflix content is Movies vs 30.3% TV Shows
- The US dominates production by a wide margin; India ranks 2nd among non-Western countries
- Content addition surged dramatically from 2015 to 2019, then dropped — likely COVID impact
- Drama and International Movies are the top two genres by a large margin
- Most movies cluster between 90–120 minutes; a sharp peak at ~100 min
- Built ML classifiers (Logistic Regression, Decision Tree, Random Forest, SVM) to predict content type — **SVM achieved 77% accuracy**; genre was the strongest predictive feature

---

### 2. Zomato Restaurant Analysis
Explored Bangalore's restaurant ecosystem across price, location, cuisine, and ratings.
- BTM Layout has the highest restaurant density (5,124 restaurants); Koramangala leads in total customer votes (2M+)
- Restaurants offering online ordering tend to have higher and more consistent ratings — confirmed via box plot
- Higher cost does not reliably predict a better rating; the scatter shows weak correlation
- Delivery and Dine-out dominate restaurant types; niche categories like Desserts and Cafes are underrepresented
- Trained regression models (Linear Regression, Decision Tree, Random Forest) to predict ratings — Decision Tree achieved the best MAE of **0.05**

---

### 3. Swiggy Restaurant Analysis
Focused on pricing, delivery performance, and cuisine trends across Indian cities.
- Kolkata has the most restaurants, followed by Mumbai and Chennai
- Most restaurant prices cluster under ₹500; a long tail extends to ₹2,500+
- Delivery time is the **most important feature** influencing ratings — more than price or city
- North Indian and Chinese cuisines dominate at 17.9% and 13.3% respectively
- Random Forest predicted ratings with MAE of 0.55 using price, city, and delivery time as features

---

### 4. COVID-19 India Analysis
Merged two datasets (confirmed cases + statewise testing data) to track the pandemic across India.
- Maharashtra had the highest confirmed cases (~6M); followed by Kerala and Karnataka
- Clear two-wave pattern visible in daily new cases: first wave (mid-2020), second wave (April–May 2021)
- 7-day rolling positivity rate spiked sharply in early 2020 then stabilised — important for understanding data quality
- Punjab had an outlier high fatality rate relative to its case count
- States like Kerala and Maharashtra showed high recovery rates despite high case counts

---

### 5. YouTube Trending Video Analysis
Compared trending video patterns between India and the US.
- Entertainment dominates trending in the US; Music and Entertainment lead in India
- Most Indian videos trend within **0–4 days** of being published — very fast virality window
- Friday is the best day to publish for maximum trending chances in India
- Likes and views are highly correlated (0.83) — comments correlate more with likes (0.77) than views (0.57)
- Science & Technology has the highest average like-to-view ratio in India (~8 likes per 100 views)
- Capitalized titles get marginally more views (52% vs 48%) — minimal but measurable

---

### 6. Amazon Prime Video Analysis
Explored content trends on Amazon Prime from the 1920s to 2020.
- 80.8% of Prime content is Movies; only 19.2% TV Shows — more movie-heavy than Netflix
- Content release exploded after 2000, with a sharp vertical climb post-2015
- Drama dominates genres, followed by Comedy and Action
- Most movies run between 80–120 minutes, similar to Netflix's distribution
- Rating system is far more fragmented than Netflix — over 15 distinct rating categories

---

### 7. Spotify Music Trends Analysis
Analyzed audio features and streaming data to understand what makes a hit song.
- Top streamed song: **Blinding Lights** (~3.6B streams); Shape of You close behind
- Bad Bunny leads in artist hit count, followed by Taylor Swift and The Weeknd
- High energy and high valence (happier) songs tend to be more danceable — positive correlation
- Acousticness is **negatively correlated** with energy (-0.58) — louder songs are less acoustic
- May has the highest number of hit releases; July the lowest
- Top 50 songs are noticeably more danceable and energetic than the overall dataset average

---

### 8. IMDB Top 1000 Movies Analysis
Investigated what separates critically acclaimed films from the rest.
- Critic scores (Metascore) and user ratings (IMDB Rating) are positively correlated but with significant spread — critics and audiences often disagree
- Box office gross surged from the 1980s onward, peaking in the 2000s
- Adventure is the most prevalent genre (28.5%), followed by Action and Thriller
- Films rated 90–150 minutes get the best IMDB ratings — very long and very short films score lower
- Frank Darabont has the highest average director rating, followed by Lana Wachowski and Irvin Kershner
- U-rated films are most common in the Top 1000, suggesting family-friendly content ages better

---

### 9. Flipkart E-Commerce Analysis
Analyzed product pricing, categories, discounts, and ratings across Flipkart's catalog.
- Clothing is by far the largest category; Jewellery and Footwear follow
- Automotive products have the highest average discount (~50%); most categories average 25–45%
- Retail price and discounted price are tightly correlated — discounts are proportional, not random
- Linear Regression struggled to predict price (R² = 0.04); Decision Tree improved significantly
- Product ratings cluster heavily at 3–4 stars; very few products rated below 2

---

### 10. Blinkit Quick Commerce Analysis
Multi-table analysis across orders, products, delivery performance, and marketing data.
- Dairy & Breakfast and Snacks & Munchies are the top revenue-contributing categories
- Peak sales hours are irregular throughout the day — no single dominant hour, suggesting round-the-clock demand
- Most deliveries cluster near on-time; a secondary spike around 0.5T delay suggests a recurring late-delivery pattern
- 34.2% of customers gave a 5-star rating; 28% gave 4 stars — majority positive
- Marketing spend has near-zero correlation with revenue generated (R² = -0.008) — spend alone doesn't drive sales
- K-Means clustering split campaigns into 3 distinct segments by spend and revenue

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Plotly Express | Interactive visualizations (bar, scatter, pie, treemap, sunburst, choropleth, heatmap) |
| Scikit-learn | ML models: Logistic Regression, Decision Tree, Random Forest, SVM, Linear Regression, K-Means |
| JupyterLab | Development environment |

---

## How to Run

```bash
# Clone the repo
git clone https://github.com/abhimanyuchettiar/data-analysis-projects.git
cd data-analysis-projects

# Install dependencies
pip install pandas numpy plotly scikit-learn jupyterlab

# Launch JupyterLab
jupyter lab
```

Each notebook is self-contained. Download the corresponding dataset from [Kaggle](https://www.kaggle.com) and update the `pd.read_csv()` path at the top of the notebook.

---

## Author

**Abhimanyu Chettiar**
B.Tech CSE — Apeejay Stya University

[LinkedIn](https://linkedin.com/in/abhimanyu-chettiar) • [GitHub](https://github.com/abhimanyuchettiar)
