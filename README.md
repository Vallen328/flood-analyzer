# ⚙️ Flood Detection API (Backend)
### 🌐 Project Link
[https://flood-analyzer.netlify.app/](https://flood-analyzer.netlify.app/)

### 🔗 Live API
🌐 **Render Deployment:** [Backend hosted on Render)

---

## 🧠 Overview

The **Flood Detection API** is a FastAPI-based backend that predicts flood risk using:
1. **Geographic coordinates (latitude & longitude)**  
2. **Uploaded terrain images**

It leverages **Google Gemini AI** to analyze terrain elevation, proximity to water bodies, and flood-related visual patterns — returning an AI-generated structured JSON response containing risk level, analysis summary, and recommendations.

---

## 🚀 Features

✅ **Two Flood Assessment Modes**
- Coordinate-based prediction using latitude & longitude  
- Image-based flood risk analysis using AI  

✅ **AI-Powered Analysis**
- Integrates **Gemini 2.0 Flash (Generative AI)**  

✅ **Clean & Modular Architecture**
- Structured with FastAPI routes, models, and logging  

✅ **Image Validation**
- Handles image conversion, validation, and AI-safe formatting  

✅ **Ready for Production**
- Deployed on **Render** with `.env` configuration

---

## ⚙️ Tech Stack

| Layer | Technology |
|--------|-------------|
| **Framework** | [FastAPI](https://fastapi.tiangolo.com/) |
| **AI Model** | [Google Gemini AI](https://ai.google.dev/) |
| **Web Server** | [Uvicorn](https://www.uvicorn.org/) |
| **Image Processing** | [Pillow (PIL)](https://python-pillow.org/) |
| **Environment Variables** | [python-dotenv](https://pypi.org/project/python-dotenv/) |
| **Schema Validation** | [Pydantic](https://docs.pydantic.dev/) |
| **Logging** | Built-in Python `logging` module |

---

## 🧩 Folder Structure
```
backend/
│
├── main.py # Core FastAPI app
├── start.py # Entry script for Uvicorn server
├── requirements.txt # Backend dependencies
├── .env # Environment variables (not pushed)
├── .gitignore # Ignore environment & cache files
└── README.md # This documentation

```

---

## 🧠 API Endpoints

### 1️⃣ **Health Check**
**`GET /health`**  
> Verifies API and AI model status.  

**Response Example:**
```json
{
  "status": "healthy",
  "ai_model": "Gemini 2.0 Flash",
  "timestamp": "2025-10-23T12:00:00"
}
```

## ⚡ Local Setup

### 1️⃣ Clone the repository
```
git clone https://github.com/Vallen328/flood-analyzer.git
cd backend
```
### 2️⃣ Create and activate a virtual environment
```
python -m venv .venv
source .venv/bin/activate   # (Mac/Linux)
.venv\Scripts\activate      # (Windows)
```
### 3️⃣ Install dependencies
```
pip install -r requirements.txt
```
### 4️⃣ Add your .env file
```
GEMINI_API_KEY=your_gemini_api_key_here
PORT=8000
HOST=0.0.0.0
```
### 5️⃣ Run the server
```
python start.py
```

---

## Author
- **Vallen Dsouza**

## Institution
- Father Conceicao Rodrigues College of Engineering

## Description
This project is part of an AI-based flood risk prediction system. The system utilizes machine learning algorithms to predict potential flood risks based on various data inputs. It is designed to assist in making timely decisions to mitigate the impact of floods.

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) — feel free to modify and use it for learning or research purposes.
