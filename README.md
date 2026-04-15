# 🚀 Transformer-based English → Vietnamese Translator (Fine-tuned NMT System)

## 📌 Overview

This project implements a Neural Machine Translation (NMT) system for
translating English to Vietnamese, built by fine-tuning a pretrained
Transformer model from:

https://huggingface.co/Helsinki-NLP/opus-mt-en-vi

The system demonstrates a complete end-to-end machine learning pipeline,
including model adaptation, inference deployment, and full-stack
integration via a web application.

---

## ✨ Key Highlights

- Fine-tuned a state-of-the-art Transformer model for EN → VI
  translation
- Built a complete ML pipeline: preprocessing → training → inference
- Developed RESTful API for real-time translation
- Designed a modern frontend UI for user interaction
- Structured project following production-level practices

---

## 🧠 Model & Methodology

### Base Model

- Model: Helsinki-NLP/opus-mt-en-vi
- Architecture: Transformer (encoder--decoder)
- Tokenization: SentencePiece

### Fine-tuning Approach

- Adapted pretrained model to custom dataset
- Improved domain-specific translation quality
- Optimized inference for real-time usage

Pipeline: 1. Data preprocessing $\rightarrow$ 2. Tokenization $\rightarrow$ 3. Fine-tuning $\rightarrow$ 4.Evaluation $\rightarrow$ 5. Deployment

---

## 🏗️ System Architecture

Frontend (React + Vite)\
↓\
Backend API (Python - FastAPI/Flask)\
↓\
Fine-tuned Transformer Model

---

## 📁 Project Structure

```
project-root/
├── backend/
│   ├── server.py                 # API server (serves translation requests)
│   ├── demo.py                   # Demo script for testing
│   ├── requirements.txt          # Python dependencies
│   ├── setup.py                  # Package setup (if applicable)
│   └── src/
│       └── translate_pipeline.py # Translation inference pipeline
├── frontend/
│   ├── src/
│   │   ├── App.jsx               # Main React component
│   │   ├── main.jsx              # Entry point
│   │   └── components/
│   │       └── TranslatorBox.jsx # Translation UI component
│   ├── index.html                # HTML template
│   ├── package.json              # Frontend dependencies
│   └── vite.config.js            # Vite configuration
├── code_du_doan.py               # Additional prediction script
└── README.md                     # Project documentation
```

---

## ⚙️ Tech Stack

Machine Learning: - Python - PyTorch / TensorFlow - Transformer

Backend: - FastAPI / Flask

Frontend: - React - Vite

---

## 🚀 Getting Started

### Backend

```bash
cd backend
pip install -r requirements.txt
python server.py
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 📡 API Example

POST /translate

Request: { "text": "Hello, how are you?" }

Response: { "translation": "Xin chào, bạn khỏe không?" }

---

## 📈 Future Improvements

- Improve BLEU score
- Domain fine-tuning
- Cloud deployment
- Add translation history

---

## 💼 Why This Project Matters

- Demonstrates NLP & Deep Learning knowledge
- Shows fine-tuning pretrained models
- End-to-end ML system building
- Full-stack integration

---

## 👨‍💻 Authors

- Nguyen Tran Loi
- Tran Minh Tam
- Mai Xuan Quy

---

## 📜 License

MIT

---

## 🔗 References

https://huggingface.co/Helsinki-NLP/opus-mt-en-vi  
https://huggingface.co/CLAck/en-vi
