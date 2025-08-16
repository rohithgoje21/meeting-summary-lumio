# AI-Powered Meeting Notes Summarizer and Sharer

This project is a full-stack web application that allows users to input meeting transcripts and receive summarized notes powered by Hugging Face's BART model. The summarized notes can then be emailed directly using Nodemailer.

## 🚀 Features

- ✅ Summarizes long meeting transcripts using Hugging Face Transformers (BART model)
- ✅ Sends the summary via email using Gmail SMTP and Nodemailer
- ✅ CORS and dotenv support for clean development
- ✅ Deployed-ready structure (for platforms like Railway, Vercel, etc.)

## 🛠️ Tech Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Node.js, Express
- **AI Integration**: Hugging Face Transformers API (BART)
- **Email Service**: Nodemailer (Gmail SMTP)
- **Other**: CORS, dotenv, node-fetch

## 🧾 Setup Instructions

1. Clone the Repository
```bash
git clone https://github.com/rohithgoje21/meeting-summary-lumio.git
cd meeting-summary-lumio
```

2. Install Dependencies
```bash
npm install
```

3. Set Environment Variables

Add the following in .env file.
```bash
HUGGINGFACE_API_KEY=your_huggingface_api_key
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password_or_2fa_token
```
4. Run the Server
```bash
node index.js
```

5. Access the App
6. Navigate to http://localhost:5000 (or your assigned port) and test the meeting summarization and email functionality.


📄 Sample Prompt Format
```bash
[Meeting Transcript]
Sarah: We completed the frontend redesign...
Mike: Backend authentication integration is done...
```
📧 Email Output
```bash
Receiver gets an email with the subject “Meeting Summary”
Email body contains the summarized notes
```
