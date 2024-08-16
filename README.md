# Content Based Filter Recommendation System With FuzzyWuzzy

## Project Introduction

<p>This project is a personal initiative aimed to develop an algorithm for a content-based product e-commerce recommendation system. The algorithm will recommend product based on the similarity of their name, category, brand, and department</p>

## Objectives
<ul>
  <li>
    Develop a content-based recommendation algorithm to suggest product name similar to those a user has shown interest in.
  </li>
  <li>
    Implement text processing and feature extraction techniques to represent product content.
  </li>
</ul>

## Dataset
The dataset I used is from an open dataset on BigQuery. Here is the link where you can access the dataset.

## Methodology
1. Data Preprocessing
   <ul>
     <li>
       Data Cleaning: Checking duplicate and handling missing data
     </li>
     <li>
       Delete Data: Deleting data that not corralated with the objectivity
     </li>
   </ul>
2. Feature Engineering
   <ul>
     <li>
       One-Hot Encoder: convert categorical data into numerical data
     </li>
     <li>
       TF-IDF Vectorization: Transform product name into TF-IDF vectors to capture the importance of terms relative to the product name.
     </li>
   </ul>
3. Similarity Calculation
   <ul>
     <li>
       Cosine Similarity: Compute the cosine similarity between the feature vectors of product to measure content similarity.
     </li>
   </ul>
4. Recommendation Algorithm
   <ul>
     <li>
       Title Matching: Compare product name using FuzzyWuzzy to find product with similar names.
     </li>
     <li>
       Score Aggregation: Combine similarity scores from product name, category, brand, and department to generate an overall similarity score for each product.
     </li>
     <li>
       Ranking: Rank the recommended product based on their aggregated similarity scores.
     </li>
   </ul>
   
