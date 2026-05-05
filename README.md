# QA-Technical-Assignment
A complete QA test suite , built as part of a QA Engineer technical assignment. Includes a structured Postman collection with automated test scripts, a Google Sheets test case management system.

## 📁 Repository Structure
 
```
gemini-api-qa/
├── postman/
│   ├── Gemini_API_QA_Test_Suite.postman_collection.json
│   └── Gemini_API_QA_Environment.postman_environment.json
│  
└── README.md
```
 
---
 
## 🧪 What Is Being Tested
 
**API:** Google Gemini `generateContent`  
**Base URL:** `https://generativelanguage.googleapis.com/v1beta`  
**Model:** `gemini-2.5-flash, gemini-flash-latest`  
**Auth:** API Key (query parameter)
 
---
## 📋 Test Coverage — 13 Requests, 5 Folders
 
| Folder | Requests | What It Covers |
|---|---|---|
| Happy Path | 2 | Valid requests, Available models |
| Validation Errors | 3 | Bad input, empty prompts, invalid model |
| Error States | 3 | Missing API key,Wrong API key, malformed JSON |
| Idempotency | 2 | Repeated requests return consistent structure |
| AI Output Quality | 3 | Response content, safety ratings, relevance |
 
---
 
## 🚀 How To Run
 
### Prerequisites
```bash
npm install -g newman
```
 
### Add your API key
Open `postman/QA_testing_Assignment.postman_environment.json` and replace:
```json
{ "key": "api_key", "value": "YOUR_GEMINI_API_KEY_HERE" }
```
 
### Run the collection
```bash
newman run newman run ".\QA_Testing_Assignment.postman_collection.json" -e ".\QA_testing_Assignment.postman_environment.json"
  
```
**Screen Recording:** [Video](https://drive.google.com/file/d/1w46GISOIPzWf2qH_qw838Xw6re-awDy5/view?usp=drive_link)    
**Google Sheets:** [Sheet Link](https://docs.google.com/spreadsheets/d/1LbLb9LCeGCNEpT_yGI23lUW3hkqjb0zFUshbtln66NQ/edit?usp=sharing)
---
 
 
## 👤 Author
 
**Vimal Singh Panwar**  
Date: 05/05/2026
