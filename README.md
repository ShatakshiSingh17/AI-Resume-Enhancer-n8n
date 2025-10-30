# AI Resume Enhancer (n8n Workflow)

This project is an **AI-powered resume enhancement workflow** built using [n8n](https://n8n.io), integrated with OpenAI and Google Drive. It takes your existing resume content and intelligently tailors it to match any job description — formatting it into a polished Google Doc that’s ready to submit.

This tool was designed to help job seekers, especially those in data analytics, customize their resumes with minimal effort.

---

## ✨ Features

- 🧠 Connects with OpenAI API (GPT-4/GPT-3.5) for resume enhancement
- 📄 Formats output into a clean, styled HTML resume
- 📁 Saves the enhanced resume directly to a Google Drive folder
- 📌 Uses dynamic job descriptions and company names for personalized titles
- 🔁 Works as an n8n workflow (modular and scalable)

---

## 🚀 How It Works (Workflow Overview)

1. **Input Resume Content**: Original resume text (from markdown, plain text, or HTML).
2. **Fetch Job Description**: Pull job title and description dynamically or manually.
3. **Send to OpenAI**: Craft a prompt that asks the AI to reformat your resume for that job.
4. **Format HTML Output**: Clean and wrap the AI-enhanced content in styled HTML.
5. **Upload to Google Docs**: Create a new document titled with the company name and date, saved in a chosen Drive folder.

---

## 🛠 Tools & APIs Used

| Tool         | Purpose                                    |
|--------------|--------------------------------------------|
| n8n          | Workflow automation and integration        |
| OpenAI API   | AI-generated resume improvements           |
| Google Docs API | Upload formatted resumes to Drive       |
| JavaScript   | Used in n8n Function/HTML Formatter nodes  |

---

## 🧪 How to Use Locally

### Prerequisites

- Free [n8n account](https://n8n.io)
- OpenAI API key (via [https://platform.openai.com](https://platform.openai.com))
- Google Cloud project with Google Docs API enabled

---

### Setup Steps

1. **Import the Workflow**
   - Download the `Resume Enhancer AI.json` from this repo
   - Go to your n8n dashboard → “Import Workflow” → select the file

2. **Set up Credentials**
   - Google Docs: Connect your Google account inside n8n
   - OpenAI: Add your API key under "Credentials" → OpenAI

3. **Customize Your Prompt (Optional)**
   - Modify the AI prompt inside the `Resume Enhancement` node if needed

4. **Run the Workflow**
   - Provide your resume and job description as inputs
   - Execute the workflow
   - Enhanced resume will be saved to your Google Drive folder

---

## 🖼 Sample Output

Check the sample resume in this repo: [`Resume enhancer.pdf`](./Resume%20enhancer.pdf)

---

## 📌 Project Status

✅ Functional and tested  
🛠️ Can be extended to support:
- LinkedIn job scraping
- Resume keyword optimization
- PDF formatting output (via Google Docs to PDF)

---

## 📄 License

MIT License – feel free to use, adapt, and improve it.
