# 🚀 Prompt Analyzer

An AI-powered Prompt Evaluation and Experimentation platform built with FastAPI, React, MongoDB, Docker, Jenkins, and SonarQube.

---

# 📌 Overview

Prompt Analyzer is a full-stack platform designed for testing, evaluating, comparing, and optimizing AI prompts using deterministic scoring metrics and multi-model analysis.

The system helps developers and prompt engineers analyze prompt quality, compare responses from different LLMs, track prompt versions, and monitor prompt performance over time.

---

# 🎯 Main Objectives

- Evaluate prompt quality using deterministic metrics
- Compare outputs from multiple AI models
- Perform A/B prompt testing
- Store prompt history and revsions
- Capture user feedback
- Detect prompt injection attempts
- Integrate DevOps workflows for deployment and quality monitoring

---

# 🧠 Features

## ✅ Prompt Evaluation

The platform evaluates prompts using:

- Clarity scoring
- Context scoring
- Specificity checks
- Instruction quality analysis
- Ambiguity detection
- Conciseness analysis
- Keyword relevance validation
- Response format validation

---

## 🔄 A/B Prompt Testing

Compare two prompts side-by-side and analyze:

- Response quality
- Scoring differences
- Best prompt recommendation
- Regression changes

---

## 🤖 Multi-Model Comparison

Supports comparisons between:

- Gemini
- Groq
- HuggingFace Models

Includes:

- Latency tracking
- Quality scoring
- Model performance comparison

---

## 📚 Prompt Version History

- Save prompt revisions
- Track prompt improvements
- Load previous versions
- Monitor prompt regressions

---

## 👍 Feedback System

- Thumbs-up / thumbs-down reactions
- User comments
- Feedback storage for future analysis

---

## 🛡️ Security Features

- Prompt injection detection
- Safe mock responses when API keys are unavailable
- Input validation and sanitization

---

# 🧩 Tech Stack

## Backend
- FastAPI
- Python
- Motor (MongoDB Driver)

## Frontend
- React
- Vite
- Nginx

## Database
- MongoDB

## DevOps
- Docker
- Docker Compose
- Jenkins
- SonarQube
- GitHub Actions Ready

---

# 📂 Project Structure

```bash
Prompt-Analyzer/
│
├── backend/
│   ├── Dockerfile
│   ├── requirements.txt
│   ├── .env
│   └── ...
│
├── frontend/
│   ├── Dockerfile
│   ├── nginx.conf
│   └── ...
│
├── docker-compose.yml
├── Jenkinsfile
└── README.md
```

---

# ⚙️ Local Setup

## Backend Setup

```bash
cd backend

python -m venv venv

source venv/bin/activate

pip install -r requirements.txt

uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

---

## Frontend Setup

Open another terminal:

```bash
cd frontend

npm install

npm run dev
```

---

# 🌐 Local URLs

| Service | URL |
|---|---|
| Frontend | http://localhost:5173 |
| Backend | http://localhost:8000 |
| Swagger Docs | http://localhost:8000/docs |

---

# 🔐 Environment Variables

Create a `.env` file inside backend:

```env
GROQ_API_KEY=your_groq_key
GOOGLE_API_KEY=your_gemini_key
HUGGINGFACE_API_KEY=your_huggingface_key
```

If API keys are unavailable, the backend automatically uses safe mock responses.

---

# 🐳 Docker Setup

## Run Full Application

```bash
docker compose up --build
```

## Stop Containers

```bash
docker compose down
```

---

# 🐳 Manual Docker Builds

## Backend

```bash
docker build -t prompt-analyzer-backend ./backend
```

## Frontend

```bash
docker build -t prompt-analyzer-frontend ./frontend
```

---

# 🔄 Jenkins CI Pipeline

Integrated CI pipeline includes:

- Source code checkout
- Backend validation
- Frontend build
- SonarQube analysis
- Docker build support

---

# 📊 SonarQube Integration

The project uses SonarQube for:

- Code quality analysis
- Vulnerability detection
- Code smell detection
- Maintainability tracking

---

# 📍 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/analyze` | Analyze prompt |
| POST | `/api/optimize` | Optimize prompt |
| POST | `/api/compare` | Compare AI models |
| POST | `/api/ab-test` | A/B prompt testing |
| POST | `/api/feedback` | Submit feedback |
| GET | `/api/prompt-history` | Fetch prompt history |
| POST | `/api/prompt-history` | Save prompt version |

---

# 📈 Workflow

```text
GitHub
   ↓
Jenkins CI Pipeline
   ↓
Backend Validation
   ↓
Frontend Build
   ↓
SonarQube Analysis
   ↓
Docker Deployment
```

---

# ✅ Current Status

- Backend integration completed
- Frontend UI completed
- MongoDB integration working
- Docker containerization completed
- Jenkins pipeline configured
- SonarQube analysis configured
- Prompt history tracking implemented
- Feedback system implemented

---

# 📚 Learning Outcomes

This project demonstrates:

- Full-stack application development
- Prompt engineering workflows
- DevOps integration
- Docker containerization
- CI/CD pipeline implementation
- Multi-model experimentation
- Backend API architecture

---

# 🚀 Future Improvements

- Analytics dashboard
- Prompt regression graphs
- Kubernetes deployment
- Authentication system
- Monitoring and logging
- Cloud deployment support
- Unit and integration testing

---

# 👨‍💻 Author

Developed for learning, experimentation, and AI workflow analysis.
