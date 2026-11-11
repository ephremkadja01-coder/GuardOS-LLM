# GuardOS LLM

## Overview
GuardOS LLM is a security middleware (an asynchronous application proxy) designed to intercept, analyze, and secure JSON data flows between internal applications and Large Language Models (LLMs).

The system provides defense against injection attacks (Jailbreak, homoglyphs, semantic mutations) and ensures compliance through the anonymization of personal data.

## FoxCommit Team
- **Ephrem K.** : Project Manager and Offensive Security Analyst (Red Team, Initial Architecture)
- **Soulymane** : Defensive Security Engineer (Blue Team, Text Normalization)
- **Masso** : Infrastructure and Flow Architect (Data Scientist, Server and Database)
- **Djafarou** : Governance and Compliance Expert (AI Safety, Anonymization)

## Repository Architecture
- `docs/` : Technical documentation and specifications.
- `data/` : Static dictionaries and configuration files.
- `scripts/` : Automation scripts and execution entry points.
- `src/` : Modular application source code.
- `tests/` : Unit and non-regression test suites.

## Installation
1. Create a virtual environment:
   `python -m venv venv`
2. Activate the virtual environment:
   - Windows: `venv\Scripts\activate`
   - Mac/Linux: `source venv/bin/activate`
3. Install dependencies:
   `pip install -r requirements.txt`
4. Configure environment variables:
   `cp .env.example .env`

## Execution
The project will be launched via dedicated scripts located in the `scripts/` folder. The team will work in isolation on their respective modules before the final pipeline integration.