# Video Classification Pipeline 🎥🤖

This notebook demonstrates a complete pipeline for **video classification** using a combination of **Convolutional Neural Networks (CNNs)** and **Recurrent Neural Networks (RNNs)**. The goal is to classify actions in videos by capturing both spatial and temporal features.

---

## Process Flow 🚀

1. **Data Preparation**:
   - Load and preprocess video datasets (e.g., UCF101 dataset).
   - Extract frames from videos for spatial analysis.
   
2. **Feature Extraction with CNNs**:
   - Utilized the Xception CNN due to it's computational efficiency to extract spatial features from individual frames.
   - These features capture the objects and actions within each frame.

3. **Temporal Modeling with RNNs**:
   - Feed extracted features into an RNN to model temporal relationships across frames.
   - This step helps the model understand how actions evolve over time (e.g., walking vs. running).
   - RNN developed by utilizing the keras API , below is the architecture designed:
![gru_model_architecture](https://github.com/user-attachments/assets/8dfb9d4f-4ca6-4b78-a55b-275488cb27a8)


4. **Model Training**:
   - Train the combined CNN-RNN architecture on labeled video data.
   - Optimize for accuracy in predicting video actions.

5. **Evaluation and Inference**:
   - Evaluate the trained model using metrics like accuracy and loss.
   - Use the model to predict actions in new video inputs.

---

## Key Highlights ✨

- **Combining CNNs and RNNs**: 
  - CNNs capture spatial details from video frames.
  - RNNs analyze the sequence of features to model temporal dynamics.
  
- **Preprocessing**:
  - Frames are extracted from videos and normalized for input to the CNN.
  
- **Output**:
  - The model outputs the predicted action label for each video (e.g., "jumping", "running").

---

## How to Use 🛠️

1. **Setup Environment**:
   - Install necessary dependencies from the notebook.
   - Ensure you have access to a video dataset like UCF101.

2. **Run the Notebook**:
   - Follow the notebook's step-by-step instructions for data preprocessing, training, and evaluation.

3. **Test Your Model**:
   - Use the trained model to classify actions in new videos.

