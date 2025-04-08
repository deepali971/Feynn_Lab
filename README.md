# 🧠 AI-Powered Local Tourism & Hotel Recommender System 🇮🇳

## 📌 Overview  
This project is a **comprehensive machine learning-based tourism and hotel recommender system** tailored for the Indian travel landscape. It provides **personalized travel recommendations** by analyzing geographic, categorical, and sentiment-based tourism patterns, and also delivers **intelligent hotel suggestions** using a hybrid recommendation system combining **content-based** and **collaborative filtering** techniques.

---

## 🧩 Problem Statement  
Tourists often struggle to find destinations and accommodations that align with their **personal preferences**, **budget**, and **review sentiments**. This project solves this by:
- Segmenting popular travel locations using clustering.
- Analyzing reviews, fees, and visit durations.
- Recommending hotels based on user behavior and content similarity.

---

## 🛠️ Approach  

### 🔹 Part 1: Tourism Clustering (Exploratory + Unsupervised Learning)

Applied three types of clustering techniques:
- **K-Means**
- **Hierarchical Clustering**
- **DBSCAN (Density-Based Spatial Clustering)**

#### Key Clustering Areas:
1. **Geographic Clustering**  
   Identify tourist hotspots across India based on latitude, longitude.

2. **Significance-Based Clustering**  
   Cluster based on **type of place**, **entry fees**, and **visit duration** to understand traveler behavior.

3. **Review-Based Clustering**  
   Analyze how **Google ratings**, **review counts**, and **entry fee structures** influence tourist interest.

📊 **Key Insights:**
- Highlighted popular regions and high-rated cities.
- Mapped fee structures across types of tourist spots.
- Correlation found between visit duration and review sentiment.

---

### 🔹 Part 2: Hotel Recommendation System (Recommender System)

A **hybrid recommendation engine** built to recommend the best hotels based on user preferences using:

#### 🔸 Content-Based Filtering
- Uses hotel attributes like **amenities**, **location**, **ratings**, and **price**.
- Computes **TF-IDF vectors** from hotel descriptions and similarity via **Cosine Similarity**.

#### 🔸 Collaborative Filtering
- Based on **user-hotel interaction matrix** (ratings).
- Applied **Singular Value Decomposition (SVD)** to uncover latent factors influencing user preferences.

#### 🔸 Hybrid Recommendation
- Combines both filtering strategies for **enhanced personalization** and **accuracy**.

---

## 🧼 Data Preprocessing

- Removed missing values and duplicates.
- Applied **Label Encoding** for categorical variables.
- Scaled features using **StandardScaler**.
- Normalized rating values for better collaborative filtering performance.

---

## 📚 Datasets Used

1. **Tourism Dataset**  
   [Guide to India's Must See Places – Kaggle](https://www.kaggle.com/datasets/saketk511/travel-dataset-guide-to-indias-must-see-places)

2. **Hotel Dataset**  
   - Simulated dataset of hotels with features: `hotel_name`, `city`, `rating`, `amenities`, `price`.  
   - Simulated `user-hotel` interaction data for collaborative filtering.

---

## 🚀 How It Works

| Functionality | Methodology |
|---------------|-------------|
| **Tourist Clustering** | Unsupervised ML (K-Means, DBSCAN, Hierarchical) |
| **Hotel Similarity** | Content-Based (TF-IDF + Cosine Similarity) |
| **User-Based Prediction** | Collaborative (SVD Matrix Factorization) |
| **Hybrid Recommendations** | Merge of content & collaborative results |

---

## 💡 Usage

You can use this system to:
- 🔍 Get **place recommendations** based on clustered preferences.
- 🏨 Receive **hotel suggestions**:
  - **By hotel name** – similar hotels (content-based).
  - **By user ID** – predicted preferences (collaborative).
  - **Hybrid** – for optimal personalization.

---

## 👥 Authors  
- Vishal Dangiwala  
- Deepali Malik

---

## 📈 Future Enhancements
- Integrate **real-time data** from APIs (Google Places, TripAdvisor).
- Add **user login system** and **travel planner UI**.
- Integrate **sentiment analysis on reviews** using NLP.

---




