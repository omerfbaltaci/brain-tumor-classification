# 🧠 Brain Tumor Classification Using Convolutional Neural Networks

## 🚀 Overview
In the realm of medical imaging, early and accurate diagnosis is paramount. This project harnesses the power of Convolutional Neural Networks (CNNs) to classify MRI images of brain tumors. By automating the classification process, we aim to provide a supportive tool for healthcare professionals in their diagnostic journey.

## 📊 Dataset
This project utilizes the **Brain Tumor Classification MRI** dataset, which contains a rich collection of MRI images categorized into four classes:
- **Glioma Tumor**
- **Meningioma Tumor**
- **Pituitary Tumor**
- **No Tumor**

The images are organized into training and testing directories, ensuring an efficient workflow for model training and evaluation.

![MRI Sample Image](https://github.com/user-attachments/assets/ae073965-bda8-4431-9787-a6df467f413b)

## 🛠️ Project Structure
The project is neatly organized into the following components:
- **Data Directory**: Contains categorized MRI images.
- **Jupyter Notebook**: The heart of our project, where we perform data preprocessing, model training, and evaluation.

## 🧪 Methodology

### 1. Data Preparation
We kick off the project by importing necessary libraries like **NumPy**, **Pandas**, **Keras**, and **OpenCV**. The images are then loaded and resized to a uniform dimension of **150x150 pixels** to maintain consistency across the dataset.

### 2. Label Encoding
Each tumor category is transformed into a numerical format, allowing the CNN to interpret the labels effectively.

### 3. Splitting the Dataset
The dataset is divided into training and testing subsets, ensuring our model can be evaluated against unseen data, which is crucial for assessing its real-world performance.

### 4. CNN Model Architecture
The architecture of our CNN model includes:
- Multiple **Convolutional Layers**: These layers automatically extract features from the images.
- **MaxPooling Layers**: These reduce dimensionality while preserving essential features.
- **Dropout Layers**: These layers mitigate overfitting by randomly dropping units during training.
- A fully connected layer at the end for final classification.

### 5. Training the Model
Using the **Adam optimizer** and **categorical crossentropy loss**, the model is trained on the dataset with validation to monitor its performance.

## 📈 Results
The performance of the model is evaluated through accuracy metrics, with training and validation accuracy and loss visualized through plots.

### Training vs Validation Accuracy
![Accuracy Plot](https://www.kaggleusercontent.com/kf/198930340/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..DtcSjEg1G6WZPld-hmhZ8g.mTro7oBnevPjCEUdgcebhXTER2AV40y49tpD5QGLGEyKBxYq3sDCylGSQw6gmL9WbAbgmpt3-PNfeZIpA17H1RoD8m1N_Bb3J3KT85QK4uzSb6tyZLfhE60lnP2zIWsCXlRm_fpnmssgiU2ndGRHtMYOXqy1LOJQavF52lw5-yewPIZvQR3ggjYtzT_NJe1hklKilvLhWVS4FRsR6fKkEUECrtj6pImwuV1ryZ2lIC27HHPYtCcybf6gtKM9TkDmLfXoRQCBSWdchNeJoQkTv-yg_4bliVbwdwc9C5o7y3OANXsnWNirLazn_olEC9IXqQquAUsY3DHxdWX5J-1HsPekz4D3EbR6ar8Ic4r40NGHXr1fUMTixZtrPq4BATpbIBrwFxas3_QwlmZaoiiniYCSTkYr7pBUg70MGN4a68SXHm0qDhu8IBUJrVoeIGOf65lns5W8sMJbfRs94OIXF7gO-4SiDYgswwS6Hn4Hti52fYgIbtgZeGB9NrzJh9334Yczb5AwxxP95xGjJL0in3zGFz6hHISBrfZDDK3Z4QjjfU-VGy6wf2JrN_gmD8NnwFA13FjJ_abQjxYukAEsfxEqjTu53PdJZ-5qiBOBvFvM3iA6kIaDeMbS0Azi6OfBrTg9RgOJcEg2Uo1U30be0Q._K41uG7dvqVShGH8AaF4AA/__results___files/__results___21_0.png)

### Training vs Validation Loss
![Loss Plot](https://www.kaggleusercontent.com/kf/198930340/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..DtcSjEg1G6WZPld-hmhZ8g.mTro7oBnevPjCEUdgcebhXTER2AV40y49tpD5QGLGEyKBxYq3sDCylGSQw6gmL9WbAbgmpt3-PNfeZIpA17H1RoD8m1N_Bb3J3KT85QK4uzSb6tyZLfhE60lnP2zIWsCXlRm_fpnmssgiU2ndGRHtMYOXqy1LOJQavF52lw5-yewPIZvQR3ggjYtzT_NJe1hklKilvLhWVS4FRsR6fKkEUECrtj6pImwuV1ryZ2lIC27HHPYtCcybf6gtKM9TkDmLfXoRQCBSWdchNeJoQkTv-yg_4bliVbwdwc9C5o7y3OANXsnWNirLazn_olEC9IXqQquAUsY3DHxdWX5J-1HsPekz4D3EbR6ar8Ic4r40NGHXr1fUMTixZtrPq4BATpbIBrwFxas3_QwlmZaoiiniYCSTkYr7pBUg70MGN4a68SXHm0qDhu8IBUJrVoeIGOf65lns5W8sMJbfRs94OIXF7gO-4SiDYgswwS6Hn4Hti52fYgIbtgZeGB9NrzJh9334Yczb5AwxxP95xGjJL0in3zGFz6hHISBrfZDDK3Z4QjjfU-VGy6wf2JrN_gmD8NnwFA13FjJ_abQjxYukAEsfxEqjTu53PdJZ-5qiBOBvFvM3iA6kIaDeMbS0Azi6OfBrTg9RgOJcEg2Uo1U30be0Q._K41uG7dvqVShGH8AaF4AA/__results___files/__results___23_0.png)

## 🎉 Conclusion
Our CNN model demonstrates the potential of deep learning in the classification of brain tumors from MRI scans. The promising results pave the way for further exploration and improvement in automated medical diagnostics.

## 📝 License
This project is licensed under the [Apache License 2.0](https://opensource.org/licenses/Apache-2.0). Feel free to use, modify, and share it according to the terms outlined in the license.
Also inspired from CodersArts' YouTube channel, [https://www.youtube.com/watch?v=juJYmc4vrWU&ab_channel=CodersArts](https://www.youtube.com/@CodersArts/videos)
