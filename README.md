# ![EvoDoc Logo](logo.svg)  
# ***AI-Powered Prescription Assistant***  
*(Powered by Google Cloud & Generative AI)*

$EvoDoc$ $is$ $an$ $AI-powered$ $medical$ $assistant$ $that$ $reads$ $handwritten$ $or$ $digital$ $prescriptions,$ $extracts$ $important$ $details$ $using$ $OCR$ $(Google$ $Vision),$ $and$ $explains$ $medications$ $in$ $simple$ $language$ $using$ $LLMs.$

---

![Tech Stack](https://img.shields.io/badge/Frontend-React%20%2B%20Vite-blue?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/Backend-FastAPI-darkgreen?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/Cloud-Google%20Cloud-orange?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/OCR-Google%20Vision-yellow?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/AI-RAG%20%2B%20LLM-purple?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/Database-MongoDB%20%2B%20Vertex_AI-darkred?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/Authentication-Oauth2.0%20%2B%20JWT-darkblue?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/Ocr-Google_Vision_API-white?style=for-the-badge)


---

## ***📖 Overview***

$Doctors$ $often$ $write$ $prescriptions$ $in$ $unreadable$ $handwriting,$ $making$ $it$ $difficult$ $for$ $patients$ $to$ $understand$ $what$ $medicines$ $to$ $take$ $and$ $why.$ $EvoDoc$ $solves$ $this$ $by:$

>- ***Extracting text from prescriptions (handwritten or digital) using OCR***

>- ***Parsing drug names, dosage & instructions using AI***

>- ***Providing human-friendly explanations for each medicine using LLMs***

>- ***Ensuring privacy & security of patient data***

## ***✨ Key Features***

- ***Prescription Upload – Upload prescription as Image (JPG, PNG) or PDF***

- ***OCR Integration – Extract text from handwritten or printed prescriptions***

- ***AI Explanation – Convert medical jargon into plain language using LLMs***

- ***Drug Parsing – Identify medicine names, dosage, and frequency***

- ***Multi-language Support – Explain prescriptions in multiple languages***

- ***RAG Integration – Fetch trusted drug information from reliable sources (avoid hallucinations)***

- ***Secure Data Handling – IAM, OAuth2/JWT, HIPAA-ready approach for patient privacy***

## ***🔥 Tech Stack***

>- $Frontend:$  $React$ $+$ $Vite$
>
>- $Backend:$ $FastAPI$
>
>- $Database:$ $MongoDB$
>
>- $AI/LLM:$ $LangChain, Vertex AI, OpenAI(optional)$
>
>- $OCR:$ $Google$ $Vision$ $API$
>
>- $Vector$ $Database:$ $Vertex AI$
>
>- $Cloud$ $Infrastructure:$ $Google$ $Cloud$ $Platform$
>
>- $Authentication:$ $OAuth2$ $/$ $JWT$

## ***📂 Project Structure***
```
EvoDoc/
├── backend/
│   ├── app/
│   │   ├── main.py                # FastAPI entry point
│   │   ├── routes/
│   │   │   ├── prescription.py    # Upload, OCR & AI processing
│   │   │   ├── auth.py            # Authentication & JWT
│   │   ├── services/
│   │   │   ├── ocr_service.py     # Google Vision integration
│   │   │   ├── llm_service.py     # Vertex AI text generation
│   │   │   ├── vector_service.py  # Matching Engine for RAG
│   │   ├── models/
│   │   │   ├── prescription.py    # MongoDB schemas
│   │   ├── utils/
│   │   │   ├── security.py        # HIPAA compliance & encryption
│   │   ├── config.py              # GCP & MongoDB configs
│   ├── requirements.txt           # Backend dependencies
│   ├── Dockerfile                 # Containerization
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.jsx
│   ├── package.json
│
├── docs/
│   ├── API_Documentation.md
│
├── .env.example                   # Example environment variables
├── README.md

```

## ***🚀 How It Works***

- #### *Upload prescription (Image/PDF)*

- #### *OCR extracts text using Google Vision API*

- #### *AI Parsing identifies medicine names, dosage & instructions*

- #### *RAG Pipeline fetches trusted drug details from medical sources*

- #### *LLM Explanation converts medical jargon into plain language*

- #### *User Dashboard displays results with dosage & instructions*

- #### *Secure Storage → Encrypted storage in MongoDB*

## ***🔒 Security & Compliance***

-  #### *De-identification of patient PHI (Protected Health Information)*

-  #### *Data Encryption at rest & in transit*

-  #### *IAM-based Access Control for API calls*

-  #### *HIPAA-ready architecture*

## ***🖼 Screenshots / Demo***

(Add your screenshots or Loom video here)


## ***📦 Installation***

### **Clone the repository**
- *git clone https://github.com/SREEDHIL/EvoDoc.git*

   - *cd EvoDoc*

### **Install server dependencies**
- *cd server*
   - *npm install*

### **Install client dependencies**
- *cd ../client*
   - *npm install*

<!-- ### **Environment Variables**

GCP_PROJECT_ID=your_project_id
GCP_CREDENTIALS_PATH=/path/to/credentials.json
MONGODB_URI=your_mongodb_uri
VERTEX_AI_INDEX_ID=your_vector_index_id -->

### **Run FastAPI Server**
-  **uvicorn app.main:app --reload*
### **Start frontend**
- *npm run dev*

## ***🎉 Future Enhancements***

- ***Mobile App for easy access***

- ***Voice-based prescription reading***

- ***Multi-language AI explanations***

- ***Integration with Pharmacy APIs***

## ***📝 License***

***This project is licensed under the*** $MIT$ $License.$
 
