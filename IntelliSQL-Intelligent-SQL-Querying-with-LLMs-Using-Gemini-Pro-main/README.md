**IntelliSQL: Intelligent SQL Querying with Gemini Pro**

IntelliSQL is a revolutionized database querying tool that bridges the gap between natural language and structured data. By leveraging the Gemini 1.5 Flash model, it allows non-technical users to extract insights from a SQLite database using plain English.

**🚀 Features**

**Text-to-SQL Translation:** Converts English questions into precise SQL queries using LLMs.

**Regex Sanitization:** A custom logic layer that cleans AI responses to ensure only valid SQL is executed.

**Interactive Dashboard:** A professional Streamlit interface with dark-mode support and sidebar navigation.

**Secure Configuration:** API keys are managed safely via .env files and python-dotenv.

**Real-time Results:** Instant rendering of database records in structured data tables.

**🛠️ Technology Stack**

Frontend: Streamlit

Backend: Python, Google Generative AI SDK

Database: SQLite

AI Model: Gemini 1.5 Flash

**📂 Project Structure**

Plaintext

IntelliSQL/
├── .venv/                # Virtual environment [cite: 113]
├── Project Files/        # Core application source
│   ├── .env              # Secure API Key storage [cite: 1, 127]
│   ├── app.py            # Streamlit UI & AI Logic [cite: 83, 136]
│   ├── sql.py            # DB Engineering & Seeding [cite: 137]
│   ├── data.db           # SQLite Database [cite: 109]
│   └── requirements.txt  # Project Dependencies [cite: 122]
└── README.md             # High-level Documentation [cite: 57, 83]

**⚙️ Setup & Installation**

**Clone the Repository:**

Bash
eg: git clone https://github.com/rajeevparisa/IntelliSQL-Intelligent-SQL-Querying-with-LLMs-Using-Gemini-Pro.git


**Set up Environment:**

Bash
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
pip install -r "Project Files/requirements.txt"

**Configure API Key:**

Create a .env file in the Project Files directory and add your key:
Plaintext
GOOGLE_API_KEY="your_google_gemini_api_key"

**Initialize Database:**

Bash
python "Project Files/sql.py"
**Run Application:**

Bash
streamlit run "Project Files/app.py"

**👥 Team Members & Roles**

1.Sadam Venkata Sai Chandra Sekhar (Team Leader): AI Specialist & Project Manager 

2.Tadiparthi Gayathri: QA Engineer & Documentation 

3.Shaik Shabbe Afroz: Frontend Developer & UI/UX Designer 

4.Shaik Habeeb: Backend Developer & Data Engineer

**⚠️ Known Issues**

Occasional hallucinations on complex multi-table joins if not specified in the schema.

Requires an active internet connection to reach the Gemini API.
