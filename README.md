# 🦠 COVID-19 & Lung Disease Detection App (Image + Audio)

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/DeepLearning-TensorFlow-orange?logo=tensorflow)
![Streamlit](https://img.shields.io/badge/UI-Streamlit-ff4b4b?logo=streamlit)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

> 🔬 **PulmoAI**: A dual-mode AI system for detecting COVID-19, Pneumonia, and other lung conditions using **chest X-ray images** and **cough audio recordings** — developed for the **2025 Arab AI Olympiad**.

---

## 📌 Overview

The **PulmoAI Detection App** is a powerful diagnostic aid that combines **computer vision** and **audio signal processing** to detect:

- **COVID-19**
- **Viral Pneumonia**
- **Healthy Lung States**
- **Symptomatic Non-COVID Coughs**

Using deep learning models (CNNs), the app analyzes both medical **images** and **cough audio** to assist healthcare professionals in early, rapid diagnosis.

---

## 🧠 Core Features

- 🖼️ **X-ray Image Detection**: Upload chest X-rays to detect lung diseases.
- 🔊 **Cough Audio Classification**: Upload or **record** cough audio for diagnosis.
- 🧪 **Dual-Modal AI**: Combine image and sound inputs for enhanced accuracy.
- 💡 **Spectrogram-Based Audio Analysis**: Converts coughs to mel-spectrograms before prediction.
- 🌐 **Web UI**: Built with Streamlit for cross-platform accessibility.
- 📊 **Confidence Scores**: High-accuracy predictions displayed clearly.
- 🧰 **Real-time Recording Support**: Capture audio live from microphone.

---

## 🏗️ Tech Stack

| Layer         | Tools & Libraries                                 |
|---------------|---------------------------------------------------|
| Language      | Python 3.8+                                       |
| UI/UX         | Streamlit, HTML/CSS                               |
| Deep Learning | TensorFlow / Keras, OpenCV, NumPy                 |
| Audio         | Librosa, SoundFile, Matplotlib, streamlit-webrtc |
| Models        | CNN for images & spectrograms                     |
| Deployment    | Local / Docker / Cloud (optional)                |

---

## 📂 Project Structure

📦 PulmoAI-COVID-Detection
┣ 📂 models/
┃ ┣ 📜 lung_disease_model.h5 # Image-based CNN
┃ ┗ 📜 cough_model_multi.h5 # Audio-based CNN
┣ 📂 utils/
┃ ┗ 📜 helpers.py # Preprocessing functions
┣ 📂 static/ # Custom CSS & Images
┣ 📜 app.py # Streamlit application
┣ 📜 requirements.txt # All dependencies
┣ 📜 README.md # Project documentation
┗ 📜 LICENSE

yaml
Copy
Edit

---

## 🖥️ Installation & Running

### 🔧 Prerequisites

- Python 3.8+
- `pip`
- `ffmpeg` (for audio processing)
- Virtual environment (recommended)

### 📦 Setup Instructions

```bash
# Clone the repository
git clone https://github.com/your-username/pulmoai-covid-app.git
cd pulmoai-covid-app

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
🧪 How It Works
🖼️ Image Analysis
Input: Chest X-ray image (.jpg/.png)

Preprocessed using OpenCV

Resized to (250x250) and normalized

Passed to CNN model for prediction

Output: COVID-19, Normal, or Viral Pneumonia

🔊 Cough Audio Analysis
Input: Audio file (.wav) or live microphone

Converted to Mel-spectrogram using Librosa

Spectrogram image resized to (64x64)

Passed to CNN model trained on cough sounds

Output: COVID-19, Symptomatic, or Healthy

📸 Demo
Image Detection	Cough Audio Detection
	

🚀 Future Enhancements
📱 Build a mobile version (Flutter or React Native)

🧠 Improve dataset diversity for rural/underrepresented lungs

🧪 Add multi-label detection (Tuberculosis, Asthma, etc.)

🌍 Multilingual Interface (Arabic, English, French)

🤖 Integrate voice-based symptom interview (LLM-powered)

👥 Team & Contact
Momen Mohammed Bhais — LinkedIn | GitHub


📧 For inquiries: momenbhais@outlook.com

📜 License
This project is licensed under the MIT License. See LICENSE for details.

⭐ Acknowledgements
COVID-19 radiographic image dataset (Kaggle, Cohen et al.)

CoughVid dataset

Streamlit & TensorFlow communities

🥇 Arab AI Olympiad 2025 for inspiration

