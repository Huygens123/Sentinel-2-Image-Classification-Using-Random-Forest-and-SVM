# Sentinel-2-Image-Classification-Using-Random-Forest-and-SVM

## **Project Overview**  
This project analyses Sentinel-2 satellite imagery for Iwo Local Government, Osun State, Nigeria. The study focuses on understanding spatial patterns, extracting key insights using machine learning models, and visualizing vegetation and land cover features.  

The workflow includes:  
1. Data exploration and preprocessing.  
2. Visualization of spectral bands and derived indices (e.g., NDVI).  
3. Implementation of machine learning models for land classification.  

---

## **Objectives**  
- Conduct an exploratory analysis to understand the spectral and spatial characteristics of Sentinel-2 data.    
- Apply machine learning models to classify land cover types and evaluate their performance.  

---

## **Data Sources**  
- **Sentinel-2 Imagery:** Multispectral satellite data providing high-resolution information across 13 spectral bands.  
- **Geospatial Shapefiles:** Boundary data of Iwo Local Government.  

---

## **Methodology**  

### **1. Exploratory Data Analysis (EDA)**  
- **Data Loading and Preparation:**  
  Loaded and preprocessed Sentinel-2 bands using `rasterio`, aligning and clipping the data to the study area.  

- **Data Visualization:**  
  - True-color and false-color composites were created to visually understand the landscape.
    ![Layer Composition](images/raster_band.png)
    The top left image shows the "Natural Color" view, which presents the landscape as it would appear to the human eye from above. In this image, we can see what appears to be an urban centre (appearing as a bright white area in the centre) surrounded by darker regions that likely represent less developed or natural areas

- **Statistical Analysis:**  
  Histograms and scatter plots highlighted the relationships between spectral bands, revealing patterns relevant to land cover classification.  

### **2. Machine Learning Models**  
After preprocessing the data, machine learning models were applied to classify land cover types:  
- **Algorithms Used:**  
  - Random Forest (RF)  
  - Support Vector Machine (SVM)
- **Model Evaluation:**  
  Models were evaluated using metrics such as accuracy, precision, recall, and F1-score. Confusion matrices were plotted to analyze performance across classes.  

---

## **Results**  
1. **EDA Findings:**  
   - NDVI maps revealed distinct zones of dense vegetation and sparse or degraded areas.  
   - Spectral band analysis indicated strong correlations useful for land classification.  

2. **Machine Learning Outputs:**  
   - Random Forest achieved the highest accuracy, effectively classifying forests, urban areas, and agricultural land.  
   - Gradient Boosting performed well in distinguishing mixed vegetation zones.  
   - Confusion matrices highlighted misclassification trends, such as overlaps between urban and barren lands.  

---

## **Tools and Libraries**  
- **Programming Language:** Python  
- **Data Manipulation:** `pandas`, `numpy`  
- **Visualization:** `matplotlib`, `seaborn`, `folium`  
- **Geospatial Analysis:** `rasterio`, `geopandas`, `earthpy`  
- **Machine Learning:** `scikit-learn`, `xgboost`  

---

## **Next Steps**  
- Perform temporal analysis to track vegetation and land-use changes over time.  
- Integrate field validation data to improve model accuracy.  
- Develop a web-based dashboard to visualize results interactively for decision-making.  

---

## **How to Use**  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-repo-name.git  
   cd your-repo-name  
   ```  

2. Install dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Run the notebooks:  
   Open Jupyter Notebook and follow the steps in the `EDA_and_Machine_Learning.ipynb` file.  

---

## **Contributors**  
- **Abdulquawiyy A. Owolabi** - Geospatial Scientist  

For questions or contributions, feel free to reach out or open an issue in this repository. 
