# 🎬 Movie Recommendation System Using KNN  

![Movie Recommendation System](/assets/images/mr2.png)

## 🔍 Overview  
This project is a **movie recommendation system** built using the **K-Nearest Neighbors (KNN) algorithm**. The system suggests movies similar to a given movie based on **genres** and **average ratings**, leveraging the popular **MovieLens dataset**.  

---

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/KNN-Movies-Recommendation)


## 🚀 Features  
✅ **Dataset Merging** – Combines movie metadata and user ratings for unified processing.  
✅ **Genre Encoding** – Encodes multi-genre data for better analysis.  
✅ **Aggregated Ratings** – Uses average movie ratings as a key feature.  
✅ **KNN Implementation** – Leverages cosine similarity to recommend similar movies.  

---

## 🔄 Project Workflow  

### 1️⃣ Data Loading  
The project uses two datasets:  

- **Movies Metadata** – Contains details like `movieId`, `title`, and `genres`.  
- **User Ratings** – Includes user preferences in the form of ratings.  

### 2️⃣ Data Merging  
Datasets are merged on the `movieId` column to align **movie details** with their respective **ratings**.  

### 3️⃣ Feature Engineering  
- **Multi-genre encoding** using `MultiLabelBinarizer`, converting genres into binary features.  
- This allows the model to compare movies based on **genre similarity**.  

### 4️⃣ Aggregation  
For each movie, the following features are calculated:  
- **Average Rating** – Summarizes user feedback.  
- **Genre Binary Features** – Indicates the presence of specific genres.  

### 5️⃣ Recommendation Model  
- The **KNN algorithm** is used to find movies **similar** to a selected one.  
- **Cosine similarity** measures similarity between movies based on their **features**.  

---

## 🛠️ Technologies Used  
🔹 **Python** – Programming language for implementation.  
🔹 **Pandas** – Data processing and aggregation.  
🔹 **Scikit-learn** – Encoding genres and implementing KNN.  

---

## Why KNN?  
✔️ **Simple and effective** – Works well for similarity-based recommendations.  
✔️ **No assumption of data distribution** – Unlike some parametric models.  
✔️ **Cosine similarity** – Ideal for comparing high-dimensional data like movie genres.  

---
