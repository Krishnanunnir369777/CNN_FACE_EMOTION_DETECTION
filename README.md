# Facial Expression Recognition with CNN  
## Problem Statement  
The goal of this project is to classify facial expressions from images to enhance feedback mechanisms during campus activities. By understanding and categorizing emotions, this solution could contribute to real-time feedback collection and improve engagement strategies.  

## Solution
I build a model using Convolutional Neural Network , it can claasify facial expressions from images and also using OpenCV i connected model with that so it will show the emotion on the detected face.
We can implement this on the cameras at the exit of our institute event venue, by this the model can detect the emotion of the participants.Also we can upload images of the event by this also our model can detect the emotion.

I created a website for this project,through this users can upload their images and detect the emotion on that You can see the website for this project using this link <a href="https://krishnanunnir369777.github.io/CNN_website.github.io/">Facial Expression Recognition  Website</a>

## Dataset
The project uses the **FER 2013 Dataset** (Facial Expression Recognition), which contains grayscale 48x48 pixel facial images categorized into seven emotions:  
https://www.kaggle.com/datasets/nicolejyt/facialexpressionrecognition
- Anger  
- Disgust  
- Fear  
- Happiness  
- Sadness  
- Surprise  
- Neutral

  Additional preprocessing and augmentation were applied to balance the dataset and improve model performance.  

## Approach 
The project followed these key steps:  
1. **Data Exploration and Visualization**  
   - Inspected emotion distribution and visualized samples from the dataset.  
   - Balanced the dataset using Random Over Sampling to address class imbalance.  

2. **Data Preprocessing**  
   - Normalized pixel values to a [0, 1] range.  
   - Reshaped images into a 4D tensor for compatibility with CNN.  
   - One-hot encoded the emotion labels.  

3. **Model Development**  
   - Designed a **Convolutional Neural Network (CNN)** with multiple convolutional, pooling, and dropout layers.  
   - Used **ReLU activation** for non-linearity and **Batch Normalization** for faster convergence.  
   - Applied **Softmax activation** in the final layer to output probabilities for each emotion class.  

4. **Evaluation and Metrics**  
   - Evaluated the model using **Accuracy** and **F1-score**.  
   - Visualized the performance using confusion matrices and examples of correctly and incorrectly classified images.  

## Results  
- **Accuracy**: Achieved an accuracy of 81.07% on the test dataset.  
- **F1-score**: Computed per-class and overall F1-scores to ensure balanced performance.  
- **Visualizations**:  
   - Confusion Matrix: Displays the prediction performance across all emotion classes.  
   - Sample Outputs: Examples of correctly classified and misclassified images with their true and predicted labels.
## Model Architecture  
The CNN architecture consists of:  
- **Convolutional Layers** for feature extraction.  
- **Max Pooling** layers for down-sampling.  
- **Dropout Layers** for regularization.  
- **Dense Layers** for final classification.  

## Challenges  
- **Class Imbalance**: The original dataset had imbalanced emotion classes, resolved through oversampling.  
- **Overfitting**: Mitigated by adding dropout layers and data augmentation techniques.  
- **Computational Cost**: Training a deep model required significant computational resources; optimized hyperparameters to reduce training time.  


![Screenshot 2024-12-12 164905](https://github.com/user-attachments/assets/093e21ca-8901-4b81-88af-d115a6f9a2ca)
