# 🌍 TouristHelp – Smart Travel Recommender using ML & Flask

**TouristHelp** is a personalized travel recommendation system built using **Python**, **Flask**, and **Machine Learning**. The system suggests travel destinations based on user preferences, travel history, and demographic information. It uses **collaborative filtering** and **content-based techniques** to generate real-time, customized travel suggestions for users.  

This project demonstrates the power of **data science** in enhancing user experience in the **tourism industry**. Whether you're a solo traveler, family planner, or adventurer, this app finds your next best destination.

---

## 🧠 Project Objective

To build a smart **Travel & Tourism Recommendation System** that analyzes user profiles, preferences, and history to recommend **personalized travel destinations** using machine learning techniques.

---

## 📌 Problem Statement

Users often struggle to find destinations that match their interests, group size, or seasonal preferences. Static lists or generic travel blogs fail to provide **personalized experiences**. This system solves that by:

- Understanding user preferences (demographics, travel type, interests)
- Analyzing travel history and ratings
- Recommending meaningful, relevant destinations

---

## 📊 Dataset Information

**Source**: [Kaggle – Travel Recommendation Dataset](https://www.kaggle.com/datasets/amanmehra23/travel-recommendation-dataset)

### 📁 Key Files:
- `Expanded_Destinations.csv` – Details of various travel destinations
- `Final_Updated_Expanded_UserHistory.csv` – User interaction history
- `final_df.csv` – Preprocessed data for model training

### 🧾 Features:
- `DestinationID`, `Name`, `State`, `Type`, `BestTimeToVisit`
- `Preferences`, `Gender`, `NumberOfAdults`, `NumberOfChildren`, `ExperienceRating`

---

## 🧮 Machine Learning Techniques Used

### ✅ 1. **Content-Based Filtering**
- Uses **user input features** like destination type, state, season, preferences, gender, group size.
- Predicts whether the destination will be **popular** using a **Random Forest Classifier**.
- All categorical features are label-encoded.

### ✅ 2. **Collaborative Filtering**
- Based on **user similarity** calculated via **cosine similarity** on user-item matrix.
- Recommends destinations visited and rated highly by similar users.
- No deep learning or embeddings needed — efficient and interpretable.

---

## 🚀 Tech Stack

| Layer             | Technology             |
|------------------|------------------------|
| Frontend         | HTML |
| Backend          | Python (Flask)         |
| ML & Data        | Pandas, NumPy, Scikit-Learn |
| Recommendation   | TF-IDF, Cosine Similarity, Random Forest |
| Deployment Ready | Render / Railway       |

---

## ✨ Features

- 📍 Recommends **Top 5 Destinations** based on similar travelers
- 💬 Predicts whether a trip is likely to be **popular or not**
- 👥 Supports demographic filters (gender, children, adults)
- 🗺️ Location + seasonal filtering (Type, State, Best Time to Visit)
- 🔄 Combined approach: **Collaborative + Content-based**
- 🧠 In-memory processing for fast response

---

## 🛠️ How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Anishhar03/touristhelp.git
cd touristhelp
