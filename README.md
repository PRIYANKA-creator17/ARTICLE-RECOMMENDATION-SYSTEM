# ARTICLE-RECOMMENDATION-SYSTEM

# News Article Recommendation System Using MongoDB

This repository contains a project report on the development of a News Article Recommendation System using MongoDB. This system is designed to provide personalized news recommendations to users based on their preferences and behaviors.

## Table of Contents

1. [Abstract](#abstract)
2. [Introduction](#introduction)
3. [Literature Survey](#literature-survey)
4. [Dataset Description](#dataset-description)
5. [Existing System](#existing-system)
6. [Problem Statement](#problem-statement)
7. [Proposed Methodology](#proposed-methodology)
8. [Implementation](#implementation)
9. [Results](#results)
10. [Conclusion](#conclusion)
11. [Future Work](#future-work)
12. [References](#references)

## Abstract

In today's digital landscape, delivering personalized content has become critical. This project delves into the development of a tailored recommendation system using MongoDB. The process includes data gathering, preprocessing, and applying content-based filtering techniques. The system leverages user-article interaction matrices and content-based feature extraction techniques like TF-IDF to enhance user experiences.

## Introduction

The project addresses the challenge of information overload by developing a sophisticated content-based news article recommendation system. The system leverages machine learning algorithms and user behavior analysis to provide users with a curated selection of articles aligned with their individual preferences and interests.

### Objectives

- **Personalization:** Tailor news recommendations based on user preferences, interactions, and content engagement.
- **Algorithmic Analysis:** Employ advanced machine learning algorithms to analyze user behavior patterns.
- **Real-time Adaptability:** Develop a system that adapts in real-time to user interests and emerging trends.

## Literature Survey

A comprehensive review of existing literature on news recommendation systems, collaborative filtering, content-based filtering, and the integration of NoSQL databases like MongoDB for handling vast and dynamic user data.

## Dataset Description

### Topics

The news dataset includes six distinct topics: Politics, Health, Emotion, Financial, Sport, and Science.

### Attributes

- Title
- Date
- Category (Topic)
- Description
- Source
- URL
- Author

### Content

The NBC News Dataset (2010-2020) includes user interactions like reading, liking, or sharing news articles, which help in building user profiles and understanding their interests.

## Existing System

Existing news article recommendation systems utilize NoSQL databases like MongoDB for efficient storage and retrieval of user interactions and preferences. The schema-less design of NoSQL databases caters to the dynamic attributes of news articles and supports real-time updates and query retrieval.

## Problem Statement

The project aims to develop a hybrid recommendation system to tackle the challenge of information overload in news consumption. The system leverages NoSQL databases for efficient storage and retrieval of user profiles, combining collaborative and content-based filtering to offer a more personalized and responsive news experience.

## Proposed Methodology

The system employs a multi-faceted strategy, starting with topic identification through NLP on a sample dataset. It combines collaborative filtering using the NBC News Dataset and content-based filtering based on topic analysis. MongoDB is used for its flexibility and scalability, facilitating real-time recommendations.

![image](https://github.com/user-attachments/assets/c79e6ecf-1886-4139-8de0-841e36de36cf)

## Implementation

### MongoDB Database Setup

- **Database:** RECSYS
- **Collections:** ARS (news articles and user interactions), class (data for topic classification)

### Data Exploration and Visualization

- Data is retrieved from MongoDB and converted into a Pandas DataFrame for Exploratory Data Analysis (EDA).

### Data Preprocessing

- Combining sample news datasets and the NBC News Dataset for a hybrid recommendation system.
- Topic identification using NLP and a combination of collaborative and content-based filtering.

### Content-Based Filtering

- TF-IDF encoding for text content.
- Vector space model for calculating cosine similarities between articles.

### Collaborative Filtering

- User-item interaction matrix and cosine similarity between users for recommendations.

### Hybrid Recommendation System

- Combining collaborative and content-based recommendations with assigned weights.

### Clustering

- K-means clustering for grouping news articles.

### Topic Classification Model

- XGBoost for topic classification based on article content.

### Final Recommendations

- Combining collaborative, content-based, and hybrid approaches for final recommendations.

### MongoDB Integration

- **Data Storage:** Store user profiles, preferences, past interactions, and item metadata.
- **Querying MongoDB:** Retrieve user profiles, item data, and interaction history for generating recommendations.
- **Generating Recommendations:** Use collaborative filtering, content-based filtering, and hybrid approaches.
- **Updating MongoDB:** Log new user interactions to keep recommendations up-to-date.

## Results

The system achieves an accuracy of 74% with varied precision, recall, and F1-scores across different classes, reflecting its strengths and weaknesses in classification performance.

## Conclusion

The project successfully developed a hybrid news article recommendation system using collaborative and content-based filtering. Future work includes data export for fine-tuning, cross-domain recommendations, advertisement management, real-time personalization, and enhanced user feedback mechanisms.

## Future Work

Enhancements to the system include incorporating user profiles, real-time updates, a user feedback and rating system, scalability solutions, and performance optimization.
