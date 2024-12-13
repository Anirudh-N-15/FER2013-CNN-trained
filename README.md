# Facial Expression Recognition using CNNs

## Description
This project aims to build a Convolutional Neural Network (CNN) model that classifies facial expressions (e.g., happy, sad, neutral) from images. Such a system could help enhance feedback mechanisms in campus activities and other interactive settings.

## Dataset
The primary dataset used is the **FER 2013 Dataset (Facial Expression Recognition)**, which contains labeled images for training and testing the model.

---

## Documentation Outline

### 1. Problem Statement
Facial expressions convey significant emotional and social information. Recognizing these expressions from images can provide valuable insights into user emotions, especially in campus activities, where feedback mechanisms can benefit from understanding the participants' reactions.It can also help in detecting and monitoring the mental health of students inside the campus and provide help if necessary.

### 2. Approach
The methodology involves the following steps:

1. **Data Collection:**
   - Used the FER 2013 dataset containing labeled facial expression images.

2. **Data Preprocessing:**
   - Resize images to a uniform size (e.g., 48x48 pixels).
   - Normalize pixel values for consistent input to the CNN (Divided by 255 to get value between 0 and 1).
   - Split data into training and  validation data (80% and 20%).

3. **Model Architecture:**
   - Designed a sequential CNN model with layers such as:
     - Convolutional layers for feature extraction.
     - Pooling layers to reduce spatial dimensions.
     - Fully connected layers for classification.
     - Learning rate scheduler and optimizer
     - Also used Rectified Linear Unit activation function to introduce non-linearity into the model.
   - Apply techniques like batch normalization and dropout to improve generalization.

4. **Training:**
   - Use categorical cross-entropy loss as the objective function.
   - Optimize the model using Adam algorithm.
   - Trained 150 epochs while monitoring performance on the validation set.

5. **Evaluation:**
   - Assess the model's performance on the test set using metrics like accuracy, precision, recall, and F1-score.
   - Visualize confusion matrices to analyze classification performance.

6. **Deployment:**
   - Package the model for deployment in an application or API for real-time expression recognition.

### 3. Results
Present the following:
- Performance metrics (e.g., accuracy, F1-score) on the test dataset.
- Visualizations:
  - Training and validation accuracy/loss curves.
  - Confusion matrix to display classification results.
- Observations:
  - Insights into model strengths and weaknesses.

### 4. Challenges
Document the obstacles encountered during the development process, such as:
- Handling imbalanced datasets.
- Reducing overfitting in the model.
- Improving generalization on unseen data.
- Computational limitations during training.

---

