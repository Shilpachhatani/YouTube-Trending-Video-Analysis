
# 📺 YouTube Trending Video Analysis

## 📌 Project Overview & Task Objective

The `Youtube_Trending_Analysis_Main.ipynb` notebook focuses on analyzing trending YouTube videos to understand patterns behind what makes content popular. The objective is to perform data cleaning, feature engineering, and exploratory analysis to uncover insights related to video trends, engagement, and content characteristics.

---

## 📂 Dataset Information

The dataset contains trending video data from YouTube including:
- Video metadata: title, tags, description, channel, category
- Engagement metrics: views, likes, dislikes, comments
- Dates: published and trending dates

**Key Cleaning Tasks:**
- Handled missing values (`description`)
- Removed duplicates
- Cleaned and transformed date/time fields
- Processed text fields (tags, description)

---

## ✨ Features

- Cleaned text, dates, and numerical fields
- Created new features:
  - Time-based: `publish_hour`, `publish_day_of_week`, `days_to_trend`, etc.
  - Engagement: likes/dislikes/comments per view
  - Textual: `tag_count`, `title_length`, `description_length`
- Explored content trends, engagement patterns, and timing insights

---

## 🛠️ Installation

Install required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 🚀 Approach

- **Library Import**: Used pandas, numpy, matplotlib, seaborn
- **Data Cleaning**:
  - Removed nulls and duplicates
  - Converted date columns and removed timezones
  - Cleaned text (tags and descriptions)
- **Feature Engineering**:
  - Time-based: publish hour, weekday, month, year
  - Engagement metrics: per-view ratios and scores
  - Text stats: tag count, title and description length
- **Analysis Ready**: Dataset is fully preprocessed and feature-rich for visualization or modeling

---

## 🧰 Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

---

## 📊 Visualizations
### Distribution of Views
![image](https://github.com/user-attachments/assets/810f4286-f806-4f3b-86b6-cfc7def6c98a)

**Insights:**
This graph shows that 
- most YouTube videos have a relatively low number of views, while a small number of videos gain very high view counts.
- The distribution is heavily right-skewed.
- Most videos struggle to get views, so creators must focus on optimizing content for visibility (thumbnails, titles, SEO) to stand out in the crowded space.

### Distribution of Likes
![image](https://github.com/user-attachments/assets/287da5b8-2cf4-49ed-a760-e0e09afdefa9)

**Insight:**
The Graph shows that
- most videos receive a modest number of likes, with only a few getting large like counts.
- This follows a skewed distribution.
- Engagement through likes is not evenly spread. Encouraging viewers to like videos can improve visibility and algorithm ranking.

### Distribution of Dislikes
![image](https://github.com/user-attachments/assets/e8130a0d-5c12-4235-bc67-f473390430cf)

**Insights:**
The Graph shows that
- Dislikes are much fewer overall compared to likes and views.
- Most videos receive very few dislikes.
- While dislikes are relatively rare, they still indicate audience dissatisfaction.
- Keeping audience satisfaction high reduces the chances of negative feedback.

### Distribution of Comment Count 
![image](https://github.com/user-attachments/assets/7aaafcbe-e07e-4b2e-b586-a4614d0b2b87)

**Insights:**
The Graph shows that
- Most videos receive very few comments, while a few get a lot.
- Comment activity is highly skewed like other engagement metrics.
- Encouraging viewers to comment can boost engagement signals. Interactive videos or questions in content help increase comment counts.

### Distribution of Days to Trend
![image](https://github.com/user-attachments/assets/7cdcee2c-0394-4c67-a282-18cb512f08a3)

**Insights:**
The Graph shows that:
- Most videos that end up trending do so within just a few days of being uploaded, while very few trend later.
- The first few days after upload are critical for gaining traction.
- Creators should focus their promotion and viewer engagement efforts right after publishing a video.

### Top 15 Most Common Video Categories in Trending Videos
![image](https://github.com/user-attachments/assets/b7a3ad29-ee09-4f16-9265-d8b627123b3e)

**Insights:**
The Above Graph Shows that: 
- `Entertainment` dominates with the highest number of trending videos, followed by Music and Howto & Style.
- Other popular categories include Comedy, People & Blogs, and News & Politics, while categories like Autos & Vehicles and Shows appear much less frequently in the trending list.
- This indicates that entertainment-based and music content are more likely to go viral or trend on YouTube.
- For creators aiming to reach trending status, producing content in these popular categories might increase their chances, especially if combined with quality, engagement, and timing.

### Likes vs. Views Scatter Plot (with Category and Comment Count)
![image](https://github.com/user-attachments/assets/28bb0c19-a93f-48b7-9c68-8eebb42cd398)

**Insights:**
The Graph shows that:
- Strong positive correlation between views and likes.
- Larger bubbles (more comments) appear in high-view/like areas.
- Categories like Entertainment & Music lead in engagement.

### Correlation Heatmap of Numerical Features
![image](https://github.com/user-attachments/assets/466307b5-37db-4670-bb33-a12aea527325)

**Insights:**
The Graph shows that:
- views, likes, dislikes, comment_count are highly correlated with each other (e.g., likes vs. views = 0.85).
- engagement_score strongly correlates with likes_per_view (0.97), indicating a solid metric for evaluating video performance.
- days_to_trend has weak or negative correlation with most metrics, suggesting that virality is unpredictable time-wise.

### Number of Trending Videos by Publish Hour
![image](https://github.com/user-attachments/assets/2197027d-1e1a-4762-920b-ea81307f63da)

**Insights:**
This graph shows that:
- Most trending videos are published between 2 PM and 5 PM(14:00 to 17:00), with a clear peak at 4 PM.
- Posting in the afternoon greatly boosts the chance of trending, while early morning hours see the fewest trends.
- Timing your upload is a key factor for visibility.
- Posting your videos in the afternoon peak window (especially around 2–5 PM) can significantly increase their chances of trending and reaching a wider audience.

### Number of Trending Videos by Publish Day of Week
![image](https://github.com/user-attachments/assets/d6535b0f-a594-4b79-a5f9-f89df475ae3f)

**Insights:**
This graph shows that
- Most trending videos are published between Monday and Friday, with a peak on Wednesday and Thursday.
- Fewer trending videos are posted on weekends, especially Saturday and Sunday.
- To increase chances of trending, upload during weekdays.

## 📉 Results and Insights

### Key Insights:
- Videos often trend **within 0–1 days** of publishing
- Higher engagement scores correlate with quicker trending
- **Upload timing** (hour/day) may influence trending behavior
- **Text length and tag count** can help assess content richness

---

## 🧪 Usage

```bash
# 1. Clone the repository
git clone https://github.com/your-username/Youtube-Trending-Analysis.git

# 2. Navigate to the project directory
cd Youtube-Trending-Analysis

# 3. Launch the notebook
jupyter notebook Youtube_Trending_Analysis_Main.ipynb
```

---

## 🤝 Contributing

Feel free to contribute improvements, feature ideas, or visualizations. Open an issue or pull request.

---

## 📬 Contact

- GitHub: `AhsanNFt`
- Email: syedahsan0991@gmail.com
