# 👁️ AI-Yama: The Soul Reader (Emotion Detection)

> *"The face is but a mask, yet the eyes betray the soul. AI-Yama looks past the surface to reveal the turbulent emotions hidden within."*

![Project Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![FER-2013](https://img.shields.io/badge/Dataset-FER--2013-yellow)

---

## 📜 The Legend (Introduction)
In the court of Yama, judgment isn't passed just on facts, but on the *intent* and *feeling* behind actions. **AI-Yama (Emotion Edition)** extends the omniscience of the original biometric system. It does not just ask "Who are you?", but "How do you feel?"

By analyzing subtle micro-expressions and facial muscle movements, this deep learning model classifies the human emotional state into one of seven distinct "Rasas" (Emotions):
* **Angry** 😡
* **Disgust** 🤢
* **Fear** 😨
* **Happy** 😊
* **Sad** 😢
* **Surprise** 😲
* **Neutral** 😐

---

## 🧠 The "Third Eye" Architecture (Model)
To perceive emotions that often fleet across a face in milliseconds, AI-Yama utilizes a specialized **Convolutional Neural Network (CNN)** optimized for feature extraction from low-resolution inputs.

1.  **The Gaze (Input):** Processes 48x48 pixel grayscale images (from the FER-2013 standard).
2.  **The Insight (Deep Layers):**
    * **Convolutional Blocks:** Four distinct blocks with Batch Normalization and Max Pooling to capture edges (eyebrows, lips) and textures (wrinkles).
    * **Dropout Layers:** Randomly deactivates neurons during training to prevent "hallucinations" (overfitting).
3.  **The Judgment (Softmax Output):** A final dense layer calculates the probability distribution across the 7 emotional classes.

<img width="373" height="135" alt="image" src="https://github.com/user-attachments/assets/8d0ee13b-f97f-42a2-bd02-64696a954077" />


---

## 🛠️ Tech Stack
* **Core:** Python 3.x
* **Neural Network:** TensorFlow / Keras
* **Computer Vision:** OpenCV (Haar Cascades for face localization)
* **Dataset:** FER-2013 (Facial Expression Recognition)
* **Interface:** Real-Time Webcam Bridge (JavaScript/Python)

---

## ⚡ Instant Insight (Using Pre-Trained Model)
If you wish to test the Seer immediately without retraining the neural pathways:

Ensure `emotion_model.h5` (or `.keras`) is in your directory and run:

```python
import tensorflow as tf
import numpy as np

# Load the emotion model
try:
    model = tf.keras.models.load_model('emotion_model.h5')
    print("Success! The Third Eye is open.")
except Exception as e:
    print(f"Vision blocked: {e}")
```

---

## 🚀 How to Summon the Soul Reader (Installation)

### 1. Clone the Repository
```bash
git clone [https://github.com/lovevyas/AI-Yama-Emotion.git](https://github.com/lovevyas/AI-Yama-Emotion.git)
cd AI-Yama-Emotion
```

### 2. Install Dependencies
```bash
pip install tensorflow pandas numpy matplotlib opencv-python
```

### 3. Run the Ritual
Open the notebook `Emotion_Detection.ipynb` in **Google Colab**.
* **Training:** Run the training cells to teach Yama using the FER-2013 dataset.
* **Live Judgment:** Execute the final **Webcam Bridge** cell to see your emotions classified in real-time video.

---

## 📊 Performance Metrics
* **Training Accuracy:** ~75% (State-of-the-art for FER-2013 raw data is typically 70-75%).
* **Real-Time Latency:** < 50ms per frame.

---

## 👤 Author
**Love Vyas**
* [LinkedIn](https://www.linkedin.com/in/love-vyas)
* [GitHub](https://github.com/lovevyas)

> *"The mind is restless, Krishna, turbulent, strong and unyielding." — Bhagavad Gita*
