# 🧠 ManoVani – Conversational AI for Depression Detection

**ManoVani** is a voice-enabled AI system that intelligently detects signs of depression by analyzing both speech and text. It simulates an empathetic dialogue with users, offering support while classifying their mental state into no depression, mild/false depression, or true depression. Built using machine learning and natural language processing, it aims to provide early mental health intervention.

---

## 🌟 Features

- 🗣️ **Voice Assistant (Sakhi)** – Natural conversation via voice
- 📊 **NBTree Classifier** – Hybrid Naive Bayes + Decision Tree model
- 🔍 **Feature Engineering** – PCA & standard scaling applied on extracted features
- 🧾 **Data Source** – DAIC-WOZ dataset for depression detection
- 📁 **Audio Feedback** – Generates AI voice output after analysis
- 🔒 **Privacy-first** – Local inference, no personal data stored or uploaded

---

## 🧠 How It Works

mermaid
```graph TD;
    A[User Voice Input] --> B[Speech-to-Text + Preprocessing]
    B --> C[Feature Extraction]
    C --> D[Scaling & PCA]
    D --> E[Ensemble ML Model (NBTree)]
    E --> F[Depression Classification]
    F --> G[Voice Response (response.mp3)]
```
🗂️ Project Structure
```graphql
ManoVani/
├── README.md                  # Project overview (this file)
├── index.md                   # GitHub Pages version of README
├── _config.yml                # GitHub Pages theme config
├── main.py                    # Runs full system pipeline
├── sakhi.py                   # Handles voice input/output
├── model.py                   # Loads model and transformers
├── best_ensemble_model.pkl    # Trained depression detection model
├── scaler.pkl                 # StandardScaler for normalization
├── pca.pkl                    # PCA dimensionality reduction
├── processed_data.pkl         # Preprocessed dataset features
├── response.mp3               # AI's voice response
├── requirements.txt           # Python dependencies
└── LICENSE                    # MIT License (recommended)
```
📦 Installation
Clone the repository

```bash
git clone https://github.com/NandiniJaiswal05/ManoVani.git
cd ManoVani
```
Install dependencies
```bash
pip install -r requirements.txt
```
▶️ Run the Application
```bash
python main.py
```
Speak when prompted.

The AI will process your voice and provide a depression assessment.

Response is saved and played from response.mp3.

## 🧪 Dataset Used
- Name: DAIC-WOZ Dataset

- Files Used: covarep.csv, formant.csv, transcript.csv, audio.wav

- Purpose: Detect depression from speech and facial cues during interviews.

##🔍 Model Details
- Algorithm: Ensemblled Learning (RandomForest, XGBoost, Voting Classifier, NBTree)

# Preprocessing:

- StandardScaler for normalization

- PCA for reducing noise and complexity

**Performance: Optimized on validation subset of DAIC-WOZ**

##🛠️ Tools & Technologies
- 🐍 Python 3.11+

- 🔬 scikit-learn

- 🧠 NLTK, NumPy, pandas

- 🧏 SpeechRecognition, PyAudio, gTTS

- 📊 PCA, StandardScaler

- 📁 Git, GitHub Pages

## 🌐 GitHub Pages Deployment
Project is also accessible via GitHub Pages:
📍 [ManoVani](https://github.com/KanakDharamthok/Fake-Depression-Detection-Using-Speech-Analysis)

💡 Future Enhancements
- ✅ Multilingual support (Hindi, Marathi)

- ✅ Full frontend (Streamlit or React)

- ✅ Emotion timeline and progress tracking

- ✅ Doctor/counselor integration API

- ✅ Docker & Android deployment

📜 License
This project is licensed under the MIT License.

⚠️ Disclaimer: This is a research-based assistant and not a substitute for professional mental healthcare.

🙋‍♀️ Author
- ✨ Kanak Dharamthok
- 🚀 Third-Year CSE (AIML) Student | Passionate about building real-world solutions through AI & ML
- 🧠 Mental Health Advocate | Contributed to Manovani: an AI-powered system for detecting depression using voice and text analysis
- 🔬 AI/ML Researcher in Progress | Exploring NLP, Emotion Recognition, and Responsible AI
- 💬 Loves turning data into meaningful insights and bringing empathy into tech
- 🌱 Learning: ML applications, Research Paper Writing
- 📚 Always open to collaborations, ideas, and learning new things

📍 GHRCE, India

🤝 Contributions
Pull requests, feature ideas, and bug reports are welcome!

```bash
# Fork → Code → Pull Request ✔️
```
📬 Contact
📧 ms.kanak.dharamthok@gmail.com
📦 GitHub: [KanakDharamthok](https://github.com/KanakDharamthok)
🔗 Linkedin: [Kanak Dharamthok](https://www.linkedin.com/in/kanak-dharamthok-8b6b8928b/)
