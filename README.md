

# Apna Sehat – Smart Health Assistance Platform

## Introduction
Apna Sehat is an AI-powered health assistance platform designed to help users
access medical insights, blood transfusion recommendations, digital reports,
hospital locators, and emergency support. This project integrates NLP, ML,
and secure backend systems to provide a complete healthcare ecosystem.

## Team Members (6 Members)
1. Abhishek – Frontend (React)
2. Anuj – Backend (API/DB)
3. Aditya – UI/UX
4. Sidharth – ML Model
5. Ojas – NLP Extraction
6. Dhruv – Testing

## Repository Structure

-  apna-sehat/
- │
- ├── frontend/
- ├── backend/
- ├── ml/
- ├── nlp/
- ├── testing/
- └── docs/

## System Design  


--                         ┌───────────────────────────────┐
--                         │        Users (Patients)        │
--                         │  - Symptom input               │
--                         │  - Report upload               │
--                         │  - Multilingual UI             │
--                         └───────────────┬───────────────┘
--                                         │
--                                         │
--                         ┌───────────────▼───────────────┐
                           │        Frontend Layer          │
                           │    React / Flutter App         │
                           │  - UI/UX                       │
                           │  - Language switcher           │
                           │  - Form validation             │
                           └───────┬───────────┬───────────┘
                                   │           │
            ┌──────────────────────┘           └────────────────────────┐
            │                                                           │
            ▼                                                           ▼
┌──────────────────────┐                                  ┌──────────────────────┐
│  Authentication API   │                                  │ Real-Time API        │
│  (Login/Signup/Auth)  │                                  │ (Chat, Video, Calls) │
└───────────┬──────────┘                                  └──────────┬──────────┘
            │                                                           │
            ▼                                                           ▼
      ┌───────────────────────────────────────────────────────────────────────────┐
      │                             Backend Layer (API)                            │
      │                        Node.js + Express / Flask                           │
      │  ┌────────────────────────┬────────────────────────────┬──────────────────┐│
      │  │       Routing          │     Business Logic         │  Access Control  ││
      │  │  (REST Endpoints)      │  (Handling workflows)      │  (JWT/OAuth2)    ││
      │  └────────────────────────┴────────────────────────────┴──────────────────┘│
      └───────────────────────┬────────────────────────────────────────────────────┘
                              │
                              │
                 ┌────────────▼─────────────┐
                 │   AI Diagnosis Engine     │
                 │ PyTorch (Cloud) + TFLite  │
                 │ ───────────────────────── │
                 │  • Symptom extraction     │
                 │  • Data preprocessing     │
                 │  • Condition prediction   │
                 │  • Severity scoring       │
                 └────────────┬─────────────┘
                              │
                              ▼
                 ┌────────────────────────────┐
                 │  Decision Engine (Rules)   │
                 │ ───────────────────────────│
                 │  • Green Zone  (Low risk)  │
                 │  • Yellow Zone (Moderate)  │
                 │  • Red Zone    (High risk) │
                 └────────────┬──────────────┘
                              │
                              ▼
              ┌────────────────────────────────────┐
              │   Encrypted Database (MongoDB)      │
              │ ─────────────────────────────────── │
              │  • User Profiles                    │
              │  • Symptoms & Reports               │
              │  • AI Outcomes                      │
              │  • Appointments                     │
              │  • Doctor Records                   │
              └───────────────────┬────────────────┘
                                  │
                                  ▼
                     ┌───────────────────────────────┐
                     │   Cloud & DevOps Layer        │
                     │ ───────────────────────────── │
                     │  • MongoDB Atlas              │
                     │  • CI/CD (GitHub Actions)     │
                     │  • Dockerized microservices   │
                     │  • AWS / GCP Deployed APIs    │
                     └───────────────────────────────┘







## Branching Strategy
- `main` → Stable production-ready code  
- `dev` → All team features merged  
- Feature branches:
  - `frontend-abhishek`
  - `backend-anuj`
  - `ui-aditya`
  - `ml-Sidharth`
  - `nlp-Ojas`
  - `testing-Dhruv`

## Contribution Workflow
1. Pull latest from `dev`
2. Work in your feature branch
3. Push changes
4. Create Pull Request → dev
5. Team lead merges to main weekly

## Tech Stack
- React / HTML / CSS  
- Flask / Node.js  
- Python (NLP, ML)  
- MongoDB / MySQL  
- GitHub for version control  

## License
This project is for academic use.

