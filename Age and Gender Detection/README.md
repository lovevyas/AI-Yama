# 👹 AI-Yama: The All-Seeing Face Analyst

> *"Chitragupta records the deeds, but Yama sees the soul. Just by glancing at a face, AI-Yama reveals the truths of Age and Gender hidden within."*

![Project Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-red)

---

## 📜 The Legend (Introduction)
In mythology, Yama is the impartial judge who knows the details of every living being. Inspired by this omniscience, **AI-Yama** is a deep learning system designed to extract biological attributes from a single facial image.

While it cannot judge your karma, it **can** judge your biometrics with high accuracy. Whether through a static photo or a live video feed, AI-Yama analyzes facial features to instantly predict:
* **Biological Age** (Regression)
* **Gender** (Classification)

---

## 🧠 The "Chitragupta" Architecture (Model)
Just as Yama relies on his scribe Chitragupta for records, this AI relies on a **Multi-Task Learning (MTL)** architecture to process data efficiently. Instead of running two separate models, AI-Yama uses a **Shared Backbone**:

1.  **The Eye (Input):** Accepts a 128x128 grayscale image.
2.  **The Brain (Shared CNN):** A 4-layer Convolutional Neural Network extracts deep facial features (edges, textures, shapes).
3.  **The Verdict (Dual Output):**
    * **Branch A (Gender):** A Sigmoid classifier that distinguishes Male from Female.
    * **Branch B (Age):** A ReLU regression head that estimates age as a continuous number.
<img width="685" height="235" alt="image" src="https://github.com/user-attachments/assets/0d5dc70c-fb14-4c17-a2c7-eb56807bbb10" />


---

## 🛠️ Tech Stack
* **Core:** Python 3.x
* **Neural Network:** TensorFlow / Keras (Functional API)
* **Vision:** OpenCV (Haar Cascades for face detection)
* **Data Handling:** NumPy, Pandas (Custom serialization for speed)
* **Interface:** IPython/JavaScript Bridge (For Colab Webcam support)

---

## ⚡ Instant Judgment (Using Pre-Trained Model)
Don't want to wait for training? You can load the trained "brain" of Yama immediately to start making predictions. 

Ensure you have the `final_model.keras` file in your directory and run:

```python
import tensorflow as tf

try:
    # Load the all-seeing model
    model = tf.keras.models.load_model('final_model.keras')
    print("Success! AI-Yama is ready to judge.")
except Exception as e:
    print(f"Summoning failed: {type(e).__name__}")
    print(f"Error Message: {e}")
```

---

## 🚀 How to Summon AI-Yama (Installation & Usage)

### 1. Clone the Repository
```bash
git clone [https://github.com/lovevyas/AI-Yama.git](https://github.com/lovevyas/AI-Yama.git)
cd AI-Yama
```

### 2. Install Dependencies
Since this project relies on specific Deep Learning libraries, install them directly:
```bash
pip install tensorflow pandas numpy matplotlib seaborn opencv-python tqdm kagglehub
```

### 3. Run the Ritual (Notebook)
Open the notebook file (e.g., `Age_Gender_Prediction.ipynb`) in **Google Colab** or Jupyter.
* **Data Setup:** The script automatically downloads the UTKFace dataset via `kagglehub`.
* **Webcam Demo:** Scroll to the final section of the notebook to activate the "Real-Time Webcam Bridge" and see the model work live in your browser.

---

## 📊 Performance Metrics
* **Gender Accuracy:** ~90%
* **Age Prediction:** Mean Absolute Error (MAE) of ~6-8 years.
    * *Note: Like the real Yama, the model is most accurate with adults. Very young children or very elderly faces may show slightly higher variance.*

---

## 👤 Author
**Love Vyas**
* [LinkedIn](https://www.linkedin.com/in/love-vyas)
* [GitHub](https://github.com/lovevyas)

> *"Your face is the index of your mind."*
