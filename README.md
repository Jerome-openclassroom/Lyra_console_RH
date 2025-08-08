# 🤖 Lyra_Console_RH — AI Recruitment Assistant (RAG + OpenAI)

![Made with Gradio](https://img.shields.io/badge/Made%20with-Gradio-ff6b6b?logo=gradio)
![OpenAI Assistant](https://img.shields.io/badge/OpenAI-Assistant_API-01a982?logo=openai)
![License MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Language](https://img.shields.io/badge/Python-3.10+-blue?logo=python)


**Lyra_Console_RH** is a lightweight AI-based human resources assistant that simulates the behavior of a responsive, intelligent tool for recruiter.  
It combines OpenAI Assistants API, persistent thread memory, retrieval-augmented generation (RAG), and a Gradio interface.

---

## 🚀 Key Features

- 🧠 **OpenAI Assistant with RAG**: Connects to a vector store built from README files covering AI, ecology, meteorology, and agronomy projects.
- 🧾 **Persistent Memory**: Uses a fixed `thread_id` to ensure conversation continuity and historical awareness.
- 🪄 **Natural Email Generation**: Generates personalized emails based on context and candidate data.
- 🎛️ **Interactive Console**: Simple Gradio UI simulating a virtual HR office.
- 🔐 **API Key Isolation**: Uses a local `.env` text file for secure API usage (`ENV/env.txt`).

---

## 📦 How to Use

### 1. Clone the repository

```bash
git clone https://github.com/Jerome-openclassroom/Lyra_Console_RH.git
cd Lyra_Console_RH
```

### 2. Set up your API key

Create a file named `env.txt` inside the `ENV/` folder with the following content:

```
OPENAI_API_KEY=sk-XXXXXXXXXXXXXXXXXXXXXXXX
```

### 3. Launch the console

```bash
python lyra_console_rh.py
```

The interface will open locally using [Gradio](https://www.gradio.app/).

---

## 📬 Example Use Case

**User prompt:**
```
Peux-tu me rédiger un mail de réponse à l'attention de Jérôme FRASSON sollicitant un échange suite à sa candidature spontanée ?
```

**AI-generated output:**
> *"We would be delighted to schedule a conversation with you to discuss potential collaboration opportunities based on your experience in ecological modeling and open-source AI integration..."*

👉 Email is ready to copy-paste, contextual, and aligns with the candidate’s background.

---

## 📚 Vector Store Corpus

Documents used in the RAG system include:

- 10+ README files from [Jerome's repositories](https://github.com/Jerome-openclassroom)
- Topics: AI workflows, ecological diagnostics, fine-tuning, environmental datasets

---

## 🧪 Technologies Used

- [OpenAI Assistant API](https://platform.openai.com/)
- Python 3.10+
- Gradio
- `.env` file management (manual)
- Retrieval with built-in OpenAI vector store

---

## 📂 Folder Structure

```
📁 Lyra_Console_RH/
├── 📄 README.md                   # Main README (English)
├── 📄 README_Lyra_Console_RH_FR.md  # French version of the README
├── 📄 requirements.txt            # Minimal Python dependencies
│
├── 📁 code/                       # Source code (Notebook)
│   └── Lyra_RH_console.ipynb      # Interactive HR console using OpenAI Assistant + Gradio
│
├── 📁 screenshots/                # Illustrative screenshots
│   ├── prompting_console.png      # Prompt input area with UI
│   ├── questions_list.png         # Example of assistant listing previous questions
│   └── Reply_mail.png             # Example of AI-generated HR email

```

## 🔄 Related Projects

🔗 Also check out the n8n version of the recruiter agent: [Lyra_Recruiter_Agent_n8n](https://github.com/Jerome-openclassroom/Lyra_Recruiter_Agent_n8n)  

🔗 Or explore the Make.com version integrated into a full AI scenario: [Lyra_Recruiter_Agent_Make](https://github.com/Jerome-openclassroom/Lyra_Recruiter_Agent_Make)

## 🧠 Author

**Jérôme Frasson**  
GitHub: [@Jerome-openclassroom](https://github.com/Jerome-openclassroom)  
Email: jerome.frasson.vsi@gmail.com  
Focus: AI × Environment × Agent-based workflows

---

## 📝 License

This project is open-source and intended for educational, research, and personal use.  
Re-use encouraged under proper attribution.
