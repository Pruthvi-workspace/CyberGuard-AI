
🌐 CyberGuard AI – National Cyber Crime Reporting Portal
________________________________________
🌟 Overview
CyberGuard AI is a next-gen platform that simplifies and secures the process of reporting cybercrimes. Powered by Google Gemini AI and built using Streamlit and Supabase, it ensures that every complaint is categorized intelligently, tracked in real-time, and stored with full privacy compliance.
🔑 Key Benefits
•	AI-Driven Categorization – Automatically detects and classifies complaints using Gemini AI.
•	User-Friendly Interface – Submit reports via text, voice, or file uploads with multilingual support.
•	Secure & Private – End-to-end encryption and GDPR/CCPA compliant.
•	Real-Time Tracking – Get live updates on your complaint status using a unique ticket ID.
CyberGuard AI is not just a tool—it’s a digital guardian for cybercrime victims.
________________________________________
🔐 Features
•	Secure User Authentication – Supabase Auth with MFA and OAuth.
•	Multi-Mode Complaint Submission – Via chatbot, manual form, or voice input.
•	AI-Powered Categorization – Classifies types like Phishing, Harassment, etc.
•	Complaint Tracking – Track progress via dashboard using ticket ID.
•	Data Encryption & Compliance – GDPR, CCPA, AES-256 at rest, TLS 1.3 in transit.
•	Multilingual UI – Supports submission in 22 regional Indian languages.
•	PDF Confirmation Reports – Automatically generated using ReportLab.
________________________________________
🚀 Workflows
Complaint Submission
1.	Login
2.	Select Language
3.	Choose Input Method
o	AI Chatbot
o	Manual Form
4.	Submit Details
o	Text, Voice, or File Upload
5.	Receive Ticket ID
6.	Track via Dashboard
Complaint Tracking
1.	Login
2.	Navigate to 'Track Complaint'
3.	Enter Ticket ID
4.	View Real-Time Status
📊 Text-Based Diagram:
[User] --> [Login] --> [Select Language] --> [Input Method: Chatbot/Form] --> [Submit Details] --> [Ticket ID] --> [Track Status]
________________________________________
💻 Technology Stack
•	Frontend: Streamlit
•	Backend: Python (FastAPI/Flask)
•	AI: Google Gemini AI
•	Database: Supabase (PostgreSQL + Auth)
•	Voice Input: SpeechRecognition, pyaudio
•	PDF Generation: ReportLab
•	Text-to-Speech: gTTS (optional)
________________________________________
🏗️ Architecture
+--------------------+
| Client Layer       | (Streamlit UI)
+--------------------+
           ↓
+--------------------+
| API Layer          | (Python - FastAPI)
+--------------------+
           ↓
+--------------------+
| Processing Layer   | (Google Gemini AI)
+--------------------+
           ↓
+--------------------+
| Data Storage Layer | (Supabase DB)
+--------------------+
________________________________________
📝 Usage Guide
Submit a Complaint
1.	Login
2.	Select Language
3.	Choose Input Method (Chatbot/Form)
4.	Provide Details (Text/Voice/File)
5.	Review and Submit
6.	Note the Ticket ID
Track a Complaint
1.	Login
2.	Go to "Track Complaint"
3.	Enter Ticket ID
4.	View Status Updates
💡 Always save your ticket ID securely.
________________________________________
🛡️ Security & Privacy
•	Encryption: AES-256 at rest, TLS 1.3 in transit
•	Authentication: MFA via Supabase Auth
•	Data Control: Users can delete/anonymize data
•	Compliance: GDPR + CCPA aligned
•	Minimal Data Collection: Only essential information stored
________________________________________
🧠 AI-Powered Intelligence
•	Complaint Categorization – Uses Gemini AI to tag cybercrime types.
•	NLP Understanding – Processes both typed and spoken complaints.
•	Key Info Extraction – Auto-extracts names, dates, keywords.
🔍 Example:
User Input: "Someone emailed me asking for bank details pretending to be SBI."
Gemini Classifies: Phishing
________________________________________
📁 Project Structure
Monolithic Setup – All-in-One app.py
•	Core File: app.py
o	Imports & Config (Supabase, Gemini, SMTP)
o	AI Functions
o	Speech-to-Text Utility
o	Dashboard UI & Logic
o	Session State Handlers
•	Optional Files:
o	requirements.txt
o	.env
o	.gitignore
o	README.md
Database Schema (Supabase SQL)
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  username TEXT UNIQUE NOT NULL,
  password TEXT NOT NULL,
  email TEXT UNIQUE NOT NULL
);

CREATE TABLE complaints (
  id SERIAL PRIMARY KEY,
  ticket_id TEXT UNIQUE NOT NULL,
  data JSONB NOT NULL,
  translated_data JSONB NOT NULL,
  status TEXT NOT NULL,
  date_filed TEXT NOT NULL,
  last_updated TEXT NOT NULL
);
________________________________________
⚙️ Setup Guide
1. Install Dependencies
sudo apt-get install portaudio19-dev   # Linux
brew install portaudio                 # macOS
pip install pyaudio                   # Windows
pip install -r requirements.txt
2. Setup Environment
touch .env
# Add the following
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
SMTP_EMAIL=your_email@example.com
SMTP_PASSWORD=your_smtp_password
GEMINI_API_KEY=your_gemini_api_key
3. Run App
streamlit run app.py
________________________________________
🔌 API Integrations
•	Google Gemini AI – Complaint classification, NLP
•	Supabase – Auth, Database
•	SpeechRecognition – Voice input support
•	gTTS – Voice output (optional)
•	ReportLab – PDF confirmation reports
________________________________________
🌐 Deployment Options
Streamlit Cloud
1.	Push to GitHub
2.	Connect to Streamlit Cloud
3.	Add Secrets (.env values)
4.	Click Deploy
✅ Supports custom Docker or VPS setups too.
________________________________________
## 🔗 Links


- 🎬 [Demo Video on Google Drive](https://drive.google.com/drive/folders/1DyI5qzy40ks3LV69vTq5YpW-f8gLjbCL)

________________________________________
🙏 Acknowledgements
•	Streamlit – UI framework
•	Supabase – Backend-as-a-Service
•	Google Gemini – AI-powered categorization
•	Python Community – Open-source libraries
________________________________________.

