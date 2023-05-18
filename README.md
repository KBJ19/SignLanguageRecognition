# Sign Language Recognition with Mediapipe and Keras
This project uses the Mediapipe library to detect hand gestures in real-time video feed, and Keras with LSTM to train a model to recognize these gestures. The project involves two main parts: data collection and model training.

# Data Collection
The collect_data.py script can be used to collect training data. It reads video frames from a camera or a saved video, and uses Mediapipe to detect and extract hand landmarks in each frame. The landmarks are saved to disk as NumPy arrays, which can be used to train the model. The data is organized into directories based on the type of gesture and the sequence number.

# Model Training
The train_model.py script loads the saved NumPy arrays and trains a Keras model with LSTM layers to recognize the gestures. The model is saved to disk as a JSON file and a weights file, which can be loaded and used for prediction.

# Usage
To collect data, run collect_data.py with appropriate command line arguments. Run the data.py file. To train the model, run train_model.py. The script will automatically load all the saved data and train the model. The training progress is logged to TensorBoard, and the final model is saved to model.json and model.h5 files.

To use the trained model for prediction, load the saved model and weights files using Keras, and use the predict() method on a new set of hand landmarks extracted from a video feed or an image..

# Requirements
Python 3.6+ 
OpenCV 
Mediapipe 
Keras
NumPy
TensorBoard

Implementation:

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/7de586df-8da9-49be-9728-9152ed5a7f4a)

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/5183e825-e2c0-4e9f-999e-1f546b44bb0f)

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/9adb1f54-0bb6-4b63-bc88-be5f83ae526c) 

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/895dab52-6d99-4ac1-9186-cbff242d6e18)  ![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/73251c2a-48d2-4342-bbcd-323814eb218f)

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/76a39d01-8327-4784-8df4-ee9589673be4)

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/b6cd8352-3494-4717-9814-78f902c1610a)

Output:

![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/d95c4924-94fe-4a97-b781-5fd7c03f6f41)  ![image](https://github.com/KBJ19/SignLanguageRecognition/assets/87027526/925993c5-9488-4f94-b6ff-af91372ba452)








