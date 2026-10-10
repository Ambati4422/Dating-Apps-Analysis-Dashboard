💙 Dating Apps Analysis Dashboard | Power BI

<p align="center">
  <strong>Customer Feedback • Ratings • Sentiment Analysis • Platform Performance</strong>
</p><p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/Excel-Data%20Source-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel"/>
  <img src="https://img.shields.io/badge/DAX-Data%20Modeling-4472C4?style=for-the-badge" alt="DAX"/>
</p>📌 Project Overview

The Dating Apps Analysis Dashboard is an interactive Power BI project designed to analyze dating app reviews, customer sentiment, app ratings, review categories, and platform performance.

The dashboard transforms review data into meaningful insights through KPI cards, interactive slicers, and visualizations. It demonstrates skills in data cleaning, data modeling, DAX calculations, and business intelligence reporting.

🎯 Project Objectives

- Analyze customer sentiment across dating apps.
- Calculate average app ratings and review counts.
- Identify the most common review categories.
- Compare customer feedback across Google Play and Apple App Store.
- Explore review trends and patterns using interactive filters.
- Present insights through a professional dashboard.

🛠️ Tools & Technologies

- Power BI Desktop — Dashboard development and visualization
- Power Query — Data cleaning and transformation
- DAX — Measures and KPI calculations
- Microsoft Excel — Source dataset
- Data Modeling — Calendar table and date relationships

📊 Dashboard Features

1. Key Performance Indicators (KPIs)

- Total Reviews
- Average Rating
- Total Apps
- Positive Sentiment Percentage
- Negative Reviews

2. Customer Sentiment Analysis

Visualizes the distribution of positive, neutral, and negative reviews to understand customer feedback patterns.

3. Review Category Analysis

Analyzes review categories such as:

- App design
- Good matches
- Ease of use
- Safety and verified profiles
- Pricing and payments
- Account bans and support
- Poor match quality
- Bugs and crashes
- Fake profiles and bots

4. Platform Performance

Compares review counts and sentiment across Google Play and Apple App Store.

5. Interactive Filters

The dashboard includes slicers for:

- App Name
- Platform
- Country
- Sentiment
- Year

These filters allow users to explore different segments of the dataset.

🧮 Sample DAX Measures

Total Reviews

Total Reviews =
COUNTROWS('Dating_Apps_1500')

Average Rating

Average Rating =
AVERAGE('Dating_Apps_1500'[Rating])

Total Apps

Total Apps =
DISTINCTCOUNT('Dating_Apps_1500'[App_Name])

Positive Sentiment %

Positive Sentiment % =
DIVIDE(
    CALCULATE(
        [Total Reviews],
        'Dating_Apps_1500'[Sentiment] = "Positive"
    ),
    [Total Reviews],
    0
)

Format the Positive Sentiment % measure as a percentage in Power BI.

Negative Reviews

Negative Reviews =
CALCULATE(
    [Total Reviews],
    'Dating_Apps_1500'[Sentiment] = "Negative"
)

🎨 Dashboard Design

The dashboard uses a professional visual theme:

- Navy Blue ("#142D4E") — Header and titles
- Light Blue-Grey ("#EAF2F8") — Page background
- Blue ("#4472C4") — Primary charts
- Green ("#27856C") — Positive sentiment
- Amber ("#E5A443") — Neutral sentiment
- Red ("#C85B62") — Negative sentiment

The layout combines KPI cards, charts, and slicers to provide a clear and interactive analytical experience.

📁 Project Structure

Dating-Apps-Analysis/
│
├── README.md
├── Dating_Apps_Analysis.pbix
├── Dating_Apps_Dataset.xlsx
└── images/
    └── dashboard-screenshot.png

Update the filenames to match the files you actually upload.

🚀 How to Use the Project

1. Download or clone this repository.
2. Open "Dating_Apps_Analysis.pbix" using Power BI Desktop.
3. If prompted, reconnect the Excel data source.
4. Refresh the dataset if required.
5. Use the slicers to filter apps, platforms, countries, sentiments, and years.
6. Explore the visualizations to analyze review patterns.

📈 Key Insights

The dashboard can help explore:

- Which review categories receive the most feedback.
- How customer sentiment is distributed.
- Differences in review patterns between platforms.
- How average ratings vary across dating apps.
- Which apps and review categories deserve further investigation.

Add verified findings from your final dashboard before publishing specific business conclusions.

⚠️ Data Disclaimer

The dataset used for this project is marked as SIMULATED. It is intended for learning, demonstration, and portfolio purposes. The results should not be interpreted as verified real-world customer feedback or market research.

👨‍💻 Skills Demonstrated

- Data cleaning and transformation
- Exploratory data analysis
- DAX measures and KPI development
- Calendar table creation
- Data modeling and relationships
- Interactive Power BI dashboard design
- Data storytelling and visualization

🔮 Future Improvements

- Add monthly review trend analysis.
- Build a Top 10 Apps by Average Rating visual.
- Add more advanced sentiment comparisons.
- Improve tooltip pages and drill-through functionality.
- Publish an interactive report where appropriate.

📬 Connect

Project: Dating Apps Analysis Dashboard
Technology: Microsoft Power BI

Thank you for visiting this project! ⭐ If you find it useful, feel free to explore the repository and share feedback.
