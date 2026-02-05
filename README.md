# Convue : Intelligent Visa Processing Assistant

![Project Status](https://img.shields.io/badge/Status-Active-success) ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue) ![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688)

## 📋 Overview

**VisaAssist AI** is a specialized conversational agent designed to simplify complex visa and immigration procedures. Built on a high-performance **FastAPI** backend and powered by **Google's Gemini Generative AI**, this system provides accurate, real-time guidance on visa requirements, documentation, and application procedures for countries worldwide.

The system features a strict "domain-guard" protocol (System Instructions), ensuring the AI maintains a professional persona and exclusively addresses visa-related inquiries while politely filtering out irrelevant topics.

## ✨ Key Features

* **Intelligent Query Resolution:** Capable of understanding natural language questions regarding visa types (Tourist, Student, Work) and specific country requirements.
* **Context-Aware Guardrails:** Configured with robust system instructions to maintain focus strictly on immigration and travel documentation.
* **High-Performance Backend:** Utilizes **FastAPI** for asynchronous, non-blocking request handling.
* **Modern AI Integration:** Leverages the **Google GenAI SDK** (Gemini Flash model) for low-latency, high-accuracy responses.
* **Responsive Interface:** Intuitive chat interface featuring real-time typing indicators and mobile-friendly design.

## 🛠️ Technology Stack

* **Backend Framework:** Python 3.x, FastAPI
* **AI Engine:** Google Gemini API (`google-genai` SDK)
* **Server:** Uvicorn (ASGI Implementation)
* **Frontend:** HTML5, CSS3, Vanilla JavaScript (Fetch API)
* **Environment Management:** `python-dotenv`

## 🚀 Installation & Setup

### Prerequisites
* Python 3.9 or higher installed.
* A valid Google AI Studio API Key.

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/visa-helper-bot.git](https://github.com/your-username/visa-helper-bot.git)
cd visa-helper-bot
 **2. Configure Environment Variables**
Create a file named .env in the root directory to securely store your credentials. Add the following line:
GEMINI_API_KEY=your_actual_api_key_here

### 3. Install Dependencies
Install the required Python packages using pip:
pip install fastapi uvicorn google-genai python-dotenv

### 4. Launch the Application
Start the backend server:
python main.py

The server will initialize at http://127.0.0.1:8000.

### 5. Access the Interface
Open the index.html file in any modern web browser to begin interacting with the agent.

API Reference
Chat Endpoint
Interacts with the AI model.

URL: /chat

Method: POST

Content-Type: application/json

Request Body:

{
  "message": "What are the documents required for a Japan tourist visa?"
}

Success Response (200 OK):

{
  "response": "To apply for a Japan tourist visa, you typically need: 1. A valid passport..."
}
