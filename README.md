# Predicting-Fungal-Habitat-Types-Using-Taxonomic-Classification-and-Observation-Data

Fungi play a vital role in ecosystems, contributing to nutrient
cycling and plant health. Despite their importance, our
understanding of fungal habitats is limited, hindering conservation
efforts and ecosystem management. This project explores the use
of machine learning to bridge this gap by answering the question:
"Can we predict the habitat type of a fungal species based on its
taxonomic classification and observation details?" Utilizing a
Random Forest model and k-fold stratified cross-validation, we
aim to reveal patterns in fungal habitats, offering insights that
could guide conservation strategies and enhance our ecological
knowledge.

## Research Objective
Can we predict the habitat type of a fungal species based on its
taxonomic classification and observation details?"

## Methodology
Our project utilized a structured methodology to predict fungal
habitat types from taxonomic classification and observation details.
The process encompassed several key phases:

## Data Preparation
We began by selecting relevant features
('family', 'genus', 'month') and our target
variable ('habitat'), ensuring the dataset was
separated of missing values for these fields.
Recognizing the diversity of habitats, we
simplified the target variable by focusing on the
most common habitat types and grouping the
remaining ones under an 'Other' category. This
step was critical for managing the dataset's
complexity and ensuring a focused analysis.

## Feature Encoding
To make our categorical data suitable for
machine learning analysis, we applied one-hot
encoding to the 'family', 'genus', and 'month'
features. This transformation expanded our
feature set, enabling the model to effectively
interpret and utilize these categorical inputs.

## Label Standardization
We standardized the habitat labels to ensure
consistency, addressing variations in
capitalization and merging similar categories.
Subsequently, we applied label encoding,
converting these standardized categories into
numerical labels, facilitating their use as the
target variable in our model.

## Model Application
We selected the Random Forest algorithm for
its robustness and ability to handle complex
datasets. Implementing k-fold stratified crossvalidation,
we assessed the model's performance
across different data segments, employing
accuracy, precision, recall, and F-score as our
evaluation metrics. This evaluation approach
provided insights into the model's predictive
capabilities and areas for improvement.

## Findings
Our analysis on predicting fungal habitat types through a Random Forest model, revealed distinct
insights into the ecological knowledge of fungi. The model, evaluated through k-fold stratified crossvalidation,
achieved a moderate mean accuracy of approximately 57.68%. This indicates a fair
predictive capability across the simplified habitat categories: 'coniferous woods', 'mixed woods', and
'other'.

![image](https://github.com/user-attachments/assets/fff98966-dc97-4e5c-b361-fc41f1376d30)

## Performance Metrics by Habitat Type
In this bar chart, we illustrated the model's precision,
recall, and F-score for each habitat category, with
'coniferous woods' and 'other' categories achieving
relatively higher scores compared to 'mixed woods'.
This highlighted the model's strength in identifying
certain habitats while also pinpointing areas for
improvement, particularly in the accurate prediction
of 'mixed woods'.

![image](https://github.com/user-attachments/assets/6c24965c-7034-4c6c-939d-a2c04ee9375b)

## Conclusion
The model showed particular strength in predicting
habitats classified under 'coniferous woods' and
'other'. However, the 'mixed woods' category
presented a challenge, revealing lower performance
metrics and indicating the need for more balanced or
enriched data representation for this habitat type..
This project represents a step towards harnessing the
power of data science in understanding fungal habitats.
It opens possibilities for further research, including
exploring more sophisticated models, and applying the
model to broader datasets, which could enhance our
predictive accuracy and contribute to the conservation
and management of fungal biodiversity.

