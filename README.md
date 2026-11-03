# 🌍 Disaster Prediction using CNN

A Deep Learning project that classifies natural disasters using **Convolutional Neural Networks (CNN)**.  
The model is trained to identify different types of disasters from images such as Cyclone, Flood, Wildfire, and Earthquake.

---

## 🚀 Features

- 🌪️ Multi-class classification:
  - Cyclone
  - Flood
  - Wildfire
  - Earthquake  
- 🧠 CNN-based deep learning model  
- 🖼️ Image preprocessing and augmentation  
- 📊 Model training and evaluation  
- ⚡ Accurate prediction on real-world dataset  

---

## 🧠 Tech Stack

- **Language:** Python  
- **Libraries:** TensorFlow, Keras, NumPy, Matplotlib  
- **Techniques:** CNN, ImageDataGenerator  
- **Platform:** Google Colab  

---

## ⚙️ How It Works

1. Load and organize dataset into training and testing sets  
2. Preprocess images (resizing, normalization)  
3. Apply data augmentation  
4. Train CNN model  
5. Evaluate model performance  
6. Predict disaster category from new images  

---

## 🏗️ Model Architecture

- Input: 128 × 128 × 3 RGB image (pixel values scaled to 0–1)
- Conv2D (32, 3×3, ReLU) → MaxPooling (2×2)
- Conv2D (64, 3×3, ReLU) → MaxPooling (2×2)
- Conv2D (128, 3×3, ReLU) → MaxPooling (2×2)
- Flatten → Dense (128, ReLU) → Dropout (0.5) → Dense (4, Softmax)
- Loss: categorical cross-entropy · Optimizer: Adam (lr = 0.001)
- About 3.3M trainable parameters

## 📁 Project Structure

```
cnn-dis/
├── app.py            # Streamlit app: upload an image and get a prediction
├── model.h5          # Trained CNN model
├── requirements.txt
└── runtime.txt
```

---

## ▶️ Installation

```bash
git clone https://github.com/pujithravi/cnn-dis
cd cnn-dis
pip install -r requirements.txt
streamlit run app.py
```

Upload a JPG/PNG image and the app predicts the disaster type.


---

## 📊 Results

- Achieved accurate classification across 4 disaster classes  
- Model trained on real-world dataset  
- Effective in distinguishing visually similar disaster images  

---

## 📈 Future Improvements

- 🔁 Use Transfer Learning (ResNet, VGG16)  
- 📊 Improve dataset size and diversity  
- 🎯 Show prediction confidence and a confusion matrix  
- ⚡ Optimize model performance  

---

## 👨‍💻 Author

**Ravi pujith**  
- GitHub:https://github.com/pujithravi

---

## ⭐ Support

If you found this project useful, give it a ⭐ on GitHub!
