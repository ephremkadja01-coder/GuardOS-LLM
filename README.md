# GuardOS LLM

## Project Overview
GuardOS LLM is a security middleware (an asynchronous application proxy) designed to intercept, analyze, and secure JSON data flows between internal applications and Large Language Models (LLMs). The system provides defense against injection attacks (Jailbreak, homoglyphs, semantic mutations) and ensures compliance through the anonymization of personal data.

## FoxCommit Team
- Ephrem K. : Project Manager and Offensive Security Analyst (Red Team, Core Architecture)
- Soulymane : Defensive Security Engineer (Blue Team, Text Normalization)
- Masso : Infrastructure and Flow Architect (Data Scientist, Server and Database)
- Djafarou : Governance and Compliance Expert (AI Safety, Anonymization)

---

## 1. Prerequisites
Before cloning the project, ensure you have the following installed on your machine:
- Git: For version control.
- Python 3.10+: For running the application.
- A Code Editor: Such as VS Code, PyCharm, or Cursor.

## 2. How to Get the Project (Team Onboarding)
Follow these exact steps to set up the project on your local machine.

Step 1: Clone the Repository
Open your terminal (or Git Bash on Windows) and run:
git clone https://github.com/ephremkadja01-coder/GuardOS-LLM.git
cd GuardOS-LLM

Step 2: Create a Virtual Environment
It is highly recommended to use a virtual environment to avoid dependency conflicts.
Windows:
python -m venv venv
venv\Scripts\activate

Mac/Linux:
python3 -m venv venv
source venv/bin/activate
(You should see (venv) appear at the beginning of your terminal prompt).

Step 3: Install Dependencies
Install all required open-source libraries defined in the requirements file:
pip install -r requirements.txt

Step 4: Configure Environment Variables
Copy the example environment file to create your local .env file:
Windows:
copy .env.example .env

Mac/Linux:
cp .env.example .env

## 3. Development Workflow (Git Rules)
To avoid conflicts and ensure a smooth integration, every team member must follow this strict Git workflow:

1. Always pull the latest changes before starting to code:
git pull origin main

2. Create your own working branch:
- Masso: git checkout -b masso/infrastructure
- Soulymane: git checkout -b soulymane/defense
- Djafarou: git checkout -b djafarou/safety
- Ephrem: git checkout -b ephrem/core

3. Work only inside your assigned folder.

4. Commit your changes regularly:
git add .
git commit -m "feat(module_name): Clear description of what you did"

5. Push your branch to GitHub:
git push origin your_branch_name

6. Create a Pull Request (PR) on GitHub when a feature is ready to be merged into main.

## 4. Repository Architecture
- docs/ : Technical documentation, architecture diagrams, and API specifications.
- data/ : Static dictionaries and JSON configuration files (homoglyphs, regex patterns).
- scripts/ : Automation scripts to launch the server or run offensive tests.
- src/ : The core source code.
  - src/core/ : Red Team modules (Fuzzing engine, attack console).
  - src/defense/ : Blue Team modules (Text normalization, Unicode parsing).
  - src/infrastructure/ : Server routing, asynchronous pipeline, and database.
  - src/safety/ : Anonymization rules, PII masking, and compliance checks.
  - src/ui/ : Streamlit dashboard and user interface.
- tests/ : Pytest unit and integration test suites.

## 5. Running the Application
Note: This will be updated as the project progresses.

To run the local server:
bash scripts/run_server.sh

To launch the offensive fuzzing console:
python scripts/run_fuzzer.py

## 6. Validation and Testing
Before submitting a Pull Request, ensure your code passes the unit tests:
pytest tests/