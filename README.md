# YouTube_Video_Performance_Predictor_and_Audience_Insights_System
### ✅ `README.md`

```markdown
# 📺 YouTube Analytics and Insights

A Streamlit web application for analyzing, forecasting, and visualizing YouTube channel performance using machine learning, visual dashboards, sentiment analysis, and geographic insights.

---

## 🚀 Features

- 📊 **Predict Video Performance** using XGBoost regression
- 📈 **Visualize Key Metrics** including top videos, correlations, and time series forecasts
- 💬 **Sentiment Analysis** with word clouds and comment filtering
- 🌍 **Geographic Insights** through choropleth and subscriber breakdowns
- 🔗 **Power BI Integration** (for embedded dashboards)
- ⚙️ **Admin Panel** for file upload, model management, and cache clearing

---

## 📂 Folder Structure


YouTube\_Web\_App/
├── app.py                       # Main landing page
├── pages/
│   ├── 1predictions.py
│   ├── 2visuals.py
│   ├── 3sentiment.py
│   ├── 4geo\_insights.py
│   ├── 5powerbi.py
│   └── 6settings.py
├── utils/
│   ├── data\_utils.py
│   └── model\_utils.py
├── data/                        # CSV files go here
│   └── \*.csv
├── xgboost\_views\_model.pkl      # Pre-trained model
├── requirements.txt
└── README.md

---

## 🛠️ Installation

### 🔧 Local Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/YouTube-Web-App.git
   cd YouTube-Web-App
````

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Add your CSV data**

   * Place your YouTube Studio exports into the `/data/` folder:

     * `Processed_Video_Data.csv`
     * `Aggregated_Metrics_By_Country_And_Subscriber_Status.csv`
     * `Daily_Views_Over_Time.csv`
     * `Processed_Comments_Sentiment.csv`

4. **Run the app**

   ```bash
   streamlit run app.py
   ```

---

## 🌐 Streamlit Cloud Deployment

1. Push your code to a **GitHub repo**
2. Go to [streamlit.io/cloud](https://streamlit.io/cloud) and sign in
3. Click **"New app"** and link your GitHub repository
4. Set the main file as `app.py`
5. Streamlit will auto-install from `requirements.txt`

---

## 💡 Data Format Guidelines

Ensure your files match the expected columns:

* `Processed_Video_Data.csv` — must include `views`, `title`, and features used in model
* `Processed_Comments_Sentiment.csv` — must include `clean_comment`, `original_comment`, `sentiment`
* `Aggregated_Metrics_By_Country_And_Subscriber_Status.csv` — must include `country`, `subscribed_status`, and numeric metrics
* `Daily_Views_Over_Time.csv` — must include `date` and `views`

---

## 🧠 Model Info

The app uses a pre-trained **XGBoost regression model** to predict video views based on video metadata.

To retrain or replace the model:

* Go to the ⚙️ **Settings & File Management** page
* Upload a new `.pkl` file or CSV to retrain

---


## 📄 License

MIT License. Free to use, modify, and share.

---

## 👨‍💻 Developed By

KAMMAMPATI SAIVAMSHI
[LinkedIn](https://www.linkedin.com/in/kammampati-saivamshi-/)                                      
[GitHub](https://github.com/kammampatiSaivamshi)



