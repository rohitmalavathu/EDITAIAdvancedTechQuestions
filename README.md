# **Project: EDITAISummerInternship**  

---

## **Overview**  
This project focuses on analyzing the Nucleus-to-Cytoplasm (NC) ratios of urine cells and evaluating model performance using Mean Absolute Error (MAE). It includes a PyTorch-based image segmentation model to predict masks for input images.  

---

## **Data Sources**  
The dataset consists of images and their corresponding segmentation masks. The masks are used to determine the NC ratio, which serves as an indicator of potential malignancy. The data comes from https://github.com/jlevy44/PreliminaryGenerativeHistoPath.

---

## **Methodology**  
1. **NC Ratio Calculation** – Extracts nucleus and cytoplasm pixel counts to compute the NC ratio.  
2. **Statistical Analysis** – Evaluates predicted NC ratios against real values using Mean Absolute Error (MAE).  
3. **Deep Learning Model** – Utilizes a PyTorch-based segmentation model to predict masks and assess NC ratios.  
4. **Visualization** – Outputs scatter plots to analyze gene expression correlations.  

---

## **Key Features**  
- **Automated NC Ratio Computation** – Extracts meaningful biological insights from image masks.  
- **Model Performance Evaluation** – Uses MAE to assess prediction accuracy.  
- **Image Segmentation** – Employs deep learning for mask generation.  
- **Flexible Data Processing** – Designed to handle various dataset formats.  

---

## **Dependencies**  
Ensure the following Python libraries are installed:  
- `numpy`  
- `torch`  
- `torchvision`  
- `matplotlib`  

A trained PyTorch model (`model.pth`) is required for predictions.  

---

## **Installation**  

### **Clone this repository:**  
```sh
git clone <repository_url>
cd EDITAISummerInternship
```  

### **Create a virtual environment and activate it:**  
```sh
python -m venv venv  
source venv/bin/activate  # On macOS/Linux  
venv\Scripts\activate  # On Windows  
```  

### **Install dependencies:**  
```sh
pip install -r requirements.txt  
```  

---

## **Usage**  

### **Prepare the Dataset:**  
- Ensure your dataset is structured with images and corresponding masks.  
- Update the `test_dataset` variable to point to your dataset.  

### **Run the Code:**  
Execute the script to calculate the MAE:  
```sh
python main.py  
```  

### **Output:**  
The script will print the Mean Absolute Error (MAE) between real and predicted NC ratios.  

---

## **Future Improvements**  
- **Enhance Model Accuracy** – Train on a larger dataset to improve segmentation performance.  
- **Automated Threshold Selection** – Implement adaptive thresholding for malignancy classification.  
- **Real-time Processing** – Optimize performance for real-time image analysis.  
- **Additional Visualization Tools** – Introduce heatmaps and histograms for deeper insights.

---

### **Author**  
Rohit Malavathu 
rohitmalavathu@vt.edu 
