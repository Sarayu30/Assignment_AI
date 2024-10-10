 
```markdown
# Webtoon Genre Classification

## Project Overview

This project aims to classify webtoon descriptions into predefined categories (genres) using machine learning techniques. The dataset contains various features related to different webtoons, and the goal is to predict their genres based on their descriptions and other attributes.

## Dataset

The dataset includes the following columns:

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
- **clean_tags**: List of cleaned tags
- **combined_text**: Combined text for analysis
- **features**: Additional features for classification
- **combined_features**: Combined features for model input
- **target**: Predefined target genres for classification

## Model Implementation

The project implements a **Decision Tree Classifier** using the Scikit-learn library to classify webtoons into genres. 

### Key Steps

1. **Data Preparation**: Combined the `title` and `clean_details` as features. The target variable was defined based on the first genre in the `clean_genres` column.
2. **Train-Test Split**: The dataset was split into training and testing sets.
3. **Feature Extraction**: Utilized TF-IDF vectorization for feature extraction.
4. **Model Training**: Trained a Decision Tree Classifier on the training data.
5. **Model Evaluation**: Evaluated the model's performance using accuracy and classification reports.

 
## Installation

To run this project, ensure you have the following libraries installed:

```bash
pip install pandas scikit-learn
```

## Usage

Clone the repository and run the notebook to see the classification results.

```bash
git clone https://github.com/yourusername/webtoon-genre-classification.git
cd webtoon-genre-classification
```

 
## Acknowledgements

- Scikit-learn for machine learning algorithms and tools.
- Pandas for data manipulation and analysis.

```
