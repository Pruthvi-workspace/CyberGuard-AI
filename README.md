

---

```markdown
<h1 align="center">CyberGuard AI 🚨🧠</h1>

<p align="center">
  <i>“AI-powered Cybercrime Complaint Portal for Safer Digital India”</i><br><br>
  <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Streamlit-Framework-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Gemini%20AI-Google-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Supabase-Database-green?style=for-the-badge" />
</p>

---

## 🧠 Project Title

**CyberGuard AI: National Cybercrime Reporting Portal using Gemini AI + Streamlit + Supabase (Multi-language NLP, Voice + File input)**

---

## 🛡️ Overview

CyberGuard AI is a powerful and secure platform that enables citizens to report cybercrimes in multiple Indian languages using text, voice, or document uploads. The app uses Gemini AI for NLP-based categorization, and Supabase as a backend service for authentication, storage, and complaint tracking. The solution ensures accessibility, transparency, and ease of use — all through a single Python file (`app.py`).

---

## 💥 Key Features

- ✅ Submit complaints in 22 Indian languages via **text, voice (STT)**, or **file uploads (PDF/Images)**
- ✅ **AI categorization** of complaint type using Google Gemini NLP
- ✅ Real-time complaint **ticket generation and tracking**
- ✅ Multilingual **confirmation email** with official ticket number
- ✅ Built-in **speech-to-text**, **OCR**, and **language translation**
- ✅ Admin dashboard for **status update**, **ticket view**, and **filters**
- ✅ Streamlit UI with **tabs**, **themed display**, and **structured workflows**
- ✅ Supabase: secure backend for data storage, auth, and ticket logs
- ✅ OTP login (optional), email notifications (optional), single-file app

---

## 🌍 Supported Indian Languages (22)

Hindi, Konkani, Kannada, Dogri, Bodo, Urdu, Tamil, Kashmiri, Assamese, Bengali, Marathi, Sindhi, Maithili, Punjabi, Malayalam, Manipuri, Telugu, Sanskrit, Nepali, Santali, Gujarati, Odia.

---


## 🏗️ App Architecture

```mermaid
flowchart TB
    A[User Input<br>(Text/Voice/File)] --> B[Preprocessing]
    B --> C[Language Detection<br>& Translation]
    C --> D[Gemini AI<br>Classification]
    D --> E[Supabase Storage]
    E --> F[Email Notification<br>with Ticket ID]
    F --> G[Track Complaint Status]
```

---

## ⚙️ Technologies Used

| Component      | Stack Used          |
|----------------|---------------------|
| Frontend       | Streamlit (Python)  |
| AI/NLP Engine  | Gemini API          |
| Database       | Supabase  |
| File Parsing   | pytesseract, pdfminer |
| Voice Input    | speech_recognition   |
| Email Service  | SMTP / Supabase Mail |
| Translation    | gemini       |
| Others         | dotenv, requests, uuid |

---

## 📁 Folder Structure

```
CyberGuard-AI/
│
├── app.py                 # Main app file with all logic (Streamlit)
├── .env                  # Stores API keys and Supabase secrets
├── requirements.txt       # Python dependencies
├── helpers/
│   ├── nlp_utils.py       # Gemini AI classification functions
│   ├── lang_utils.py      # Language detection + translation
│   ├── file_parser.py     # OCR + PDF parsing
│   ├── audio_parser.py    # Voice input handling
│   └── supabase_client.py # Auth + storage functions
├── assets/
│   ├── logo.png           # Logo for UI
│   └── sample_uploads/    # Sample complaint docs
```

---

## 🛠️ How to Run

```bash
git clone https://github.com/your-username/CyberGuard-AI.git
cd CyberGuard-AI
pip install -r requirements.txt
streamlit run app.py
```

Make sure to add your credentials in a `.env` file:

```
SUPABASE_URL=...
SUPABASE_KEY=...
GEMINI_API_KEY=...
```

---

## 📊 Complaint Workflow

1. User visits the portal
2. Enters complaint via:
   - Text
   - Voice (converted to text)
   - File (image/PDF converted to text via OCR)
3. Language is auto-detected and translated to English
4. Gemini AI processes and classifies the complaint
5. Data is stored securely in Supabase
6. User receives ticket number + confirmation in original language
7. User can track complaint using ticket ID

---

________________________________________
🔌 API Integrations
•	Google Gemini AI: Categorization and NLP.
•	Supabase: Database, authentication, and storage.
•	SpeechRecognition: Voice-to-text conversion (optional).
•	gTTS: Text-to-speech (optional).
•	ReportLab: PDF report generation.
These integrations drive the platform’s core capabilities.
________________________________________
🌐 Deployment Options
Streamlit Cloud
1.	Push to GitHub: Upload code to a GitHub repository.
2.	Connect to Streamlit Cloud: Link your repo in the Streamlit Cloud dashboard.
3.	Configure Secrets: Add API keys (e.g., Supabase, Gemini) securely.
4.	Deploy: Launch the app with one click.
Alternative options include Docker or VPS deployment for custom setups.


## 🔗 Links


- 🎬 [Demo Video on Google Drive](https://drive.google.com/drive/folders/1DyI5qzy40ks3LV69vTq5YpW-f8gLjbCL)




<p align="center">
  Built for 🇮🇳 India | Empowering citizens against digital crime 💻🔒
</p>
```

