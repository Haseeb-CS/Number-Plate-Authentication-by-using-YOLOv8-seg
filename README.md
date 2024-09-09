
Number Plate Validation Project


This code implements a system to detect and validate UK car license plates using a YOLOv8 segmentation model trained on a custom dataset. The code processes an input image to segment the number plate, extracts individual characters, and measures their dimensions to verify their height, width, and spacing. It further checks the font style of the characters through a third-party API and assesses the background color of the plate to ensure compliance with UK standards. The system uses various image processing techniques, such as resizing, sharpening, and morphological operations, to enhance accuracy and reliability in detecting and validating license plates based on predefined criteria.


## Authors

- [@Haseeb-CS](https://github.com/Haseeb-CS)


## Features

- Detection and segmentation of UK car license plates using YOLOv8 segmentation model
- Resizing and preprocessing of input images for optimal analysis
- Extraction of individual characters from the segmented license plate
- Measurement of character dimensions (height, width) in millimeters
- Verification of character spacing to comply with standards
- Font style validation using an external API (whatfontis.com)
- Background color analysis to ensure plate authenticity
- Image sharpening and smoothing for enhanced feature detection
- Dynamic resizing and cropping of images based on aspect ratio
- Error handling for missing or invalid image files

## 🚀 About Me
I'm a Machine Learning Engineer specializing in computer vision, natural language processing (NLP), and image generation. I develop AI solutions that leverage my expertise in these domains to solve complex problems and create innovative applications.


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/Haseeb-CS?tab=repositories)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/shahhaseeb281)



## Installation

Follow these steps to set up and run the license plate detection and validation system:

Clone the Repository: Download or clone the repository to your local machine:

```
git clone https://github.com/Haseeb-CS/License-Plate-Detection.git
cd License-Plate-Detection
```
Install Python: 

Ensure Python 3.x is installed on your system. You can download it from the official Python website.

Set Up a Virtual Environment (Recommended): Create and activate a virtual environment to manage dependencies:

```
python -m venv venv
# Activate on Windows
venv\Scripts\activate
# Activate on macOS/Linux
source venv/bin/activate
```
Install Required Libraries: Install all necessary Python packages using pip:
```
pip install opencv-python
pip install numpy
pip install matplotlib
pip install ultralytics
pip install scikit-learn
pip install python-dotenv
```
Obtain API Key for Font Validation:

Sign up at WhatFontIs to get an API key.
Create a .env file in the project directory and add your API key:
```
WHAT_FONT_IS=your_api_key_here
```
Download YOLOv8 Model Weights: Ensure the YOLOv8 model weights file (best.pt) is available in the project directory or update the path in the code.

Run the Code: Execute the script to start the license plate detection and validation:
```
python script_name.py
```
Troubleshooting:

Verify that all necessary libraries are installed and the correct paths to the image files and YOLO model weights are set.
Ensure that the .env file contains the correct API key.
By following these steps, you will have the license plate detection and validation system set up and running on your machine.