# 🐦 Twitter Bot Detection

## 📌 Project Overview

This project is about finding out which Twitter accounts are bots (automated accounts) and which ones are real users. I used Python and machine learning to analyze user behavior and tweet content. The model I built, called Relevance Vector Machine (RVM), was able to identify bots with **81.25% accuracy**.

## 🎯 Project Goals

- Collect Twitter data for analysis.
- Pull out important features from user profiles and tweets.
- Train a machine learning model to detect bots.
- Test the model and check how well it works.

## 🧰 Tools & Technologies Used

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Data Collection:** Twitter API, Twitonomy  
- **Machine Learning Model:** Relevance Vector Machine (RVM)  
- **Visualization:** Matplotlib, Seaborn  

## 📂 Project Structure

├── Python_Files/
│ ├── MergingTrainingData.py # Merges different datasets
│ └── RVMTrainingModel.py # Trains the RVM model
├── Raw_data_Files/
│ ├── Content_Data.csv # Data from tweets
│ └── Graph_Data.csv # Data from user networks
├── Training_Data_Files/
│ └── Training_Data.csv # Final dataset used for training
├── cresci-rtbust-2019/ # Public dataset folder (if used)
├── .ipynb_checkpoints/ # Auto-saved notebook versions
├── .Rhistory # R history file (if used)
└── README.md # This file


## 🔍 How It Works

### 1. Data Collection  
- I collected Twitter user data and tweets using:
  - `GET users/show` (Twitter API)
  - `GET statuses/user_timeline` (Twitter API)
- I also used [Twitonomy](https://www.twitonomy.com/dashboard.php) to get more details about user behavior.

### 2. Feature Extraction  
- **Content features**: Looked at how often people tweet, what they tweet, and the patterns in their content.  
- **Graph features**: Looked at how users are connected—followers, following, and mentions.

### 3. Data Preprocessing  
- Combined all the different data sources using a script to create a final training dataset.

### 4. Model Training  
- Trained an **RVM (Relevance Vector Machine)** model using a linear kernel.
- Achieved an **accuracy of 81.25%** in detecting bots.

## 📈 What I Found

- The model was able to correctly spot bots most of the time.
- Mixing tweet content and network behavior made the model stronger and more accurate.

## 📚 Helpful Resources

- [Twitter API Docs](https://developer.twitter.com/en/docs)
- [Tweepy for Python](http://docs.tweepy.org/en/latest/api.html)
- [Botometer Datasets](https://botometer.iuni.iu.edu/bot-repository/datasets.html)
- [GetOldTweets3 Tool](https://pypi.org/project/GetOldTweets3/)

---

