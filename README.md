# My Next Read

**My Next Read** is a hybrid book recommendation system that combines **Collaborative Filtering** and **Content-Based Similarity** to deliver personalized book suggestions. The system integrates user–item interaction data with textual metadata (title, author, genre, and description) to compute hybrid recommendation scores. Optimized for sub-100ms API responses, it features **modular data pipelines**, **efficient model evaluation**, and **reusable components** for extensibility across datasets.

The project architecture supports scalable deployment, modular retraining, and real-time recommendation generation through RESTful APIs. Built for both experimentation and production, **My Next Read** demonstrates end-to-end proficiency in **machine learning**, **data engineering**, **backend design**, and **system deployment**.

---

## Project Goal

In a world with millions of books available online, readers often struggle to discover titles that match their unique tastes and reading patterns. Traditional keyword or popularity-based systems fail to provide meaningful personalization.

**My Next Read** aims to solve this problem by developing a hybrid recommender system that:
- Combines collaborative filtering (user-behavior-based) and content-based filtering (metadata-based),
- Provides robust fallback recommendations for new users (cold start),
- Offers weighted hybrid scoring for adjustable personalization,
- Ensures fast, scalable, and modular performance for large datasets,
- Supports visual recommendation output (cover images, titles, and authors).

---

## Tech Stack

- **Python** (Pandas, NumPy, Scikit-learn)
- **Flask / FastAPI** for serving APIs  
- **SQLite / PostgreSQL** for data persistence  
- **Docker** for containerization  
- **HTML / CSS / JavaScript** for the front-end  
- **CI/CD** integration for automated builds and deployment  

---

## System Overview

- **Collaborative Filtering (KNN-based)** – recommends books based on user–item rating similarities.  
- **Content-Based Filtering (TF-IDF + Cosine Similarity)** – analyzes book descriptions and metadata to recommend similar items.  
- **Hybrid Scoring** – merges both approaches via weighted blending for optimal personalization.  
- **Data Pipelines** – clean, preprocess, and transform book datasets for model training.  
- **Model Persistence** – pre-trained models saved for fast API access.  

---

## How to Setup (Locally)
 Clone the Repository
```bash

git clone https://github.com/Khyati-Chouhan/My_Next_Read.git
cd My_Next_Read
```

 Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
Install Dependencies
```bash
pip install -r requirements.txt
```
 Run Flask App
```bash
python app.py
```
## How to Setup (Dockerized)

 Clone the Repository
```bash
git clone https://github.com/Khyati-Chouhan/My_Next_Read.git
cd My_Next_Read
```
Build Docker Image
```bash
docker build -t my-next-read .
```
 Run Docker Container
```bash
docker run -p 8501:8501 my-next-read
python app.py
```
## Deployment

Deploy easily on [Vercel](https://vercel.com), [Render](https://render.com), or [AWS EC2](https://aws.amazon.com/ec2/) for production use.  

