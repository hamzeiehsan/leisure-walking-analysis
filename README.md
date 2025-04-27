# Analysis of Points of Interests Recommended for Leisure Walk Descriptions


## Abstract
Leisure walking is a physical activity where locomotion through a natural or even urban environment is the goal in itself, e.g., in pursuit of health and wellbeing. In contrast to destination-oriented walks that are focused on navigation efficiency (i.e., shortest or simplest walk from source to destination), leisure walks emphasize experiencing the environment, engaging in activities, and discovering places that may be off route, or intermediate destinations en-route, summarily called points of interest (POIs). POIs are key for recommending leisure walks, yet a detailed analysis of POIs in the context of leisure walking is missing in the literature. This study extracts and annotates POIs of leisure walking recommendations available in [WalkingMaps.com.au](https://walkingmaps.com.au/), creating an annotated dataset  to address this research gap and provide a first analysis of leisure walking descriptions. We classify POIs using the verbal description provided in the dataset, match them with data available in OpenStreetMap (OSM), and compare the POIs with nearby alternatives in OSM. Our analysis reveals thematic and spatial patterns in POI selection, offering a machine learning approach to model POI choices for leisure walks. We further evaluate the availability of rich data in OSM for future automated leisure walking recommendation. This study contributes to automated systems for recommending leisure walks, tailoring suggestions based on available information in the spatial open data, and presents an annotated dataset to facilitate future research in this field.

## Topic Modelling
Topic modelling and annotation helper functions are provided in first notebook `1_topic_modelling.ipynb`. Here, we use Bertopic to discover topics for POI dataset, and further classify them by defining a hierarchical classification.

## Getting POIs from OSM
Here, we download OSM POIs in nearby leisure walks to provide candidate matching to POIs in leisure walking dataset and also present a contrast set of POIs (not selected) to test the POI selection methods. See `2_POIs_from_OSM.ipynb`.

## Annotation Analysis
Checking OSM matches using annotated data. Finding out how selective people are when choosing POIs for leisure walks. See `3_annotation_analysis.ipynb`

## Annotation Agreement
Analysing the annotation provided by two annotators and find out what's the agreement when we perform matching manually. See `4_annotation_agreement.ipynb`.


## POI Selection
Testing some baseline machine learning methods (considering both thematic and spatial aspects) in selecting POIs for leisure walks. See `5_POI_selection.ipynb`.


## Annotation Tool
A tool is developed for annotating, and used by both annotators. This tool is provided in a separate GitHub repo: https://github.com/hamzeiehsan/leisure_walk_annotation 