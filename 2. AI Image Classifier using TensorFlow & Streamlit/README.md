# AI Image Classifier using TensorFlow \& Streamlit

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

![Libraries](https://img.shields.io/badge/Libraries-Tensorflow%2C%20Streamlit%2C%20Numpy-orange.svg)

## 📝 Overview

This project presents an interactive web application for **image classification** using a deep-learnning model. The app, built with [Streamlit](https://streamlit.io/) and [TensorFlow / Keras](https://keras.io/), allows users to upload an image and receive AI-powered predictions about its content along with their confidence scores. The core of the project is the `MobileNetV2` model, a convolutional neural network (CNN) trained on the `ImageNet` dataset.

## ✨ Features

* **Deep Learning Classification:** Utilizes the `MobileNetV2` model from TensorFlow/Keras to recognize over 1,000 classes out of the box.
* **Interactive Web UI:** A clean and user-friendly single-page interface created with Streamlit, featuring a file uploader for easy image submission.
* **Real-Time Predictions:** Classifies images instantly upon user request by clicking a button.
* **Top-3 Predictions:** Displays the three most likely labels for the uploaded image, providing a more comprehensive analysis.
* **Efficient Model Loading:** Implements Streamlit's caching (`@st.cache_resource`) to load the model into memory only once, ensuring fast performance on subsequent runs.
* **Image Preprocessing:** Automatically preprocesses uploaded images—resizing and formatting them into vectors that the model can understand.

## 🛠️ Installation

Install the required dependencies in your Python environment:

```bash
pip install tensorflow streamlit opencv-python numpy
```

> The app is designed to run locally; GPU support is not strictly required due to the efficient MobileNetV2 model.

## 🚀 Usage

1. **Save the code** from the notebook as a Python file (e.g., `app.py`).
2. **Run the application** from your terminal by executing: `streamlit run app.py`.
3. **Open the URL** provided by Streamlit (usually `http://localhost:8501`) in your web browser.
4. **Upload an image** using the file uploader (supports `.jpg` and `.png` formats).
5. **Click the "Classify Image" button** to process the image and view the AI's predictions.

### Example

```
[Streamlit page loads]
Upload an image and let AI tell you what it is
[User uploads a picture of a cat]

Click "Classify Image"

AI Predictions
• Egyptian_cat: 97.5%
• Tabby: 2.1%
• Lynx: 0.3%
```


## 🧩 Model Used

- **Image Classification:** [`MobileNetV2`](https://www.tensorflow.org/api_docs/python/tf/keras/applications/mobilenet_v2/MobileNetV2) (pre-trained on the `imagenet` dataset)


## 📦 Dependencies

- `Python 3.x`
- `tensorflow`
- `streamlit`
- `opencv-python`
- `numpy`

> **Tip:** For best performance, run locally. MobileNetV2 is lightweight and suitable for CPU inference.