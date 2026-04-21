# 🏥 Patient History Extractor

An AI-powered chatbot that analyzes patient medical history and extracts key clinical information — built with **LangChain**, **FastAPI**, and **Streamlit**.

---

## ✨ Features

- 📋 Accepts text patient history as input
- 🔍 Extracts structured medical information including:
  - **Last diagnosis**
  - **Known diseases / conditions**
  - **Last recorded blood pressure**
  - **Last recorded blood sugar levels**

- ⚡ Fast REST API backend powered by FastAPI & Uvicorn
- 🧠 LangChain-based NLP pipeline for intelligent extraction

---

## 🛠️ Tech Stack

| Layer     | Technology                          |
|-----------|-------------------------------------|
| Frontend  | Streamlit                           |
| Backend   | FastAPI + Uvicorn                   |
| AI/NLP    | LangChain                           |
| Language  | Python                              |

---

## 📁 Project Structure

```
project-root/
├── backend/
│   ├── main.py          # FastAPI app entry point
│   └── ...              # LangChain chains, models, utilities
├── frontend/
│   ├── streamlit.py     # Streamlit chatbot UI
│   └── ...
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- pip

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/muneerahmad44/Patient-History-Extractor.git
cd Patient-History-Extractor
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```



---

## ▶️ Running the App

You will need **two terminal windows** — one for the backend and one for the frontend.

### Terminal 1 — Start the Backend

```bash
cd backend
uvicorn main:app --reload
```

The API will be available at `http://localhost:8000`.

### Terminal 2 — Start the Frontend

```bash
cd frontend
streamlit run streamlit.py
```

Streamlit will automatically open a new browser tab with the chatbot interface.

---

## 💡 How to Use

1. Open the Streamlit tab in your browser
2. Enter or paste a patient's medical history in the chat input
3. The AI will analyze the text and return a structured summary including:
   - Last diagnosis
   - Known diseases
   - Last blood pressure reading
   - Last blood sugar reading

### Example Input

```
Patient is a 58-year-old male with a history of Type 2 Diabetes and hypertension.
Last visit: March 2024. BP recorded at 145/92 mmHg. Fasting blood sugar: 172 mg/dL.
Diagnosed with early-stage diabetic nephropathy.
```

### Example Output

| Field              | Extracted Value              |
|--------------------|------------------------------|
| Last Diagnosis     | Early-stage diabetic nephropathy |
| Diseases           | Type 2 Diabetes, Hypertension |
| Last Blood Pressure| 145/92 mmHg                  |
| Last Blood Sugar   | 172 mg/dL (fasting)          |

---

## 🔧 API Reference

Once the backend is running, interactive API docs are available at:

- Swagger UI: `http://localhost:8000/docs`
- ReDoc: `http://localhost:8000/redoc`




## 👨‍💻 Author

Built with ❤️ using LangChain, FastAPI, and Streamlit.

