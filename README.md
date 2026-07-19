# 😊 DeepFER: Facial Emotion Recognition Using Deep Learning

> A Deep Learning-based Computer Vision project that classifies human facial expressions into seven emotion categories using Convolutional Neural Networks (CNN) and image preprocessing techniques.

# 📌 Project Overview

Facial expressions are one of the most effective ways humans communicate emotions. Automating facial emotion recognition enables machines to better understand human behavior and improve interactions across various applications such as healthcare, customer service, education, surveillance, and human-computer interaction.

This project develops a **Facial Emotion Recognition System** capable of classifying facial expressions into seven different emotions using a **Convolutional Neural Network (CNN)**. The model is trained on thousands of labeled facial images and incorporates preprocessing, data augmentation, and deep learning techniques to achieve robust emotion classification.

---

# 🎯 Problem Statement

Traditional methods of emotion detection often rely on manual observations or surveys, which can be subjective and time-consuming.

The objective of this project is to develop an automated emotion recognition system capable of accurately identifying facial emotions from images using Deep Learning.

The model predicts the following seven emotions:

- 😠 Angry
- 🤢 Disgust
- 😨 Fear
- 😀 Happy
- 😐 Neutral
- 😢 Sad
- 😲 Surprise

---

# 🚀 Project Objectives

- Develop an end-to-end Facial Emotion Recognition system.
- Build a robust CNN model for image classification.
- Perform image preprocessing and data augmentation.
- Train and evaluate the deep learning model.
- Save the trained model for future inference.
- Explore Transfer Learning using ResNet50V2.
- Analyze model performance using multiple evaluation metrics.

---

# 📂 Dataset

The dataset consists of thousands of labeled facial expression images categorized into seven emotion classes.

## Emotion Classes

- Angry
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprise

## Dataset Structure

```
images/

├── train/

│ ├── angry/

│ ├── disgust/

│ ├── fear/

│ ├── happy/

│ ├── neutral/

│ ├── sad/

│ └── surprise/

│

└── validation/

├── angry/

├── disgust/

├── fear/

├── happy/

├── neutral/

├── sad/

└── surprise/
```

The dataset is organized into separate **training** and **validation** folders, allowing TensorFlow's `ImageDataGenerator` to automatically assign labels based on directory names.

---

# 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Google Colab

---

# 🔄 Project Workflow

```
Dataset Collection
        │
        ▼
Image Preprocessing
        │
        ▼
Data Augmentation
        │
        ▼
CNN Model Building
        │
        ▼
Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Performance Visualization
        │
        ▼
Save Trained Model
        │
        ▼
Transfer Learning (ResNet50V2)
```

---

# 🧹 Data Preprocessing

The following preprocessing techniques were applied before model training:

- Image normalization
- Image resizing
- Grayscale conversion (for CNN model)
- Batch generation using ImageDataGenerator
- Automatic label generation from directory structure

---

# 🔄 Data Augmentation

To improve model generalization and reduce overfitting, multiple augmentation techniques were used:

- Random Rotation
- Horizontal Flip
- Zoom
- Width Shift
- Height Shift
- Rescaling

Data augmentation increases dataset diversity and improves model robustness under different lighting conditions and facial orientations.

---

# 🧠 CNN Model Architecture

A custom Convolutional Neural Network (CNN) was developed for facial emotion classification.

The architecture consists of:

- Convolution Layers
- ReLU Activation
- Batch Normalization
- MaxPooling Layers
- Dropout Layers
- Fully Connected Dense Layers
- Softmax Output Layer

The output layer predicts one of the seven facial emotion classes.

---

# ⚙️ Model Training

The CNN model was trained using:

- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Batch Size: 64
- Epochs: 30–42 (depending on training configuration)

Callbacks used during training:

- ModelCheckpoint
- ReduceLROnPlateau
- EarlyStopping (recommended)

These callbacks improve convergence, reduce overfitting, and automatically save the best-performing model.

---

# 📊 Model Evaluation

The model was evaluated using multiple classification metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- Validation Accuracy
- Validation Loss

Training history was visualized using:

- Accuracy vs Epoch
- Loss vs Epoch

These plots help analyze learning behavior and detect overfitting or underfitting.

---

# 💾 Model Saving

After successful training, the trained CNN model is saved for future inference.

```
cnn_model_new_.h5
```

The saved model can later be loaded for image prediction or real-time emotion recognition.

---

# 🚀 Transfer Learning

The project also explores **Transfer Learning using ResNet50V2**.

Transfer Learning enables the model to leverage knowledge learned from large-scale image datasets, improving feature extraction and potentially enhancing classification performance while reducing training time.

---

# 📈 Applications

Facial Emotion Recognition has numerous practical applications, including:

- Human-Computer Interaction
- Mental Health Monitoring
- Smart Surveillance Systems
- Customer Experience Analysis
- Education Technology
- Driver Fatigue Detection
- Healthcare Monitoring
- Virtual Assistants
- Robotics

---

# 📁 Project Structure

```
DeepFER/

│

├── Face Emotion Recognition Dataset/

│ ├── train/

│ └── validation/

│

├── notebooks/

│ └── facial_emotion_recognition.ipynb

│

├── saved_model/

│ └── cnn_model_new_.h5

│

├── images/

│ └── sample_predictions.png

│

├── requirements.txt

│

├── README.md

│

└── LICENSE
```

---

# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/DeepFER.git
```

Navigate into the project

```bash
cd DeepFER
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Project

Open the notebook in Google Colab or Jupyter Notebook.

Execute the cells sequentially:

1. Load Dataset
2. Preprocess Images
3. Train CNN Model
4. Evaluate Performance
5. Save Model
6. Test Predictions

---

# 📌 Future Improvements

- Improve performance using EfficientNet or MobileNetV3
- Deploy using Streamlit or Flask
- Real-time webcam emotion detection
- Hyperparameter tuning
- Larger and more diverse datasets
- Model optimization for edge devices
- Explainability using Grad-CAM

---

# 🎓 Key Learnings

Through this project, I gained practical experience in:

- Computer Vision
- Deep Learning
- CNN Architecture Design
- Image Preprocessing
- Data Augmentation
- Transfer Learning
- Model Evaluation
- TensorFlow & Keras
- OpenCV
- Performance Optimization

---

# 📚 Skills Demonstrated

- Python Programming
- Deep Learning
- Computer Vision
- CNN
- TensorFlow
- Keras
- OpenCV
- Data Preprocessing
- Image Classification
- Model Evaluation
- Transfer Learning
- Data Visualization

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

Feel free to fork the repository, create a feature branch, and submit a pull request.

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Sarathraj R**

Data Scientist | Data Analyst | Machine Learning Enthusiast

LinkedIn: https://www.linkedin.com/in/sarathraj-r-ds/


---

⭐ If you found this project useful, consider giving the repository a **Star**.
