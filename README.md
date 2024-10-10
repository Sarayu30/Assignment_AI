# Webtoon Genre Classification and Chatbot

## Project Overview

This project focuses on classifying webtoon descriptions into predefined genres using machine learning techniques and developing a chatbot to answer user queries about specific webtoons. The notebook covers the dataset's features, classification approach, model improvement suggestions, and chatbot interaction examples.

## Key Components

### 1. Webtoon Dataset Description
- The dataset includes the following columns:
  - **title**: The name of the webtoon
  - **item_id**: Unique identifier for the webtoon
  - **link**: URL to the webtoon
  - **cover**: Cover image URL
  - **creators**: The creators of the webtoon
  - **genres**: List of genres associated with the webtoon (multi-label)
  - **views**: Number of views
  - **subscribers**: Number of subscribers
  - **likes**: Number of likes
  - **banner**: Banner image URL
  - **details**: Description of the webtoon
  - **tags**: List of tags
  - **episodes**: Number of episodes
  - **released**: Release date
  - **clean_details**: Cleaned description
  - **clean_genres**: List of cleaned genres
  - **target**: Predefined target genres for classification

### 2. Classification Approach
- Initially, the first genre in the `clean_genres` column was used for classification.
- The project considers transitioning to a more nuanced multi-label classification since webtoons can belong to multiple genres.

### 3. Model Improvement Suggestions
1. **Data Augmentation**: Collect more webtoon descriptions to balance genres.
2. **Multi-Label Classification**: Implement techniques to handle multi-label genres using Scikit-learn's `MultiLabelBinarizer`.

### 4. Detailed Steps
- The notebook provides code for processing text data, preparing input features for the model, and suggestions for enhancing accuracy, particularly for the multi-label classification task.

### 5. Chatbot Response Generation
- The notebook outlines the development of a **chatbot** that can respond to user queries about a specific webtoon (Castle Swimmer). The chatbot uses **NLP techniques** to analyze the text and extract key information, including characters and themes.

### 6. Example Interaction
- Users can interact with the chatbot, asking for character details, the protagonist’s journey, or themes of the webtoon.

## Installation

To run this project, ensure you have the following libraries installed:

```bash
pip install pandas scikit-learn nltk

## Usage
-git clone https://github.com/yourusername/webtoon-genre-classification.git
-cd webtoon-genre-classification
