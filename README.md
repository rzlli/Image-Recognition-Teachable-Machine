# Image Recognition Task - Teachable Machine & Google Colab
## Cooperative Training Program - Smart Methods

This repository contains the complete solution for the Image Recognition task. The objective is to train a custom image classification model (Cats vs. Dogs) using Google's Teachable Machine, export the trained Keras model, and deploy it using a Python script inside Google Colab to predict new input images.

---

##  Detailed Project Steps

### Step 1: Model Training & Verification (Teachable Machine)
* Platform Used: Google's Teachable Machine.
* Classes Trained: 
  * Class 1: Cats 
  * Class 2: Dogs 
* Initial Testing: Uploaded a dataset of images to train the model and verified the live training performance directly on the platform. A screenshot of this step is documented below.

### Step 2: Model Exportation
* Format: Exported the trained model in TensorFlow -> Keras format.
* Downloaded Files: 
  * Keras_model[1].h5: Contains the weights and architecture of the trained model.
  * labels[1].txt: Contains the class names indexed for the predictions.

### Step 3: Local Deployment & Testing (Google Colab)
* Environment: Setup a Python environment inside Google Colab.
* Execution Workflow:
  1. Uploaded the exported model files (`Keras_model[1].h5` and `labels[1].txt`) and the test cat image (`images (23).jfif`).
  2. Imported the required libraries (`tensorflow`, PIL, and `numpy`).
  3. Loaded the model and processed the input image using the inference script.
  4. The model accurately predicted and printed the output label indicating the class with high confidence.

---

##  Repository Structure

* `Image_Recognition_Notebook.ipynb`: The final Google Colab notebook containing the Python script to load the model and perform inference.
* `Keras_model[1].h5`: The exported trained Keras model weights.
* `labels[1].txt`: The index mapping file for the output labels (Cat and Dog).
* `images (23).jfif`: The input cat image used for testing the prediction inside Google Colab.
* `teachable_machine_screenshot.png`: A screenshot showcasing the model training and prediction output within Google's Teachable Machine platform.
* `colab_prediction_screenshot.png`: A screenshot capturing the Google Colab workspace, showcasing the running code and the final prediction output.
