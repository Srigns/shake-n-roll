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
   * Extract the dataset and place it in the `data/` directory.

3. **Train the Model**:
   <br />
   * Use the `Training_Model.ipynb` Jupyter notebook to train the ResNet50 model with imagenet weights on the
     preprocessed data.

<br/>

## Using the Trained Model

To use the trained model in your application, follow these steps:

1. **Download the Model**:
   <br />
   * Download the model if you don't want to train your own from here : `https://www.kaggle.com/models/binarybrainiac/model`.
   * Put the `model.h5` in the exported_model/ directory.

2. **Run the Model**:
   <br />
   * Use the `Run_Model.ipynb` Jupyter notebook to run the `exported_model/model.h5` model.
     

<br/>

## Converting h5 to tflite

To make the model work faster, I converted the model to tflite, and to convert the model from h5 to tflite, follow these steps:

1. **Download the Model**:
   <br />
   * Download the model if you don't want to train your own from here : `https://www.kaggle.com/models/binarybrainiac/model`.
   * Put the `model.h5` in the `exported_model/` directory.

2. **Convert the h5**:
   <br />
   * Use the `Convert.ipynb` Jupyter notebook to Convert the `exported_model/model.h5` to `exported_model/model.tflite`.


<br/>

## Using the model with the game

To use the trained model for your game, follow these steps:<br/>
(Double check if the `model.tflite` is in `exported_model/` directory or not. if not convert the model)

1. **Run the Model**:
   <br />
   * Use the `Start_Model.ipynb` Jupyter notebook to run the `exported_model/model.tflite` model.
   * then the data will be sent through `127.0.0.1` in `5052` port.



