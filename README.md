# 🏆 COVID-19 & Lung Disease Detection App (Image + Audio)

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/UI-Streamlit-ff4b4b?logo=streamlit)
![TensorFlow](https://img.shields.io/badge/Model-TensorFlow-orange?logo=tensorflow)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

> 🥇 **Awarded 7th Place** at the **Arab Artificial Intelligence Olympiad 2025** for innovation in AI-powered healthcare solutions.

---

## 📌 Overview

The **PulmoAI Detection App** is an advanced AI-powered diagnostic system that detects **COVID-19**, **Viral Pneumonia**, and **normal lung conditions** using both **chest X-ray images** and **cough audio recordings**.

The project was honored with **7th place** in the **Arab AI Olympiad 2025**, showcasing the power of dual-modal AI systems in real-world healthcare settings.

---

## 🚀 Features

- 🖼️ **Chest X-ray Detection**: Classifies X-ray images into COVID-19, Pneumonia, or Normal.
- 🔊 **Cough Audio Analysis**: Accepts uploaded or live-recorded cough audio and classifies it.
- 🧪 **Dual-Modal AI Integration**: Merges both image and audio models for flexible diagnosis.
- 📊 **High Accuracy**: CNN-based models with strong training performance.
- 🌐 **Streamlit Interface**: Fully web-based and user-friendly.
- 🎙️ **Real-time Audio Capture**: Supports live cough recording through microphone.
- 📁 **Cross-platform Compatibility**: Runs on Windows, Linux, macOS.

---

## 🏗️ Tech Stack

| Layer         | Tools & Libraries                                 |
|---------------|---------------------------------------------------|
| Language      | Python 3.8+                                       |
| Interface     | Streamlit, HTML, CSS                              |
| Deep Learning | TensorFlow, Keras, OpenCV, NumPy                  |
| Audio         | Librosa, SoundFile, Matplotlib, streamlit-webrtc |
| Models        | CNN for images and spectrograms                   |
| Deployment    | Local, Docker, or Cloud (optional)                |

---

## 📂 Project Structure

📦 PulmoAI-COVID-Detection
┣ 📂 models/
┃ ┣ lung_disease_model.h5 # Image model
┃ ┗ cough_model_multi.h5 # Audio model
┣ 📂 static/ # CSS, images
┣ 📂 utils/ # Preprocessing
┣ 📜 app.py # Main Streamlit app
┣ 📜 requirements.txt # Dependencies
┣ 📜 README.md # Documentation
┗ 📜 LICENSE # MIT License

yaml
Copy
Edit

---

## 🖥️ Installation & Running

### Prerequisites

- Python 3.8+
- `pip`
- `ffmpeg` (for audio processing)
- Recommended: virtual environment

### Setup Instructions

```bash
# Clone the repository
git clone https://github.com/MomenBhais/pulmoai-covid-app.git
cd pulmoai-covid-app

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run app.py
🎯 How It Works
🖼️ Image Classification
Input: Chest X-ray image (.jpg/.png)

Processed using OpenCV

Resized to 250x250 and normalized

Passed to CNN model

Output: COVID-19, Normal, or Viral Pneumonia

🔊 Audio Classification
Input: Cough .wav file or real-time mic recording

Transformed into mel-spectrogram via Librosa

Spectrogram resized to 64x64 and fed into a CNN model

Output: COVID-19, Symptomatic, or Healthy

🧪 Model Info
Modality	Input	Model Type	Accuracy
Image	Chest X-ray (RGB)	CNN	95%
Audio	Cough (WAV + Mel)	CNN	~90%

🧠 Future Improvements
📱 Native mobile app (Flutter / React Native)

🩺 Multi-label disease classification (e.g., TB, Asthma)

🌐 Multilingual support (Arabic, French, etc.)

🤖 Add AI interview bot for symptom checking

🧑‍💻 Author
Momen Mohammed Bhais

🌍 [LinkedIn Profile](https://www.linkedin.com/in/momen-bhais-b5739b317?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app)

🐙[ GitHub Profile](https://github.com/MomenBhais)

📧 momenbhais@outlook.com

📜 License
This project is licensed under the MIT License. See the LICENSE file for more details.

⚠️ Disclaimer
This project is intended for research and educational purposes only. It is not approved as a clinical tool and should not be used for self-diagnosis or treatment decisions.
