# British Airways Virtual Internship

This repository contains my contribution to the Virtual Experience Program provided by **British Airways**. The program includes two primary tasks related to **data scraping**, **sentiment analysis**, and **predictive modeling**. Below is a detailed breakdown of each task and the methods used to solve them.

## Table of Contents
- [Overview](#overview)
- [Task 1: Web Scraping and Sentiment Analysis](#task-1-web-scraping-and-sentiment-analysis)
  - [1.1 Scraping Reviews from the Web](#11-scraping-reviews-from-the-web)
  - [1.2 Data Cleaning and Preprocessing](#12-data-cleaning-and-preprocessing)
  - [1.3 Sentiment Analysis](#13-sentiment-analysis)
- [Task 2: AutoML for Customer Booking Prediction](#task-2-automl-for-customer-booking-prediction)
  - [2.1 Feature Selection](#21-feature-selection)
  - [2.2 Building the AutoML Model](#22-building-the-automl-model)
- [Installation](#installation)
- [Usage](#usage)
- [Conclusion](#conclusion)
- [License](#license)

## Overview

This project consists of two tasks:
1. **Task 1**: Performing web scraping, data cleaning, and sentiment analysis on customer reviews.
2. **Task 2**: Building a predictive model using **AutoML** to predict customer bookings and identifying key features related to customer behavior.

## Task 1: Web Scraping and Sentiment Analysis

### 1.1 Scraping Reviews from the Web
In this part of the project, customer reviews were scraped from websites to collect feedback on British Airways services. The scraping process involved:
- Extracting the review text, rating, and other relevant information.
- Using Python libraries like **BeautifulSoup** and **Scrapy** for scraping reviews from target websites.

### 1.2 Data Cleaning and Preprocessing
Once the reviews were scraped, the next step was cleaning and preprocessing the data:
- **Removing noise** such as HTML tags, special characters, and irrelevant information.
- **Tokenizing** the review text into individual words.
- **Lowercasing** and **removing stopwords** to standardize the text data.

### 1.3 Sentiment Analysis
The cleaned review data was then analyzed to determine the **sentiment** (positive, negative, or neutral) of each review. The process involved:
- Converting the textual data into numerical features using **TF-IDF** or **Bag of Words**.
- Training a **Naive Bayes** model for sentiment classification.
- Evaluating the performance of the model using metrics like **accuracy**, **precision**, **recall**, and **F1-score**.

## Task 2: AutoML for Customer Booking Prediction

### 2.1 Feature Selection
The dataset provided by British Airways contained several features related to customer bookings. To build an effective model, I performed feature selection:
- **Exploratory Data Analysis (EDA)** was conducted to understand the relationships between features.
- Statistical techniques like **correlation analysis** and **feature importance ranking** were used to select the most significant features that influence customer bookings.

### 2.2 Building the AutoML Model
An **AutoML** approach was used to automate the process of building and selecting the best machine learning model for predicting customer bookings:
- **AutoML frameworks** like **H2O.ai** or **TPOT** were used to train multiple models and optimize hyperparameters.
- The model was evaluated based on **accuracy**, **precision**, and other key performance metrics.
- The best model was selected for deployment based on its performance on the validation dataset.

## Installation

To run this project, you need to install the following Python libraries:

```bash
pip install numpy pandas scikit-learn beautifulsoup4 scrapy requests
```
## Usage 
1. Clone the repository:
```bash
git clone https://github.com/yourusername/British_Airways_Virtual_Intership.git
cd British_Airways_Virtual_Intership
```
2. Run the scraping script:
 You can run the web scraping script to collect reviews by executing the following command:
```bash
python scrape_reviews.py
```
3. Sentiment Analysis:
Once the reviews are scraped and cleaned, run the sentiment analysis notebook:
```bash
python automl_customer_bookings.py
```
## Conclusion
This project showcases the application of data scraping, sentiment analysis, and AutoML techniques in real-world business scenarios like those faced by British Airways. Sentiment analysis helps understand customer opinions, while predictive modeling aids in improving customer engagement by predicting their future actions.
