# CRM Audio Call Report Automation

**End-to-end automation for CRM call quality audits using FastAPI, OpenAI Whisper & GPT, and Google Workspace**

---

## 🚀 What Does This Project Do?

This system automates CRM call quality reporting by:

- Downloading customer call recordings from Google Drive
- Transcribing audio calls (MP3) with OpenAI Whisper
- Generating structured, expert-level call audit reports using OpenAI GPT-4
- Storing and linking PDF reports back to Google Sheets for easy access
- Managing the entire workflow from Google Sheets with Apps Script integration

---

## 🧰 Tech Stack

- **Backend**: FastAPI (Python)
- **AI**: OpenAI Whisper (Speech-to-Text), OpenAI GPT-4 (Report Generation)
- **Google APIs**: Google Drive, Google Sheets, Google Docs
- **Automation**: Google Apps Script (GAS)
- **PDF Generation**: Google Docs + Drive API
- **Deployment**: Cloud Run (or any cloud VM), fully containerized

---

## 🌟 Why is this Cool?

- **No more manual call audits!**  
  The CRM team can process 10x more calls, with objective, high-quality reporting.
- **Truly end-to-end:**  
  From audio file to actionable PDF in Google Drive—fully automated.
- **Seamless with Google Workspace:**  
  Built for teams using Google Sheets, Drive, Docs.
- **Modern LLM stack:**  
  Uses state-of-the-art AI for both speech-to-text and audit analysis.

---

## 📸 Demo

*![image](https://github.com/user-attachments/assets/c10b4912-8a39-4d64-970a-b15fb666836b)
*

---

## 🛠️ How to Use

### 1. Clone and Setup Backend

```bash
git clone https://github.com/YOUR_USERNAME/crm-audio-call-report-automation.git
cd crm-audio-call-report-automation
pip install -r requirements.txt
# Add your .env with OPENAI_API_KEY and GOOGLE_APPLICATION_CREDENTIALS
uvicorn main:app --reload
