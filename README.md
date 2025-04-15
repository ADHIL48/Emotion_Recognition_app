
 <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/logo.png" alt="Big Smile Emoji" width="150px" align="right"><h1 align="center">🎭 Feel My Emotion - Multi-Modal Emotion Recognition App</h1>


> An intelligent, multi-modal emotion recognition system that understands how you feel—through your words, face, and voice.

<div style="display: flex; justify-content: space-around; flex-wrap: wrap;">
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/Happy.gif" alt="Happy" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/gif/angry.gif" alt="Angry" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/Neutral.gif" alt="Neutral" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/Sad.gif" alt="Sad" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/gif/disgust.gif" alt="Disgust" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/Disgust.gif" alt="Fear" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/gif/surprise.gif" alt="Pleasant Surprise" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/gif/love.gif" alt="Love" width="90"/>
  <img src="https://github.com/ADHIL48/Emotion_Recognition_app/raw/main/Emotion_Recognition%20_App_Using_Streamlit/images/Emoji/gif/humor.gif" alt="Humor" width="90"/>
</div>

---

## 📌 Table of Contents

- [🌟 Project Overview](#-project-overview)
- [✨ Key Features](#-key-features)
- [🛠 Technologies Used](#-technologies-used)
- [📥 Installation Guide](#-installation-guide)
- [🚀 Usage Instructions](#-usage-instructions)
- [📂 Project Structure](#-project-structure)
- [🧠 Models Architecture](#-models-architecture)
- [📊 Performance Metrics](#-performance-metrics)
- [📡 API Documentation](#-api-documentation)
- [📸 Screenshots](#-screenshots)
- [🚀 Future Enhancements](#-future-enhancements)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)
- [📞 Contact](#-contact)

---

## 🌟 Project Overview

**Feel My Emotion** is a multi-modal emotion recognition app that uses machine learning to analyze human emotions via text, facial expressions, and speech. Whether you're typing a message, recording your voice, or showing your face on camera, the app can detect and interpret your emotional state in real-time.

✅ Multi-modal inputs  
✅ Personalized wellbeing recommendations  
✅ Visualizations & analytics dashboard  
✅ Emotional support AI chatbot  

---

## ✨ Key Features

### 🔤 Text Emotion Recognition
- Supports typed input and TXT file uploads
- Detects 8 emotions: 😊 Happy, 😢 Sad, 😠 Angry, 😨 Fearful, 🤢 Disgusted, 😲 Surprised, 😐 Neutral, ❤️ Loving

### 📷 Face Emotion Recognition
- Static and real-time webcam-based analysis
- Emotion & gender detection
- Multi-face support

### 🎙 Speech Emotion Recognition
- Record live audio (5s segments) or upload `.wav` files
- MFCC-based analysis with waveform visualization

### 🔁 Multi-Modal Emotion Analysis
- Combines all modalities with a weighted approach
- Final report includes emotion agreement insights

### 💬 Chat & Visual Features
- AI-powered emotion chatbot (LangChain & Ollama)
- Radar and bar charts for emotion breakdown
- Emotion GIF reactions
- Dark/light mode support
- Historical tracking & usage streaks

---

## 🛠 Technologies Used

| Tech         | Purpose                      | Version   |
|--------------|------------------------------|-----------|
| Python       | Backend logic                | 3.9+      |
| Streamlit    | Frontend web interface       | 1.22+     |
| DeepFace     | Facial emotion analysis      | 0.0.79    |
| Librosa      | Audio feature extraction     | 0.9.2     |
| Scikit-learn | Text classification (NLP)    | 1.2.2     |
| TensorFlow   | Speech emotion CNN model     | 2.12.0    |
| Plotly, Altair| Interactive visualizations   | 5.14.1, 4.2.2 |
| LangChain    | LLM & AI chatbot integration | 0.0.200   |
| Ollama       | Local language model server  | 0.1.0     |

---

## 📥 Installation Guide

### ⚙️ System Requirements

- Minimum 4GB RAM, 2GB Disk
- Webcam (Face), Microphone (Speech)

### 🧱 Setup Steps

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate        # Linux/macOS
venv\Scripts\activate           # Windows

# Install dependencies
pip install -r requirements.txt

# Optional (Linux dependencies)
sudo apt-get install -y libsndfile1 ffmpeg
```

### 🧠 Model Downloads

On first run, models for text, speech, and face analysis are auto-downloaded.

### ⚙️ Environment Variables

Create a `.env` file:

```env
DARK_MODE=True
DEFAULT_MODALITY=multi
```

### ▶️ Run the App

```bash
streamlit run app.py
```

---

## 🚀 Usage Instructions

#### 🔤 Text Analysis
- Enter short text or upload `.txt` file
- View predicted emotion, confidence, and recommendation

#### 📸 Face Analysis
- Choose static photo or enable webcam
- Real-time results with emotion, confidence, and gender labels

#### 🎤 Speech Analysis
- Record or upload `.wav` audio
- View waveform and emotion probabilities

#### 🔁 Multi-Modal Flow
- Complete all 3 steps
- Final confidence-weighted emotion result + report

---

## 📂 Project Structure

```
Emotion_Recognition_app/
├── main/                   # Application source code
│   ├── app.py              # Main Streamlit app
│   ├── models/             # ML models for each modality
│   ├── utils/              # Helper and visualization functions
│   ├── assets/             # Images and emotion GIFs
│   └── tests/              # Unit & integration tests
├── docs/                   # API and architecture docs
├── requirements.txt        # Dependency list
├── .env.example            # Environment variable template
├── LICENSE                 # MIT License
└── README.md               # Project README
```

---

## 🧠 Models Architecture

### Text Classifier (Logistic Regression)
- TF-IDF with n-gram (1,3)
- Dataset: ISEAR
- Accuracy: 86%

### Speech Classifier (1D CNN)
- Features: MFCC (40 coefficients)
- Dataset: RAVDESS
- Accuracy: 78%

### Face Classifier (VGG-Face)
- Dataset: FER-2013
- Accuracy: 72%
- Outputs: Emotion + Gender

---

## 📊 Performance Metrics

| Modality | Precision | Recall | F1-Score | Avg Inference |
|----------|-----------|--------|----------|----------------|
| Text     | 0.86      | 0.85   | 0.85     | 120ms          |
| Speech   | 0.78      | 0.76   | 0.77     | 380ms          |
| Face     | 0.72      | 0.71   | 0.71     | 680ms          |
| Multi-modal | —      | —      | —        | 3.2s           |


---

## 🚀 Future Enhancements

### Features Coming Soon
- 📱 React Native mobile app
- 📊 Emotion trend timeline
- 🧘 Health app sync (Apple/Google)
- 📓 AI mood journal
- 🩺 Therapist dashboard (Pro edition)

### Technical Upgrades
- 💡 Transformers for NLP
- 🗣 Transfer learning in speech
- 🎥 3D CNN for video-based emotion
- 🌐 ONNX edge deployment
- 🌍 Multi-language support

---

## 🤝 Contributing

We welcome contributions!

```bash
# Set up environment
git clone https://github.com/ADHIL48/Emotion_Recognition_app.git
cd Emotion_Recognition_app
pip install -r requirements-dev.txt

# Run tests
pytest tests/

# Format code
black .
```

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## 📜 License

**MIT License**  
See full text in [LICENSE](LICENSE)

---

## 📞 Contact

**Adhil M**  
📧 [mohammedadhil0408@gmail.com](mailto:mohammedadhil0408@gmail.com)  
🌐 [GitHub](https://github.com/ADHIL48) | [LinkedIn](https://linkedin.com/in/adhil-m) | 📱 WhatsApp: +91 6382191903

🔗 **Project Links**:  
- [🔧 GitHub Repository](https://github.com/ADHIL48/Emotion_Recognition_app)  
- [📺 Live Demo (Streamlit)](https://share.streamlit.io/adhil48/emotion_recognition_app/main/app.py)

---

> 💬 _"Your emotions matter. Let your apps feel them too."_
```
