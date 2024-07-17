# Brest-Cancer-Prediction-Using-Neural-Network
This project demonstrates how to build a neural network for breast cancer classification using TensorFlow and Keras. The dataset is loaded from sklearn, preprocessed, and used to train a sequential model. The model's performance is evaluated, and a prediction system is demonstrated. 

## Steps

1. **Data Collection and Preprocessing:**
   - Load the breast cancer dataset from sklearn.datasets.
   - Create a pandas DataFrame and explore the data.
   - Check for missing values and analyze statistical measures.
   - Separate features (X) and target (Y).
   - Split the data into training and testing sets.
   - Standardize the features using StandardScaler.

2. **Building the Neural Network:**
   - Define a sequential Keras model with layers:
     - Flatten layer to convert input to a 1D array.
     - Dense layer with 20 neurons and ReLU activation.
     - Dense layer with 10 neurons and sigmoid activation.
     - Output layer with 2 neurons (for binary classification) and sigmoid activation.
   - Compile the model with Adam optimizer, sparse categorical crossentropy loss, and accuracy metric.

3. **Training the Neural Network:**
   - Train the model on the standardized training data with validation split.
   - Visualize training and validation accuracy and loss using matplotlib.

4. **Evaluating the Model:**
   - Evaluate the model on the standardized test data.
   - Print the accuracy.

5. **Prediction:**
   - Define a sample input data point.
   - Preprocess the input (reshape, standardize).
   - Predict the class using the trained model.
   - Print the predicted class label (Malignant or Benign).

## Requirements

- pandas
- numpy
- matplotlib
- sklearn
- tensorflow

## How to Run

1. Install the required libraries.
2. Run the notebook cells sequentially.
