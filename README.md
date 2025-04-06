

CyberGuard AI - National Cyber Crime Reporting Portal
🌟 Overview
CyberGuard AI is a cutting-edge platform designed to revolutionize the way cybercrime complaints are reported, tracked, and managed. By harnessing the power of artificial intelligence—specifically Google’s Gemini AI—this platform offers an intuitive and secure interface for users to submit and monitor cybercrime complaints. Built with Streamlit for a user-friendly frontend and Supabase for secure data management, CyberGuard AI ensures that every complaint is processed efficiently, categorized accurately, and handled with the utmost care for user privacy and security.
Key Benefits
•	AI-Driven Categorization: Automatically classifies complaints using advanced AI, ensuring swift and accurate processing.
•	User-Friendly Interface: Simplifies complaint submission with an intuitive design and support for multiple input methods (text, voice, files).
•	Secure and Private: Protects sensitive user data with end-to-end encryption and compliance with privacy regulations.
•	Real-Time Tracking: Provides transparency with real-time updates on complaint status.
CyberGuard AI is more than just a reporting tool—it's a comprehensive solution empowering individuals and authorities to combat cybercrime effectively.
________________________________________
🔑 Features
CyberGuard AI offers a robust set of features to streamline the cybercrime reporting process:
•	Secure User Authentication: Protects access with Supabase Auth, supporting multi-factor authentication (MFA).
•	Flexible Complaint Submission: Submit complaints via text, voice recordings, or file uploads, with multi-language support.
•	AI-Powered Categorization: Leverages Google Gemini AI to categorize complaints (e.g., Cyber Harassment, Financial Fraud) accurately.
•	Real-Time Complaint Tracking: Monitor complaint status updates instantly using a unique ticket ID.
•	Secure Data Management: Stores data in Supabase with encryption, 
•	User Dashboard: Centralized interface to manage complaints, view statuses, and access support resources.
•	Multi-Language Support: Enhances accessibility for users worldwide.
These features combine to deliver a powerful, accessible, and secure platform for addressing cybercrime.
________________________________________


🚀 Workflows
CyberGuard AI revolves around two core workflows: Complaint Submission and Complaint Tracking, designed for simplicity and efficiency.
Complaint Submission Workflow
1.	Log In: Access the platform with secure credentials.
2.	Select Language: Choose your preferred language for the interface.
3.	Choose Input Method: 
o	AI Chatbot: Answer guided questions via a conversational interface powered by NLP.
o	Manual Form: Fill out a structured form with complaint details.
4.	Provide Details: Submit text, voice recordings, or files (e.g., screenshots).
5.	Review and Submit: Confirm accuracy and send the complaint.
6.	Receive Ticket ID: Get a unique ID for tracking.
Complaint Tracking Workflow
1.	Log In: Sign into your account.
2.	Navigate to Track Complaint: Access the tracking section from the dashboard.
3.	Enter Ticket ID: Input your unique ID.
4.	View Status: Check real-time updates (e.g., "Under Review," "Resolved").

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

