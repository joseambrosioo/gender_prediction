# Gender Classification Using Convolutional Neural Networks (CNN)

This project was proudly presented at the **2024 Kansas Capitol Graduate Research Summit**, earning recognition from the **State of Kansas**, the **Kansas Governor**, policymakers, and **Fort Hays State University** for its significant contribution to research and innovation.

## Project Overview
Developed a **Convolutional Neural Network (CNN)** to classify a person's gender from facial images, achieving an impressive **91% validation accuracy** using a dataset of over **23,000 images**. The CNN model was trained to recognize and distinguish between male and female faces with high precision, and the results were validated against a separate test set.

### Key Features:
- **Deep Learning Architecture**: Utilizes CNN for image recognition, which is highly effective in identifying facial features for gender classification.
- **High Accuracy**: Achieved **91% validation accuracy** on a large dataset, demonstrating the model’s robustness and reliability.
- **Scalability**: The model can be extended to classify other facial attributes or be integrated into larger facial recognition systems.

## Applications
This research has potential applications in:  
- **Demographic Analysis**: Gain insights into population demographics by understanding gender distribution.
- **Targeted Advertising**: Deliver personalized ad content based on user gender classification.
- **Security Enhancements**: Improve surveillance systems by adding gender classification to identity verification processes.
- **Personalized User Experiences**: Tailor services such as online recommendations and customizations based on gender.
- **Medical Diagnostics**: Support healthcare assessments, providing tools to analyze patients' gender in clinical studies.

## Methodology
The CNN model was trained on a large dataset of facial images and utilized the following steps:

### Sample Characteristics
The dataset consists of over **23,000 facial images** annotated with gender labels. These images were sourced from various public datasets, ensuring diversity in terms of ethnicity, age, and lighting conditions, which contributed to the model's high generalization ability.

- **Sample Characteristics**:
  - Number of images: **23,000+**
  - Image dimensions: **200x200 pixels** (resized)
  - Labeling: **Male (0)** and **Female (1)** categories
  - Gender Distribution: **52.3% Male**, **47.7% Female**
  - Age Rage: **0 to 116 years**
  - Preprocessing steps: Normalization (standardized pixel values), augmentation (increased dataset variety), and grayscale conversion (reduced complexity) to improve model robustness.

![13](https://github.com/user-attachments/assets/b9b9e41a-f584-463e-a2c9-5f5919934f88)

*Figure 1. Sample of Images in the Dataset* 

- **Dataset Visualization**:  

![01](https://github.com/user-attachments/assets/67ad342a-48e4-4c19-a6d3-7d719020d45f)

*Figure 2. Distribution of Gender in the Dataset: 52.3% Male, 47.7% Female* 

### Image Preprocessing
To ensure consistent input to the model, the images were split into smaller chunks of 200x200 pixels to improve model performance and reduce computational load.

### CNN Model Architecture
The model follows a **standard CNN architecture**, featuring multiple layers for feature extraction and classification:

1. **Input Layer**: Accepts image data (resized to 200x200 pixels).
2. **Convolutional Layers**: Extract features such as edges, textures, and facial landmarks.
3. **Activation Functions**: Leaky ReLU to introduce non-linearity.
4. **Pooling Layers**: Reduce dimensionality and capture the most important features.
5. **Fully Connected Layers**: Classify images into gender categories based on extracted features.
6. **Output Layer**: A sigmoid activation function for binary classification (Male/Female).

![02](https://github.com/user-attachments/assets/d43482d5-fcab-4f8c-909a-a93fe52104d4)

*Figure 3. CNN Model Architecture* 

**CNN Model Steps**:
- Step 1: Load and preprocess the dataset.
- Step 2: Define and compile the CNN model.
- Step 3: Train the model using the training dataset.
- Step 4: Validate and test the model for accuracy and precision.
- Step 5: Evaluate performance using various metrics such as precision, recall, and F1-score.

![03](https://github.com/user-attachments/assets/b8bed775-ffcd-4adf-b5da-988fb4ef4597)

*Figure 4. CNN Model Steps* 

### Training Process
The model was trained for **15 epochs**, with performance evaluated using a validation set. The training process included tuning hyperparameters such as learning rate, batch size, and the number of layers to optimize performance.

**Training Process Visualization**:  

![04](https://github.com/user-attachments/assets/bbdd0da3-b905-4951-aba3-d4712718017f)

*Figure 5. Graph showing accuracy improvement over epochs.*

![14](https://github.com/user-attachments/assets/00f0091f-0bf3-4baf-b7f0-39c1eeca16e8)

*Figure 6. Training-Accuracy Graph*

![15](https://github.com/user-attachments/assets/72b701de-b1e3-45bd-a789-b2418942116b)

*Figure 7. Training-Loss Graph*

## Test Predictions
The model was evaluated on a separate test set, comparing predicted and actual labels to assess accuracy.

- **Test Results**:
    - **Test Sample 1**:
      - **Actual Gender**: Female
      - **Predicted Gender**: Female  
 
      ![06](https://github.com/user-attachments/assets/fcfb9eee-e4d4-4326-92bd-fa5997ee914a)  

      *Figure 8. Test Sample 1*

    - **Test Sample 2**:
      - **Actual Gender**: Female
      - **Predicted Gender**: Female  

      ![07](https://github.com/user-attachments/assets/6146f90c-f789-4552-9cf1-72649a813789)

      *Figure 9. Test Sample 2*

    - **Test Sample 3**:
      - **Actual Gender**: Male
      - **Predicted Gender**: Male  

      ![08](https://github.com/user-attachments/assets/b2e9e653-c0af-4f6b-a5bc-3273f253282f)

      *Figure 10. Test Sample 3*

    - **Test Sample 4**:
      - **Actual Gender**: Female
      - **Predicted Gender**: Female  

      ![09](https://github.com/user-attachments/assets/aee4455f-f682-457a-b546-105c46cb667c)

      *Figure 11. Test Sample 4*

    - **Test Sample 5**:
      - **Actual Gender**: Female
      - **Predicted Gender**: Female  

      ![10](https://github.com/user-attachments/assets/970408c4-22d2-44b1-a561-4a8e820fddfe)

      *Figure 12. Test Sample 5*

    - **Overall Test Set Accuracy**: **100%**

## Conclusion
This CNN-based gender classification model achieved a high validation accuracy of 91%, demonstrating its potential for real-world applications such as demographic analysis, security, and personalized services. The project highlights the effectiveness of CNNs in handling large image datasets for accurate predictions.

## Code Snippets
Below are key sections of the code used in this project:

1. **Data Preprocessing**:
![11](https://github.com/user-attachments/assets/f3cdf9d6-7e92-4523-bf4b-a603b4cdf833)

*Figure 13. Data Processing Code Snippet*

2. **CNN Model Architecture**:
![12](https://github.com/user-attachments/assets/bd4bd766-520d-4824-ae4d-dc5f8c7200dd)

*Figure 14. CNN Model Architecture Code Snippet*

3. **Model Prediction**
![05](https://github.com/user-attachments/assets/40fbf849-917c-4ab3-91a0-ded2399df663)

*Figure 15. Model Prediction Code Snippet*

## Explore the Repository
Explore the repository to learn more about the methodology, code, and results. Contributions and feedback are welcome!
