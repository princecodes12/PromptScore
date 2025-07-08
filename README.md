# 🚀 PromptScore

PromptScore is a full-stack web application that evaluates user prompts and offers constructive feedback using LLMs such as OpenAI's GPT. It provides an overall score, detailed sub-scores, and upgraded versions of prompts to help users write better, clearer, and more effective prompts for AI.

---

## 🔍 Features

- ✍️ **Prompt Analysis**: Analyze user prompts using OpenAI API or a custom LLM.
- 📊 **Sub-score Breakdown**: Includes Clarity, Specificity, and Completeness.
- 🧠 **Prompt Suggestions**: Suggests upgraded versions of submitted prompts.
- 🗃️ **Prompt History**: Stores prompt results in a PostgreSQL database.
- 🌐 **Frontend**: Built in React with clean UI and real-time feedback.
- 🛠 **Backend**: Built with Spring Boot to manage API and business logic.
- 🔗 **LLM Microservice**: FastAPI service for LLM integration.
- ☁️ **Database**: Uses Railway-hosted PostgreSQL to manage users and prompts.

---

## 🧱 Tech Stack

| Layer       | Technology                         |
|-------------|-------------------------------------|
| Frontend    | React, Tailwind CSS                 |
| Backend     | Spring Boot (Java), REST APIs       |
| LLM Service | Python FastAPI, OpenAI API          |
| Database    | PostgreSQL (via Railway)            |
| Tools       | IntelliJ IDEA, Postman, Git, Maven  |

---

## 🧠 Sub-score Categories

Each prompt is evaluated on the following dimensions:

- **Clarity** – How clearly the intent is expressed
- **Specificity** – How detailed and well-targeted the prompt is
- **Completeness** – Whether the prompt includes all necessary information

---

## 🔧 Project Structure

PromptScore/
├── backend/ # Spring Boot project (API, DB, business logic)
├── frontend/ # React UI
└── llm-service/ # FastAPI microservice for LLM integration


## Run the Backend
cd backend
./mvnw spring-boot:run

## Run the Fronend
cd frontend
npm install
npm start

# Run the LLM Microservices(Python + FastAPI)
cd llm-service
pip install -r requirements.txt
uvicorn app:app --reload
