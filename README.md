# Ayla Career Assistant

A personal AI-powered career assistant web app built to automate and improve my job search. Upload unlimited CVs and cover letters, generate tailored applications for any job description, write cold emails, and track every application — all in one single HTML file powered by the Claude API.

---

## Features

### 📄 Document Library
- Upload unlimited CVs, cover letters, and job descriptions
- Drag and drop support
- Filter documents by type
- Select specific documents as reference material when generating applications

### ✨ CV & Cover Letter Generator
- Paste any job description and generate a fully tailored CV or cover letter
- Selects relevant experience, skills, and keywords automatically
- Optimised for ATS (Applicant Tracking Systems)
- Outputs in my natural writing voice — not generic AI text

### ✉️ Cold Email Writer
- Generate outreach emails for internships, work experience, networking, follow-ups, and recruiter outreach
- Personalised to the company and role
- Concise, professional, and human-sounding

### 📊 Application Tracker
- Log and track every job application
- Status tracking: Applied, Awaiting, Interview, Offer, Rejected, No Response
- Pre-loaded with 30 real applications from my job search
- Add and delete entries directly in the app

### 💬 AI Career Chat
- Open-ended chat assistant that knows my full career profile
- Ask for interview prep, job search advice, application strategy, or anything else

---

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript (single file, no frameworks)
- **AI:** [Claude API](https://www.anthropic.com) (`claude-sonnet-4-20250514`)
- **Fonts:** DM Serif Display, DM Mono, Instrument Sans (Google Fonts)
- **No backend, no database, no build step**

---

## How to Use

### Run locally
1. Download `Ayla_Career_Assistant.html`
2. Open the file in any modern browser
3. The Documents, Tracker, and UI work immediately offline
4. To use the Generate and Chat features, you need an [Anthropic API key](https://console.anthropic.com)

### Add your API key
Open the HTML file in a text editor and find this line near the bottom:

```js
const res = await fetch('https://api.anthropic.com/v1/messages', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
```

Add your key to the headers:

```js
headers: {
  'Content-Type': 'application/json',
  'x-api-key': 'YOUR_API_KEY_HERE',
  'anthropic-version': '2023-06-01'
},
```

> ⚠️ Do not commit your API key to GitHub. If you want to deploy this publicly, use a backend proxy to keep your key secure.

### Deploy as a website (GitHub Pages)
1. Upload the HTML file to a GitHub repository
2. Go to **Settings → Pages**
3. Set branch to `main` and click **Save**
4. Your app will be live at `https://yourusername.github.io/repository-name`

---

## About

Built as part of my job search as a recent BCIS graduate from AUT (Auckland University of Technology), majoring in Networks & Cybersecurity with a minor in Artificial Intelligence. This project demonstrates practical application of AI APIs, frontend development, and real-world problem solving.

**Skills demonstrated:**
- Claude API integration
- Single-page application architecture
- UI/UX design and layout
- Data management with vanilla JavaScript
- Document processing and text extraction

---

## Screenshots

> Coming soon

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

*Built by Ayla Rusdhy · [LinkedIn](https://www.linkedin.com/in/ayla-rusdhy) · aylarusdhy450@gmail.com*
