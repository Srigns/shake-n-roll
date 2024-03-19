## Facial KeyPoint Estimation Model

This folder contains the code for a facial keypoint estimation model based on the ResNet50 architecture. The model is trained to detect two key facial landmarks: the top of the head and the chin. These keypoints can be used to control various applications, such as games or virtual reality environments.

## Training the Model

To train the model, follow these steps:

1. **Install Dependencies**:
   <br />
   ```
   pip install opencv-python tensorflow numpy matplotlib
   ```

2. **Download the MPII Dataset**:
   <br />
   * Download the processed mpii dataset here : `https://www.kaggle.com/datasets/binarybrainiac/pose-data-mpii`.
   * Extract the dataset and place it in the data/ directory.

3. **Train the Model**:
   <br />
   * Use the `Training_Model.ipynb` Jupyter notebook to train the ResNet50 model with imagenet weights on the
     preprocessed data.
