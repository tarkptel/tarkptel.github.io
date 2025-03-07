# 📚 Book Recommendation System  

![Movie Recommendation System](/assets/images/books.jpg)

## 📝 Project Description  
This is a **Flask-based web application** that recommends books based on **popularity and ratings**. The system is built using a **collaborative filtering approach** and primarily utilizes a **popularity-based** model to suggest books with the highest ratings.  

🔗 **Live Demo** – [Book Recommendation System](https://popular-book-recommend-2.onrender.com)  

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/popular-book-recommend)

---

## 🚀 How to Use  
1️⃣ **Visit the homepage** to see the top recommended books.  
2️⃣ **Enter the book name** or search criteria in the input box.  
3️⃣ **Click "Recommend"** to see the suggestions.  

---

## 📂 Dataset  
The project uses a **book recommendation dataset** from **Kaggle** for training and evaluation.  

🔗 **Kaggle Dataset Link** – *(Provide actual link here)*  

---

## 🔍 Model Training Approach  
The book recommendation system is trained using the following steps:  

1️⃣ **[popular_book]** – Identifies the **top 50 most popular books** based on ratings and votes.  
2️⃣ **[stan_df]** – Filters users who have rated more than **200 different books**.  
3️⃣ **[rating_50_book]** – Selects books that have received **more than 50 ratings** (i.e., rated by at least 50 different users).  
4️⃣ **[pt]** – Creates a **pivot table** for `rating_50_book` based on ratings and votes.  
5️⃣ **[similarity_s]** – Computes the **similarity score** between books.  
6️⃣ **Recommendation Function** – Given a book name, the system suggests **6 most related books**.  

---

## 🌍 Deployment (Render)  
The model is deployed online using **Render.com** for easy accessibility.  

### 🔧 Deployment Steps:  
1️⃣ **Render Setup** – Create a **Render.com** account and set up a new **"Web Service"**.  
2️⃣ **Connect GitHub** – Link the Render service to this GitHub repository.  
3️⃣ **Configure Build Commands** – Review and adjust the **build commands** (auto-detected for Python projects).  
4️⃣ **Deploy** – Click **"Deploy"**, and Render will build & launch the app.  
5️⃣ **Access** – Use the **Render URL** to access the deployed system.  

---

## 🔮 Future Enhancements  
📌 **User-Based Filtering** – Recommend books based on individual user preferences.  
📌 **Content-Based Filtering** – Suggest books using **textual similarities** in descriptions.  
📌 **Hybrid Model** – Combine **popularity-based & collaborative filtering** for improved accuracy.  
📌 **Enhanced UI** – Develop a **more interactive & visually appealing interface**.  

---

🎉 *This project helps book lovers discover new recommendations effortlessly!* 🚀  
