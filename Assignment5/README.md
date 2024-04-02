# Collaborative Filtering Recommender System

## Overview
This project is my fifth assignment for the Machine Learning course. It contains a practical implementation of a recommender system using the collaborative filtering learning algorithm. Our focus is on recommending movies based on user ratings, applying concepts that can easily be adapted to other recommendation needs. The goal is to match users with movies they're likely to enjoy, based on their past preferences.  

# Features
- Notation System: The algorithm employs a specific notation to represent users, movies, and their ratings efficiently.  
- Algorithm Implementation: We implement the collaborative filtering algorithm to predict how users might rate movies they haven't yet watched.  
- Data Normalization: Ratings are normalized to adjust for users who rate more harshly or more leniently than average.  
- Learning Movie Recommendations: The system is trained with existing user ratings, improving its accuracy in predicting future ratings.  
- Customizable User Ratings: Users can input their movie ratings to receive personalized recommendations.  

# Getting Started
**Packages**: TensorFlow, NumPy, and Pandas.  

**Usage**: 
- Load the Data: Start by loading the movie dataset, which contains user ratings for various movies.  
- Customize Your Ratings: Input your ratings for any movies you've already seen. This will be used as the basis for your recommendations.  
- Train the Model: Execute the collaborative filtering algorithm to learn from the dataset.  
- Get Recommendations: Once the model is trained, we can see which movies the system recommends based on the input.  

# Data Structure
The project utilizes several key matrices to represent the data:  
- Ratings Matrix (Y): Contains the ratings users have given to movies.  
- User Preferences Matrix (X): Represents the feature ratings for movies.  
- User Features Matrix (W): Contains the parameters for each user, reflecting their preferences.  

# Customizing the Recommendations
To customize the recommendations, edit the my_ratings variable in the script by assigning ratings to movie IDs as shown in the comments. This personalization allows the system to tailor its recommendations to anyone's tastes.

# Conclusion
This project demonstrates the power of collaborative filtering in building a movie recommendation system. By analyzing patterns in user ratings, it can predict user preferences for unrated movies, making personalized recommendations. 
