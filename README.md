
# PhishGuard AI

PhishGuard AI is a multilingual phishing detection system that scans email content, classifies it using AI, and explains potential scams. It uses XLM-RoBERTa for classification and mT5 for natural language explanations.

## 🔧 Setup

1. Go to the backend directory:

```bash
cd phishguard-ai/backend
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the FastAPI server:

```bash
uvicorn app:app --host 0.0.0.0 --port 8000
```

## 🧠 Endpoints

- `/classify`: Accepts `{ "text": "email content" }` and returns label + language.
- `/explain`: Accepts `{ "text": "email content" }` and returns a natural language explanation.
