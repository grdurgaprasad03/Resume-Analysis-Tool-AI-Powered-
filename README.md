# 📄 Resume Analysis Tool (AI-Powered)

An AI-powered **Resume Screening & Evaluation System** built using **LangChain, Gemini (Google GenAI), and Streamlit**.
This tool analyzes a candidate’s resume against a job description and provides a structured hiring decision like a real recruiter.

---

## 🚀 Features

* ✅ **Skill & Education Matching**
* ✅ **Experience Evaluation**
* ✅ **Salary Market Estimation**
* ✅ **Final Hiring Decision (Approve/Reject)**
* ✅ **Structured Recruiter-style Output**
* ✅ **PDF Resume & JD Upload Support**
* ✅ **Interactive UI using Streamlit**

---

## 🧠 How It Works

The system uses a **multi-agent architecture**:

### 🔹 1. Skill & Education Agent

* Compares resume skills with job requirements
* Identifies missing skills
* Uses Wikipedia for concept validation

### 🔹 2. Experience Agent

* Evaluates:

  * Years of experience
  * Role relevance
  * Companies and domains
* Uses web search for context

### 🔹 3. Salary Agent

* Estimates market salary range
* Suggests expected hike %
* Provides confidence level

### 🔹 4. Supervisor Agent (Main Decision Maker)

* Combines all insights
* Outputs:

  * ✅ Decision (APPROVE / REJECT)
  * 📊 Score (0–100)
  * 📝 Summary
  * 📌 Skill, Experience & Salary Fit

---

## 🛠️ Tech Stack

* **Python**
* **Streamlit** – UI
* **LangChain** – Agent orchestration
* **Google Gemini (2.5 Flash Lite)** – LLM
* **DuckDuckGo Search Tool**
* **Wikipedia API**
* **PyPDFLoader** – PDF parsing
* **Pydantic** – Structured output

---

## 📂 Project Structure

```
📁 resume-analyzer/
│── app.py                 # Main Streamlit app
│── .env                   # API keys
│── requirements.txt       # Dependencies
│── README.md              # Documentation
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/resume-analyzer.git
cd resume-analyzer
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Add Environment Variables

Create a `.env` file:

```env
gemini_key=YOUR_GOOGLE_GEMINI_API_KEY
```

---

## ▶️ Run the App

```bash
streamlit run app.py
```

---

## 📊 Output Example

```
Decision: APPROVE
Score: 82/100

Summary:
Strong candidate with relevant backend and data skills.

Skill Fit:
MATCH: 85%
MISSING: [Docker, Kubernetes]

Experience Fit:
FIT: 80%
ROLES: [Software Engineer]

Salary Fit:
RANGE: 8 - 14 LPA
CONFIDENCE: MEDIUM
```

---

## 📌 Use Cases

* HR Resume Screening Automation
* Job Application Filtering
* Candidate Self-Evaluation
* Placement Preparation Tool

---

## ⚠️ Limitations

* Depends on resume text quality (PDF parsing)
* Salary estimates are approximate
* Requires internet for search tools
* LLM responses may vary slightly

---

## 🔮 Future Improvements

* 🔍 ATS keyword scoring
* 📊 Resume ranking dashboard
* 🧾 Support for DOCX resumes
* 🌍 Multi-language support
* 📈 Candidate comparison feature


## 📜 License

This project is open-source and available under the **MIT License**.

---

## 💡 Author

Developed by **Durgaprasad G R**

App Link:https://32nunmea6ilbypajxxcsox.streamlit.app/
