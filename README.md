# MedAI+ — AI Healthcare Platform

MedAI+ is a full-stack AI-powered healthcare platform designed to simplify healthcare management through secure patient records, medical report analysis, appointment management, prescription handling, and AI-assisted medical information retrieval.

The platform combines a secure backend architecture with OCR and Retrieval-Augmented Generation (RAG) to help users extract information from medical documents and obtain context-aware responses grounded in their uploaded reports.

## ✨ Features

- **Secure Authentication:** JWT-based authentication using HTTP-only cookies.
- **Role-Based Authorization:** Role-specific access control for protected resources.
- **Patient Record Management:** Manage and access patient medical records securely.
- **Medical Report Analysis:** Extract text from medical documents using OCR.
- **AI-Powered Report Summarization:** Generate concise summaries of medical reports using RAG and LangGraph.
- **Document-Grounded AI Responses:** Retrieve relevant information from medical documents to provide context-aware answers.
- **Appointment Management:** Organize and manage healthcare appointments.
- **Prescription Management:** Maintain prescription-related information.
- **Medication Tracking:** Manage medication records and related information.
- **Protected REST APIs:** Secure endpoints for healthcare data and application operations.
- **Real-Time Communication:** Socket.io integration for supported real-time features.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Node.js | Backend runtime |
| Express.js | REST API development |
| MongoDB | Database and document storage |
| JWT | Authentication |
| HTTP-only Cookies | Secure token handling |
| Socket.io | Real-time communication |
| LangGraph | AI workflow orchestration |
| OCR | Text extraction from medical reports |
| RAG | Context-aware document retrieval and generation |

## 🏗️ System Overview

1. Users authenticate and access authorized healthcare resources.
2. The backend validates requests and enforces role-based permissions.
3. Healthcare records and related data are managed through MongoDB.
4. Medical documents are processed using OCR to extract readable text.
5. Extracted document content is used in a RAG pipeline orchestrated with LangGraph.
6. The AI workflow retrieves relevant context to generate report summaries and document-grounded responses.

## 🔐 Security

- JWT-based authentication.
- HTTP-only cookies for token handling.
- Role-based access control.
- Protected REST API endpoints.
- Server-side authorization checks for restricted resources.

## 🚀 Getting Started

### Prerequisites

- Node.js and npm
- MongoDB
- Git
- Required AI provider credentials for the configured AI workflow

### Installation

Clone the repository:

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd MedAI-Plus
```

Install backend dependencies:

```bash
npm install
```

Configure the environment variables required by your application in a `.env` file. Typical variables may include:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
AI_API_KEY=your_ai_provider_api_key
```

Use the actual variable names expected by your implementation. Never commit real credentials or secrets.

Start the development server using the script configured in your `package.json`:

```bash
npm run dev
```

## 📁 Project Structure

The project structure depends on the implementation. A possible organization is:

```text
MedAI-Plus/
├── controllers/
├── routes/
├── models/
├── middleware/
├── services/
├── config/
├── uploads/
├── app.js
├── package.json
├── .env.example
└── README.md
```

## 🔮 Future Improvements

- Doctor-patient video consultations.
- Real-time appointment notifications.
- Enhanced document processing and retrieval.
- Audit logging and fine-grained access control.
- Improved medical document management and search.

## ⚠️ Disclaimer

MedAI+ is intended to support healthcare information management and medical document understanding. AI-generated summaries and responses are not a substitute for professional medical advice, diagnosis, or treatment.

## 👨‍💻 Author

Developed as a full-stack AI healthcare project integrating backend engineering, authentication, database management, and document-grounded AI workflows.
