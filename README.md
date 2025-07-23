#  Zomato Restaurant Reviews EDA & Rating Prediction

This project analyzes restaurant reviews and metadata from Zomato to uncover insights about what influences customer ratings — and builds a simple machine learning model to predict restaurant ratings.

---

##  Project Goals

- Perform **EDA (Exploratory Data Analysis)** on restaurant reviews and metadata.
- Clean & prepare raw data for modeling.
- Engineer new features to improve prediction accuracy.
- Build a simple **Linear Regression model** to predict numeric ratings.
- Visualize model performance and share key insights.

---

##  Datasets Used

- **Zomato Restaurant Reviews:**  
  Contains individual customer reviews — restaurant name, reviewer, text, rating, timestamp, number of pictures, etc.

- **Zomato Restaurant Metadata:**  
  Contains details about each restaurant — name, average cost for two, cuisines offered, timings, and more.

---

##  EDA Highlights

- **Ratings Distribution:** Most reviews are positive, clustered around 4–5 stars.
- **Top Cuisines:** Identifies the 10 most popular cuisines.
- **Cost vs Rating:** Shows a mild trend that higher-priced restaurants often get slightly better ratings.
- **Pictures & Review Length:** Longer reviews and those with pictures may reflect better engagement.

---

##  Feature Engineering

- Converted `Rating` and `Cost` to numeric format.
- Created new features:
  - `Review_Length` → character length of each review.
  - `Has_Pictures` → binary flag for whether pictures are included.
  - Extracted `Main_Cuisine` from multiple cuisines and one-hot encoded it.

---

## Model

- Built a **Linear Regression model** to predict the numeric rating.
- Used features: Cost, Review Length, Has Pictures, Cuisine type.
- Split data into training and test sets.
- Evaluated with RMSE (Root Mean Squared Error) and R².

---

##  Results

- The model predicts restaurant ratings with moderate accuracy.
- Cost and cuisine help but don’t fully explain rating trends.
- More advanced features, like sentiment analysis of review text, could improve performance.

---

##  Insights

- Zomato reviews are generally positively biased.
- Costlier restaurants tend to get slightly better ratings.
- Pictures and detailed reviews indicate more engaged customers.
- Further improvements can include sentiment scoring and advanced models (Random Forest, XGBoost).

---

