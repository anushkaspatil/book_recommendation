# Book Recommendation Algorithm using K-Nearest Neighbors

This project implements a book recommendation algorithm using the K-Nearest Neighbors (KNN) algorithm. The recommendation system is developed based on the Book-Crossings dataset, which contains 1.1 million ratings of 270,000 books by 90,000 users.

## Project Overview

The main goal of this project is to create a function (`get_recommends`) that takes a book title as an argument and returns a list of 5 similar books with their distances from the input book.

## Data Cleaning and Preprocessing

- The dataset is loaded from external sources and consists of book information and user ratings.
- Columns are appropriately renamed for better readability.
- Users with less than 200 ratings and books with less than 100 ratings are filtered out to ensure statistical significance.

## Implementation

- The Nearest Neighbors algorithm from scikit-learn is utilized for measuring the distance and determining the "closeness" of book instances.
- A pivot table is created for KNN, and the model is fitted with the cosine similarity metric.
- The `get_recommends` function takes a book title as input, locates the book in the dataset, and returns a list of 5 recommended books with their distances.

## Usage

To test the recommendation algorithm, you can use the provided testing cell or call the `get_recommends` function with a specific book title.

```python
get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")
```
## FreeCodeCamp

This project is developed as part of the FreeCodeCamp Machine Learning with Python curriculum challenge. 
