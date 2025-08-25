# Enhanced Wildfire Prediction Using Multi-Source Real-Time Data


This project presents an innovative approach to wildfire prediction, leveraging machine learning to process spatiotemporal data and generate dynamic likelihood heatmaps. It is designed to be a robust tool for improving disaster response and resource allocation.

## 💡 Motivation
The escalating threat of wildfires poses a critical challenge to communities and ecosystems worldwide. Driven by the desire to create impactful, data-driven solutions, I developed this predictive model to contribute to more effective fire management and mitigation efforts. This project builds upon foundational research by integrating diverse data sources to create a more accurate and timely prediction system. My experience presenting this project at the Google AI Tinkerers meetup was a blast, offering the opportunity to engage with peers and learn from experts in the field.



## ✨ Features and Technical Implementation
This project is built around a comprehensive system that combines traditional environmental data with real-time information to improve predictive accuracy.


**Core Data Sources**: The model primarily uses MODIS data, which includes brightness values, latitude, longitude, and dates.

**Multi-Source Data Integration**: The system is designed to incorporate additional data for enhanced predictions, such as:


**Satellite Imagery**: To visually confirm fire locations and assess terrain and vegetation.


**Real-Time Data**: The project uniquely incorporates real-time emergency call records and crowd-sourced location data to identify new ignitions and rapid fire spread.



**External Factors**: It can integrate external factors like wind direction, temperature, and vegetation from public APIs to further refine predictions.


**Model Architecture**: The core of the project is a ConvLSTM (Convolutional Long Short-Term Memory) neural network. This architecture is particularly well-suited for analyzing sequential heatmaps to predict fire direction and growth.


**Key Libraries**: The project is implemented using core Python libraries, including:


_pandas_ and _numpy_: For data manipulation and numerical operations.



_tensorflow_ and _keras_: For building and training the ConvLSTM model.



_matplotlib_ and _seaborn_: For generating visualizations, including dynamic wildfire likelihood heatmaps.


## 🚀 Getting Started

The project is developed within a Google Colab environment.


**Data Acquisition**: The initial dataset can be found at /kaggle/input/hawaiiwildfiredata/MODIS_C6_1_USA_contiguous_and_Hawaii_7d.csv.


**Data Preprocessing**: The provided code outlines steps to sort data by date, create grid indices for latitude and longitude, and group data into time sequences to generate brightness grids for heatmaps.


**Model Training**: The notebook demonstrates how to build and train the ConvLSTM model using mse loss and the adam optimizer.

## 🗺️ Future Plans

While this project is a proof of concept, my goal is to enhance the framework's adaptability to a global scale by incorporating new data sources and adjusting time scales to hourly or even weekly intervals as more curated data becomes available. Furthermore, the methodology used for multi-source data integration and spatiotemporal modeling can be applied to predict other natural phenomena, such as droughts or hurricanes.
