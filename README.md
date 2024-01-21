# car-damage-assessment
The Car Insurance Image Analysis App is a powerful tool designed for the insurance sector, specifically tailored to streamline and enhance the assessment process of broken car images. This application integrates cutting-edge artificial intelligence techniques across four key modules, providing insurers with a comprehensive solution for image detection, damage severity assessment, damaged part detection, and repair cost estimations.
## Modules
### 1. AI Image Detection
Utilizing advanced image recognition algorithms, the app distinguishes between fake and real car images.
### 2. Damage Severity Assessment
The Damage Severity Assessment module employs deep learning models to analyze the extent of damage in the submitted images. 
### 3. Damaged Part Detection
By leveraging sophisticated computer vision techniques, the app identifies specific damaged parts within the car images. This module enhances the accuracy of the assessment process.

### 4. Repair Cost Estimations
The Repair Cost Estimations module utilizes machine learning algorithms to predict the repair costs associated with the identified damages. 
## Installation
1. clone the github repository 
```bash
git clone https://github.com/Asma-Ab/car-damage-assessment.git
```
2. install the requirements 
```bash
pip install requirements.txt
```
3. run the app
```bash
streamlit run app.py
```
## Models and algorithms 
Each module in this app is tested with multiple models :
##### AI Image Detection
for this part , we used  stable diffusion algorithm  a text-to-image latent diffusion model in order to built the fake images dataset .
- **Convolutional Neural Network (CNN):** Trained from scratch to recognize AI-generated images.
- **Inception V3:** Utilizing the AIData Kaggle dataset to enhance performance.
##### image severity classification
This classification model allows us to categorize car damages into varying levels, ranging from minor scratches and dents to more severe structural impairments.We compared these 3 models below 
- **ResNet**
- **4D model**
- **EfficientNet**
##### damaged parts detection
In the identification of damaged parts, our algorithms undergo training with the Car Damage COCO Dataset. Utilizing YOLOv8 for object detection, along with Mask RCNN and an extra model trained using Roboflow, we seamlessly integrate these models into our user interface.
- **yolov8**
- **roboflow**
