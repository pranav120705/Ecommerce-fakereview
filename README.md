# 🛡️ RevGuard — Fake Review Detection System  
**Walmart Sparkathon 2025 | Customer Trust / Retail Cybersecurity**

RevGuard is an AI-powered fake review detection system designed to identify deceptive and manipulated product reviews on e-commerce platforms.  
It uses a **fine-tuned RoBERTa transformer model** to classify reviews as **FAKE** or **GENUINE**, along with a confidence score, enabling platforms and users to make more informed trust decisions.

---

## 🚀 Project Overview

Online reviews heavily influence customer purchasing decisions, but fake reviews undermine trust and fairness in digital marketplaces.  
RevGuard addresses this problem by leveraging **state-of-the-art NLP models** to detect suspicious reviews in real time.

**Key Capabilities**
- Binary classification: **FAKE / GENUINE**
- Confidence-based predictions
- REST API backend for easy integration
- Scalable ML inference pipeline
- Frontend dashboard for testing predictions

---

## 🧠 Model Details

- **Base Model:** `roberta-base` (Hugging Face)
- **Architecture:** Transformer-based binary classifier
- **Labels:** 2 (`FAKE`, `GENUINE`)
- **Framework:** PyTorch + Hugging Face Transformers

### 🔍 Inference Pipeline
Review Text
↓
Tokenizer
↓
RoBERTa Encoder
↓
Logits
↓
Softmax
↓
Prediction + Confidence (%)

bash
Copy code

### 📌 Example Output
```json
{
  "prediction": "FAKE",
  "confidence": 92.73
}
📁 Project Structure
graphql
Copy code
RevGuard/
├── backend/
│   ├── app/                      # API logic (FastAPI / Flask)
│   │   └── __pycache__/
│   ├── models/
│   │   └── roberta_saved_model/  # Fine-tuned RoBERTa model files
│   ├── requirements.txt
│   └── app.py
│
├── fontend/                      # React frontend (typo retained intentionally)
│   ├── src/
│   ├── package.json
│   └── vite.config.js
│
└── README.md
🔧 Running the Project Locally
1️⃣ Backend Setup (Python)
Install dependencies:

bash
Copy code
pip install -r backend/requirements.txt
Start the backend server:

bash
Copy code
python backend/app.py
The API will be available at:

arduino
Copy code
http://localhost:8000
2️⃣ Frontend Setup (React + Vite)
Navigate to frontend directory:

bash
Copy code
cd fontend
Install dependencies:

bash
Copy code
npm install
Start development server:

bash
Copy code
npm run dev
⚙️ Tech Stack
Backend: Python, FastAPI / Flask

ML Framework: PyTorch

NLP: Hugging Face Transformers (roberta-base)

Frontend: React (Vite)

Deployment Ready: Docker / Cloud compatible

☁️ Future Enhancements
🌍 Multilingual fake review detection

🔗 Metadata & source-based validation (user history, product signals)

🧪 Adversarial fake review generation for robustness

🚀 Cloud deployment (AWS Lambda / Hugging Face Inference Endpoints)

📊 Admin dashboard with analytics and monitoring

🤝 Team
Team Horizons

🏆 Hackathon Submission
Event: Walmart Sparkathon 2025
Track: Customer Trust / Retail Cybersecurity
Theme: AI for Online Review Reliability

📜 License
This project is for educational and hackathon purposes.
Model weights and datasets follow their respective licenses.

RevGuard — Building Trust, One Review at a Time. 🛡️
