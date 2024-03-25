# DataMining Project

## Date

    March 2024

## Contributors

-   HADJ-HAMDRI Mohammed-Amine
-   TAHIRI EL ALAOUI Youness

## Introduction

The goal of this project is to create a recommendation system for images based on user preferences. The project is divided into the following tasks:
    - Collecting images/data
    - Data Analysis
    - Data Visualization
    - Recommendation System
    - Tests
    - Report
  
## Data Sources

The images are collected from the Wikidata Query Service. The images are licensed under the Creative Commons Attribution-ShareAlike 3.0 Unported License. 

## Size of Data

The size of the data is arround 100 images. 

## Information Stored for Each Image

The following information is stored for each image:
    - Image URL
    - Image Title
    - Image Description
    - Image Author
    - Image License
    - Image Date
    - Image Tags
    - Image Size
    - Image Orientation
    - Image Colors
    - Image Camera Model
    - Image Resolution
    - Image Exposure Time
    - ...
  
## Format of Data

    Images: the format of the images is .jpg but the code can accept other formats.
    Data: the format of the data is .json.

## Data Analysis

    To get the 3 most frequent colors in an image, we used the KMeans algorithm. The algorithm is used to cluster the pixels of the image into 3 clusters. The 3 clusters represent the 3 most frequent colors in the image.

    For the orientation and the size, we use the height and the width of the image to deduce it.

    For the tags, we use the tags provided by the Wikidata Query Service.

## Data Visualization

    We use the matplotlib library to visualize the data. We vizualize the 3 most frequent colors in an image, the orientation and the size of the image.



## User Preferences

    User preferences are defined by the user's favorite images. For that, we have an algorithm that display a set of images and the user will choose the images that he likes. From that, we can deduce the user preferences (tags, colors, orientation, ...).


## Recommendation System

    The recommendation system is based on the user preferences. The system will recommend images that are similar to the user preferences. The similarity is based on the tags, colors, orientation, size, ...

    For this, we choose a machine learning algorithm from the scikit-learn library: the KNeighborsClassifier. The algorithm is used to find the k-neighbors of a point. In our case, the algorithm is used to find the k-neighbors of the user preferences.

## Tests






