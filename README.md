# 👹 AI-Yama: The Biometric Judgment Suite

> *"In the Grand Hall of Justice, nothing is hidden. One eye sees the timeline of your life (Age & Gender), while the other peers into the turbulence of your heart (Emotion)."*

![Project Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/Suite-Deep%20Learning-orange)

---

## 🏛️ The Grand Archive (Overview)
**AI-Yama** is a comprehensive computer vision suite designed to extract deep biological and psychological attributes from human faces.

This repository serves as the central hub for two distinct deep learning systems, each acting as a specialized "judge" of human characteristics. By leveraging Multi-Task Learning and Convolutional Neural Networks, this suite transforms a simple camera feed into a tool of omniscience.

---

## 🔮 The Two Eyes of Yama (Modules)

### 1. [The All-Seeing Face Analyst (Age & Gender)](./Age-Gender-Detection)
> *folder: `Age-Gender-Detection/`*

A **Multi-Task Learning (MTL)** system that simultaneously predicts biological age and gender from a single image.
* **Capabilities:** Age Regression (Years), Gender Classification (Male/Female).
* **Tech:** Multi-Output CNN, Shared Backbone, UTKFace Dataset.
* **[🔗 Enter the Hall of Age & Gender](./Age-Gender-Detection)**

### 2. [The Soul Reader (Emotion Detection)](./Emotion-Detection)
> *folder: `Emotion-Detection/`*

A specialized **CNN Classifier** tuned to detect micro-expressions and reveal the subject's emotional state.
* **Capabilities:** Detects 7 core emotions (Angry, Happy, Sad, Fear, Disgust, Surprise, Neutral).
* **Tech:** VGG-style Deep CNN, FER-2013 Dataset.
* **[🔗 Enter the Hall of Emotions](./Emotion-Detection)**

---

## 🛠️ Unified Tech Stack
Both systems share a robust, modern foundation:
* **Core:** Python 3.x
* **Deep Learning:** TensorFlow / Keras
* **Computer Vision:** OpenCV (Haar Cascades)
* **Deployment:** JavaScript-Python Bridge for Real-Time Cloud Inference (Google Colab).

---

## 🚀 How to Navigate (Installation)

To use either tool, clone this entire repository and navigate to the specific module you wish to summon.

```bash
# 1. Clone the Grand Archive
git clone [https://github.com/lovevyas/AI-Yama.git](https://github.com/lovevyas/AI-Yama.git)
cd AI-Yama

# 2. Choose your path:

# --- To Judge Age & Gender ---
cd Age-Gender-Detection
# Follow the README inside this folder...

# --- OR ---

# --- To Judge Emotions ---
cd Emotion-Detection
# Follow the README inside this folder...
