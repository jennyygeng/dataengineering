# Spotify Data Pipeline: Tracking the Road to a Billion Streams 🎵

An end-to-end data engineering project that extracts, transforms, and loads (ETL) Spotify artist and track data to analyze the performance of BTS's top songs. 

This repository features two versions of the pipeline: the original foundational project, and a Senior Capstone refactor that implements Object-Oriented Programming (OOP) and advanced feature engineering.

## 📌 Project Evolution

### 🌱 V1: The Original Pipeline (`ISTA_322_Final_Project.ipynb`)
The original pipeline demonstrating foundational cloud and data extraction skills. 
* **Cloud Architecture:** Extracted data via the Spotify API, transformed it using Pandas, and loaded it into an AWS ecosystem (S3 and RDS MySQL). *(Note: AWS infrastructure was successfully deployed and tested, but spun down to prevent recurring cloud costs).*
* **Stakeholder Presentation:** Includes a comprehensive slide deck (`ISTA 322 Final Project Presentation.pdf`) detailing the ETL process, database schemas, and data visualizations.

### 🚀 V2: Senior Capstone Refactor (`DATA 498 Project 1.ipynb`)
For my senior capstone, I completely re-architected the original script to reflect professional software engineering standards.
* **Object-Oriented Design:** Encapsulated the ETL workflow into a reusable `BTSDataPipeline` Python class for cleaner, modular code.
* **AI-Assisted Refactoring:** Leveraged Google Gemini to accelerate the code refactoring process, optimizing the transition from procedural scripts to robust OOP architecture. 
* **Feature Engineering:** Engineered new metrics, including `avg_daily_streams` and a `momentum_score`, to better analyze performance trends.
* **Local Database:** Transitioned from cloud storage to a lightweight, local SQLite relational database for efficient structured querying.

## 🛠️ Tech Stack
* **Language:** Python (Pandas, Spotipy), SQL
* **Infrastructure & Storage:** SQLite, AWS (S3, RDS MySQL - V1)
* **Environment:** Google Colab / Jupyter Notebook

## 📂 Repository Contents
* **`DATA 498 Project 1.ipynb` & `.pdf`**: The V2 refactored OOP pipeline and accompanying summary report.
* **`ISTA_322_Final_Project.ipynb`**: The V1 original cloud-based pipeline.
* **`ISTA 322 Final Project Presentation.pdf`**: Visual slide deck summarizing the original V1 methodology and findings.
* **`BTS - Spotify Top Songs.csv`**: The Kworb streaming dataset utilized in both iterations.
