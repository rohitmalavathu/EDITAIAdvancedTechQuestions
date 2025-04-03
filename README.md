Project: EDITAISummerInternShip
This project contains Python code for analyzing and processing image datasets, specifically focusing on calculating Nucleus-to-Cytoplasm (NC) ratios and evaluating model performance using Mean Absolute Error (MAE).

Table of Contents
Overview
Requirements
Installation
Usage
Functions
nc_ratio
MAE_and_Results
Model
License
Overview
This project includes:

A function to calculate the Nucleus-to-Cytoplasm (NC) ratio from image masks.
A function to compute the Mean Absolute Error (MAE) between real and predicted NC ratios.
A PyTorch-based model for image segmentation, which predicts masks for input images.
The code is designed to work with datasets containing images and their corresponding masks.

Requirements
The following Python libraries are required:

numpy
torch
torchvision
matplotlib
Additionally, ensure you have a trained PyTorch model saved as model.pth.

Installation
Clone this repository:

Create a virtual environment and activate it:

Install the required dependencies:

Usage
Prepare the Dataset:

Ensure your dataset is structured with images and corresponding masks.
Update the test_dataset variable in the code to point to your dataset.
Run the Code:

Execute the script to calculate the MAE:
Output:

The script will print the Mean Absolute Error (MAE) between real and predicted NC ratios.
Functions
nc_ratio(image)
Calculates the Nucleus-to-Cytoplasm (NC) ratio for a given image mask.

Parameters:

image: A NumPy array representing the mask.
Returns:

The NC ratio as a float.
MAE_and_Results(dataset)
Computes the Mean Absolute Error (MAE) between real and predicted NC ratios for a dataset.

Parameters:

dataset: A dataset containing images and their corresponding masks.
Returns:

The MAE as a float.
Model
The code uses a PyTorch model for image segmentation. Ensure you have a trained model saved as model.pth in the project directory. The model is loaded using:

License
This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to modify this README.md file to suit your specific project details! Let me know if you need further assistance.
