# Data Mining & Machine Learning Project

## Date

March 2024



## Introduction

This project is designed to create a sophisticated image recommendation system based on user preferences. By harnessing the power of data mining and machine learning techniques, we aim to personalize the user experience, presenting images that align closely with individual tastes and preferences. The workflow is segmented into several stages, each critical to the development and refinement of the recommendation engine:

- **Collecting Images**: Automated scripts fetch images from Wikidata, leveraging SPARQL queries to access a diverse repository of creative commons images.
- **Data Analysis**: Extract metadata from each image, including dimensions, EXIF data, and predominant colors, using libraries such as PIL (Python Imaging Library).
- **Data Visualization**: Visual insights are generated from the dataset, displaying trends in image characteristics such as size, orientation, and color distributions, utilizing matplotlib and pandas for plotting and data manipulation.
- **Recommendation System**: Develops a K-Nearest Neighbors (KNN) model to learn from user interactions (likes/dislikes) and recommend images with similar characteristics.
- **Tests**: Conduct tests to validate the accuracy and performance of the recommendation system.
- **Report**: A comprehensive report documenting the methodology, process, results, and insights gained during the project.

## Data Sources

Images are sourced from the Wikidata Query Service, with a focus on ensuring diversity and compliance with the Creative Commons Attribution-ShareAlike 3.0 Unported License. This approach ensures both a broad spectrum of images and adherence to licensing requirements for use and distribution.

## Size of Data

The initial dataset encompasses 150 images, providing a substantial variety for training the recommendation model and testing its efficacy.

## Information Stored for Each Image

Extensive metadata is collected for each image to facilitate detailed analysis and improve recommendation accuracy:

- **Image URL**: Direct link to the image source.
- **Image Title**: The name or title of the image.
- **Image Description**: A brief description or contextual information about the image.
- **Image Author**: The creator or photographer of the image.
- **Image License**: Information regarding the image's licensing terms.
- **Image Date**: The creation or publication date of the image.
- **Image Tags**: Relevant keywords or tags associated with the image.
- **Image Size**: The dimensions of the image (width x height).
- **Image Orientation**: Categorization as Landscape, Portrait, or Square based on dimensions.
- **Image Colors**: Analysis of predominant colors within the image.
- **Image Camera Model, Resolution, Exposure Time**: Technical details captured from the image's EXIF data, providing insights into the photography equipment and settings used.

## Format of Data

- **Images**: Primarily in .jpg format, but the system is equipped to process a range of image file types.
- **Data**: Metadata and user interactions are serialized in .json format, facilitating easy access and manipulation for analysis and machine learning purposes.

## User Preferences

User preferences are central to the recommendation logic. By engaging with the system—liking or disliking images—users generate data that informs the model about individual preferences. This feedback loop allows the system to refine its recommendations, ensuring that suggested images closely match user tastes.

## Technical Process and Libraries

- **SPARQLWrapper**: Used to query Wikidata for images.
- **Pandas & NumPy**: Handle data manipulation and analysis.
- **Pillow (PIL)**: Processes images for feature extraction, including resizing and color analysis.
- **Scikit-learn**: Implements the K-Nearest Neighbors algorithm for the recommendation system, alongside utilities for preprocessing and model evaluation.
- **Matplotlib**: Generates plots and visualizations to represent data insights and user preferences graphically.

## Machine Learning Model

The project employs a K-Nearest Neighbors (KNN) model, trained on user feedback and image metadata. This model identifies patterns in user preferences regarding image orientation, size, and color, recommending new images that share similar features with those liked by the user. The use of this model illustrates a practical application of machine learning to personalize content delivery, adapting recommendations based on user interactions.

## Future Directions

Future enhancements could include integrating more complex models, expanding the dataset, and refining user interaction mechanisms to capture more nuanced preferences. The goal is to continually improve the system's accuracy and relevance, making each user's experience as engaging and personalized as possible.

## Conclusion

This project underscores the potential of combining data mining with machine learning to create dynamic, user-centered recommendation systems. Through meticulous data analysis, visualization, and the application of a KNN model, we have laid the groundwork for a system that not only understands user preferences but also evolves with them, offering a truly personalized browsing experience.
