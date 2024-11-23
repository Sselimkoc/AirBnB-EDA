# Airbnb Data Cleaning and Analysis

This project involves cleaning and analyzing Airbnb listing data to uncover insights into various aspects, including price distribution, neighborhood density, host activity, and more. The dataset used is the Airbnb Open Data, which has been processed to remove missing values, handle outliers, and ensure it’s ready for detailed analysis.

---

## Project Overview

### Data Cleaning

- **Missing Data Handling:**  
  Missing values in columns are dealt with using appropriate techniques such as filling with default values for categorical columns or imputing numerical columns with the median.

- **Feature Engineering:**  
  Columns are standardized for consistency (e.g., renaming for clarity), and irrelevant features (like `country_code` or `house_rules`) are removed to streamline the dataset.

- **Outlier Handling:**  
  Outliers in numerical columns like `price`, `service_fee`, and `construction_year` are identified and handled using boxplots and histograms.

- **Data Transformation:**  
  Data types are converted as necessary (e.g., converting `price` and `service_fee` to floats). Categorical columns such as `host_identity_verified` are transformed appropriately for easier analysis.

---

### Data Analysis and Visualization

- **Top Neighborhoods and Hosts:**  
  Insights are provided into the neighborhoods with the most listings and the hosts with the highest number of listings.

- **Price Distribution:**  
  Visualizations explore the distribution of prices and factors influencing them, such as neighborhood and room type.

- **Listing Density:**  
  An analysis of listing density is presented by geographic location (latitude and longitude).

---

## Libraries Used

- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for data visualizations
- `geocoder` for reverse geocoding latitude and longitude to neighborhood names

---

## Dataset

The dataset used in this project is the **Airbnb Open Data**, which contains various columns related to Airbnb listings in New York City. Key columns include:

- `name`: Listing name
- `host_name`: Host's name
- `neighbourhood_group`: Grouped neighborhood information
- `price`: Listing price
- `latitude` and `longitude`: Coordinates of the listing
- `number_of_reviews`: Number of reviews for the listing
- `service_fee`: Service fee associated with the listing
- `room_type`: Type of room (e.g., entire home, shared room)
- `construction_year`: Year the building was constructed

---

## Features

- **Missing Data Handling:**  
  Different strategies are applied to handle missing data, including filling default values for categorical columns and using the median for numerical columns.

- **Data Transformation:**  
  Irrelevant columns are dropped, data types are converted where necessary, and column names are standardized for clarity.

- **Geocoding:**  
  For missing neighborhood data, latitude and longitude coordinates are used for reverse geocoding to fill in neighborhood group information.

- **Data Visualizations:**  
  Several key visualizations are included, such as:
  - Price distribution by room type and neighborhood group.
  - Number of listings by neighborhood and host.
  - Listing density on a map based on geographic coordinates.

---

## How to Use

1. Clone or download the repository.
2. Open the Jupyter notebook `airbnb_analysis.ipynb`.
3. Import the necessary libraries (pandas, numpy, seaborn, matplotlib, geocoder).
4. Run the notebook step-by-step to load, clean, analyze, and visualize the data.

---

Kaggle notebook link : https://www.kaggle.com/code/selimkoc/notebook2f4620f073
