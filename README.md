#  Loan Origination System

A full-stack demo project that simulates a **Loan Origination Platform** — covering borrower onboarding, loan application submission, decisioning, and offer generation.  
Built as part of a coding interview exercise, this project demonstrates clean architecture, domain-driven design, and modern full-stack practices using **Spring Boot + React + Gradle + Vite**.

---

##  Architecture Overview
```
swift

loan-origination-system/
├── backend/
│   ├── src/main/java/com/example/loanorigination/
│   ├── src/test/java/com/example/loanorigination/
│   ├── build.gradle.kts
│   └── settings.gradle.kts
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   ├── vite.config.js
│   └── README.md
│
└── README.md  ← this file
```

### Backend
- **Framework:** Spring Boot 3 (Java 17)
- **Build:** Gradle Kotlin DSL (`build.gradle.kts`)
- **Database:** H2 (in-memory) or PostgreSQL (configurable)
- **Libraries:** Lombok, MapStruct, JPA, Spring Web, Validation
- **Testing:** JUnit 5, Mockito
- **Observability:** SLF4J logging, Exception Handling, DTO mapping
- **Pattern:** Domain-Driven Design + Layered Architecture (Controller → Service → Repository)

### Frontend
- **Framework:** React 18 with Vite
- **Language:** JavaScript / JSX
- **UI:** Responsive form-based flow (Loan Application)
- **Styling:** CSS / optional Tailwind / Bootstrap
- **Build Tool:** Vite (`vite.config.js`)

---

## ⚙️ Setup Instructions

### 🧩 Prerequisites
- Java 17+
- Node.js 18+
- npm 9+
- (Optional) PostgreSQL if using a persistent DB

---

### 🖥️ Backend Setup

```
bash

cd backend
./gradlew clean build
./gradlew bootRun
```
Backend runs on:
➡️ http://localhost:8080

💻 Frontend Setup
```
bash

cd frontend
npm install
npm run dev
```
Frontend runs on:
➡️ http://localhost:5173

You can now open the app in your browser, fill in loan details, and see approval or rejection decisions dynamically rendered via API responses.

🧪 Example API Endpoints
Method	Endpoint	Description
POST	/api/loans/apply	Submit a loan application
GET	/actuator/health	Health check endpoint


🧑‍💻 Author

Surabhi Subbanarasimha
Senior Software Engineer — Commonwealth Bank of Australia
