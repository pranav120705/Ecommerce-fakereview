
# 🛡️ RevGuard — Fake Review Detection System

![Hackathon](https://img.shields.io/badge/Event-Walmart%20Sparkathon%202025-blue)
![Track](https://img.shields.io/badge/Track-Customer%20Trust%20%2F%20Retail%20Cybersecurity-green)
![Status](https://img.shields.io/badge/Status-Prototype-orange)

**RevGuard** is an AI-powered fake review detection system designed to identify deceptive and manipulated product reviews on e-commerce platforms. It leverages a **fine-tuned RoBERTa transformer model** to classify reviews as **FAKE** or **GENUINE**, providing a confidence score to enable better trust decisions.

---

## 🚀 Project Overview

Online reviews heavily influence purchasing decisions, but fake reviews undermine trust and fairness in digital marketplaces. RevGuard addresses this problem by leveraging **state-of-the-art NLP models** to detect suspicious reviews in real-time.

### Key Capabilities
* **Binary Classification:** Detects `FAKE` vs `GENUINE` reviews.
* **Confidence Scoring:** Provides probability percentages for predictions.
* **REST API Backend:** Easy integration using FastAPI/Flask.
* **Interactive Dashboard:** React-based frontend for testing predictions.

---

## 🧠 Model Details

* **Base Model:** `roberta-base` (Hugging Face)
* **Architecture:** Transformer-based binary classifier
* **Framework:** PyTorch + Hugging Face Transformers
* **Labels:** `FAKE`, `GENUINE`

### 🔍 Inference Pipeline
`Review Text` $\rightarrow$ `Tokenizer` $\rightarrow$ `RoBERTa Encoder` $\rightarrow$ `Logits` $\rightarrow$ `Softmax` $\rightarrow$ `Prediction + Confidence (%)`

### 📌 Example Output
```json
{
  "prediction": "FAKE",
  "confidence": 92.73
}

```


## ⚙️ Tech Stack

* **Backend:** Python, FastAPI / Flask
* **ML Framework:** PyTorch
* **NLP:** Hugging Face Transformers (`roberta-base`)
* **Frontend:** React (Vite)
* **Deployment:** Docker / Cloud compatible

---

## 📁 Project Structure

```graphql
RevGuard/
├── backend/
│   ├── app/                    # API logic
│   │   └── __pycache__/
│   ├── models/
│   │   └── roberta_saved_model/ # Fine-tuned RoBERTa model files
│   ├── requirements.txt
│   └── app.py
│
├── fontend/                    # React frontend
│   ├── src/
│   ├── package.json
│   └── vite.config.js
│
└── README.md

```

---

## 🔧 Running the Project Locally

### 1️⃣ Backend Setup (Python)

Navigate to the root directory and install dependencies:

```bash
pip install -r backend/requirements.txt

```

Start the backend server:

```bash
python backend/app.py

```

> The API will be available at: `http://localhost:8000`

### 2️⃣ Frontend Setup (React + Vite)

Navigate to the frontend directory:

```bash
cd fontend

```

Install dependencies:

```bash
npm install

```

Start the development server:

```bash
npm run dev

```

---

## ☁️ Future Enhancements

* 🌍 **Multilingual Support:** Detect fake reviews in multiple languages.
* 🔗 **Metadata Validation:** Analyze user history and product signals.
* 🧪 **Adversarial Robustness:** Test against generated fake reviews.
* 🚀 **Cloud Deployment:** AWS Lambda or Hugging Face Inference Endpoints.
* 📊 **Admin Dashboard:** Analytics and monitoring tools.

---

## 🤝 Team

**Team Horizons**

---

## 🏆 Hackathon Submission

* **Event:** Walmart Sparkathon 2025
* **Track:** Customer Trust / Retail Cybersecurity
* **Theme:** AI for Online Review Reliability

---

## 📜 License

This project is for educational and hackathon purposes. Model weights and datasets follow their respective licenses.

> **RevGuard — Building Trust, One Review at a Time. 🛡️**

```

**Next Step:** Would you like me to generate the `requirements.txt` or the `app.py` file to match this README?

```
