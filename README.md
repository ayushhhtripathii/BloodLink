\# 🩸 BloodLink — Blood Donor Finder



\*\*Connecting Blood Donors with People in Need. Saving Lives Through Technology.\*\*



BloodLink is a web-based Blood Donor Finder application designed to help connect people who need blood with potential blood donors. It provides a centralized platform for discovering donors, managing blood requests, and supporting faster communication during medical emergencies.



The project aims to make blood donor discovery more accessible through a user-friendly interface, donor search functionality, and a backend designed to manage users, requests, and donor matching.



> \*\*Project Type:\*\* Full-Stack Web Application  

> \*\*Domain:\*\* Healthcare Technology / Social Impact  

> \*\*Frontend:\*\* React, Vite, JavaScript  

> \*\*Backend:\*\* Node.js, Express.js  

> \*\*Database:\*\* Configure according to the backend's database settings



\---



\## 📌 Table of Contents



\- \[About the Project](#-about-the-project)

\- \[Problem Statement](#-problem-statement)

\- \[Objectives](#-objectives)

\- \[Features](#-features)

\- \[Technology Stack](#-technology-stack)

\- \[Project Architecture](#-project-architecture)

\- \[Screenshots](#-screenshots)

\- \[Project Structure](#-project-structure)

\- \[Installation and Setup](#-installation-and-setup)

\- \[Environment Configuration](#-environment-configuration)

\- \[Running the Application](#-running-the-application)

\- \[API Overview](#-api-overview)

\- \[Future Scope](#-future-scope)

\- \[Security and Medical Disclaimer](#-security-and-medical-disclaimer)

\- \[Contributing](#-contributing)

\- \[Author](#-author)

\- \[License](#-license)



\## 📖 About the Project



BloodLink aims to simplify the process of finding potential blood donors by bringing donor discovery and blood request management into one platform.



In urgent medical situations, finding a suitable donor can be challenging. BloodLink provides a digital solution intended to help recipients discover potential donors and coordinate blood requests more efficiently.



The application includes a React-based user interface and a Node.js backend with dedicated routes for authentication, donor discovery, blood requests, matching, notifications, and chat.



\## ❗ Problem Statement



Finding an appropriate blood donor can be difficult when information is scattered across personal contacts, social media groups, and different organizations.



Common challenges include:



\- Difficulty discovering donors with a required blood group.

\- Delays in communicating urgent blood requirements.

\- Lack of a centralized donor discovery platform.

\- Difficulty organizing and tracking blood requests.

\- Limited access to structured donor information.



\*\*Proposed solution:\*\* BloodLink provides a centralized web application to help users discover potential donors and organize blood donation requests through a structured digital platform.



\## 🎯 Objectives



1\. Develop an accessible and user-friendly blood donor discovery platform.

2\. Help users search for potential donors by relevant criteria.

3\. Support the management of blood donation requests.

4\. Organize backend functionality into maintainable modules.

5\. Provide a foundation for donor matching and notification features.

6\. Encourage voluntary blood donation and community participation.



\## ✨ Features



\### 🩸 Donor Discovery

\- Interface for finding potential blood donors.

\- Donor search and filtering workflows.

\- Dedicated donor discovery page.



\### 🚨 Emergency Dashboard

\- Dedicated interface for emergency-related workflows.

\- Centralized access to important blood request information.



\### 🏥 Blood Bank Directory

\- Dedicated blood bank page.

\- A foundation for displaying blood bank information and contact details.



\### 🔐 Authentication

\- Dedicated login interface.

\- Backend authentication routes.

\- User model for organizing account information.



\### 🔄 Blood Request Management

\- Dedicated backend routes for blood requests.

\- Structured request data using a dedicated model.

\- A foundation for managing requests and their status.



\### 🤝 Donor Matching

\- Dedicated matching API routes.

\- Matching service designed to organize donor matching logic.



\### 💬 Chat and Notifications

\- Dedicated chat API routes.

\- Notification service and notification endpoints.

\- A foundation for improving communication between users.



\*Feature availability depends on the current implementation and configuration. Production authentication, live notifications, and real-time messaging should be verified before being advertised as fully operational.\*



\## 🛠️ Technology Stack



| Technology | Purpose |

|---|---|

| React | Component-based frontend |

| Vite | Frontend development server and build tool |

| JavaScript (JSX) | Frontend application logic |

| CSS | Responsive styling and interface design |

| Node.js | Backend JavaScript runtime |

| Express.js | Backend routing and API framework |

| npm | Dependency and package management |

| Git and GitHub | Version control and source code hosting |



\*\*Additional components:\*\* The backend includes user and blood request models, authentication routes, donor routes, matching services, notification functionality, and chat routes. Confirm the configured database and any third-party integrations in the backend configuration before listing them as dependencies.



\## 🏗️ Project Architecture



BloodLink follows a client-server architecture.



```text

&#x20;                 ┌────────────────────────┐

&#x20;                 │       User             │

&#x20;                 └───────────┬────────────┘

&#x20;                             │

&#x20;                             ▼

&#x20;                 ┌────────────────────────┐

&#x20;                 │   React + Vite         │

&#x20;                 │   Frontend             │

&#x20;                 └───────────┬────────────┘

&#x20;                             │ HTTP / API

&#x20;                             ▼

&#x20;                 ┌────────────────────────┐

&#x20;                 │   Node.js + Express    │

&#x20;                 │   Backend API          │

&#x20;                 └───────────┬────────────┘

&#x20;                             │

&#x20;            ┌────────────────┼────────────────┐

&#x20;            ▼                ▼                ▼

&#x20;      ┌───────────┐   ┌─────────────┐  ┌─────────────┐

&#x20;      │   Users   │   │ Donors and  │  │ Matching,   │

&#x20;      │   Auth    │   │ Requests    │  │ Chat, Alerts│

&#x20;      └───────────┘   └─────────────┘  └─────────────┘

&#x20;                             │

&#x20;                             ▼

&#x20;                 ┌────────────────────────┐

&#x20;                 │ Configured Database    │

&#x20;                 └────────────────────────┘

```



The frontend handles the user interface, while the backend exposes API routes and services for application operations. The actual database connection and authentication flow depend on the backend configuration.



\## 📸 Screenshots



The repository includes three project images. Open them below to explore the available interface or design references.



\### Screenshot 1



!\[BloodLink Screenshot 1](./screen.png)



\### Screenshot 2



!\[BloodLink Screenshot 2](./screen2.png)



\### Screenshot 3



!\[BloodLink Screenshot 3](./screen3.png)



\## 📂 Project Structure



```text

BloodLink/

│

├── backend/

│   ├── models/

│   │   ├── User.js

│   │   └── BloodRequest.js

│   ├── routes/

│   │   ├── auth.js

│   │   ├── donors.js

│   │   ├── match.js

│   │   ├── notifications.js

│   │   ├── requests.js

│   │   └── chat.js

│   ├── services/

│   │   ├── matchingService.js

│   │   └── notificationService.js

│   ├── docs/

│   ├── .env.example

│   ├── package.json

│   ├── package-lock.json

│   ├── seed.js

│   └── server.js

│

├── frontend/

│   ├── public/

│   ├── src/

│   │   ├── assets/

│   │   ├── components/

│   │   │   ├── Chatbot/

│   │   │   └── Layout/

│   │   ├── data/

│   │   ├── pages/

│   │   │   ├── BloodBanks/

│   │   │   ├── EmergencyDashboard/

│   │   │   ├── FindDonors/

│   │   │   └── Login/

│   │   ├── services/

│   │   ├── App.jsx

│   │   ├── App.css

│   │   ├── index.css

│   │   └── main.jsx

│   ├── package.json

│   └── vite.config.js

│

├── docs/

├── AGENT.md

├── DESIGN.md

├── screen.png

├── screen2.png

├── screen3.png

└── README.md

```



\*This structure summarizes the repository layout; some files may be added or changed during development.\*



\## ⚙️ Installation and Setup



\### Prerequisites



Install the following software before running BloodLink:



\- \[Node.js](https://nodejs.org/) — use a version compatible with the project's dependencies.

\- npm — included with Node.js.

\- \[Git](https://git-scm.com/) — for cloning the repository.

\- A configured database, if required by the backend.



\### 1. Clone the repository



```bash

git clone https://github.com/ayushhhtripathii/BloodLink.git

cd BloodLink

```



\### 2. Install backend dependencies



```bash

cd backend

npm install

```



\### 3. Configure backend environment variables



Create a local `.env` file using the supplied example:



\*\*Windows PowerShell\*\*



```powershell

Copy-Item .env.example .env

```



Open `backend/.env` and configure the required variables according to `backend/.env.example` and the backend source code.



Do not commit `.env` or publish real credentials.



\### 4. Install frontend dependencies



Open another terminal from the repository root:



```bash

cd frontend

npm install

```



\## 🔧 Environment Configuration



The backend may require environment variables for database connectivity, authentication, and external integrations.



Use `backend/.env.example` as the source of truth for the exact variable names.



Example format:



```dotenv

\# Add the actual variable names from backend/.env.example

\# Set your local database connection if required

\# Configure authentication secrets if required

\# Add external API credentials only when required

```



Do not copy this illustrative block as a working configuration. Use the actual keys expected by the application.



\*\*Security recommendations:\*\*



\- Never publish passwords, tokens, private keys, or production credentials.

\- Keep `.env` files out of Git.

\- Use strong, unique authentication secrets.

\- Never expose backend-only secrets through frontend environment variables.



\## ▶️ Running the Application



Run the frontend and backend in separate terminals.



\### Terminal 1: Start the backend



```powershell

cd backend

npm start

```



The backend uses `server.js` as its startup entry point, according to the package configuration.



Check the terminal output for the port and startup status. Configure the frontend API base URL to match the backend's actual address.



\### Terminal 2: Start the frontend



```powershell

cd frontend

npm run dev

```



Vite will display a local development URL, commonly:



```text

http://localhost:5173/

```



Open the URL displayed in your terminal.



\### Build the frontend



To create a production frontend build:



```powershell

cd frontend

npm run build

```



Vite generates the production build in the `dist/` directory.



\### Run the linter



```powershell

cd frontend

npm run lint

```



This runs the frontend linting script configured in `package.json`.



\### Troubleshooting



\*\*Backend does not start\*\*

\- Check the backend terminal for missing dependencies or environment variables.

\- Verify that the required database service is available.

\- Confirm that the configured port is not already in use.



\*\*Frontend cannot reach the backend\*\*

\- Check the API base URL in `frontend/src/services/api.js`.

\- Confirm that the backend is running.

\- Verify CORS settings and required environment variables.



\*\*Login or donor search does not work\*\*

\- Inspect browser developer tools and backend logs.

\- Verify the relevant API routes and database configuration.

\- Check that the frontend uses the correct API endpoints.



\## 🔌 API Overview



The backend organizes functionality into dedicated route modules.



| Route module | Responsibility |

|---|---|

| `auth.js` | Authentication-related operations |

| `donors.js` | Donor-related operations |

| `match.js` | Donor matching operations |

| `requests.js` | Blood request operations |

| `notifications.js` | Notification operations |

| `chat.js` | Chat-related operations |



These names describe the backend modules, not necessarily the complete public URL paths. Inspect `backend/server.js` to identify the exact mounted API prefixes, HTTP methods, request formats, and authentication requirements.



\## 🔮 Future Scope



BloodLink can be extended with the following enhancements:



\### 1. Intelligent Donor Matching

\- Match potential donors using blood group, location, and availability.

\- Rank results using transparent matching criteria.

\- Consider travel distance and response time.



\### 2. Real-Time Notifications

\- Notify suitable donors when a new request is created.

\- Provide request status updates.

\- Add optional email or SMS integrations.



\### 3. Location-Based Discovery

\- Integrate maps and distance calculations.

\- Display nearby donors and registered blood banks.

\- Provide location-aware search with appropriate privacy controls.



\### 4. Hospital and Blood Bank Integration

\- Provide verified organization profiles.

\- Display contact information and verified availability where integrations permit.

\- Support coordinated requests with participating organizations.



\### 5. Enhanced Security

\- Add robust authentication and role-based authorization.

\- Validate and sanitize user inputs.

\- Implement rate limiting, audit logging, and abuse prevention.

\- Protect personal and medical information.



\### 6. Better User Experience

\- Improve mobile responsiveness and accessibility.

\- Add multilingual support.

\- Improve loading states, error handling, and form validation.



\### 7. Analytics and Administration

\- Provide administrative tools for reviewing reports.

\- Display aggregate donation and request statistics.

\- Track system performance without exposing unnecessary personal information.



\## 🔐 Security and Medical Disclaimer



BloodLink is a technology platform intended to facilitate connections between potential blood donors and recipients. It does not replace professional medical advice, clinical screening, blood grouping, compatibility testing, or healthcare-provider procedures.



Donor eligibility and transfusion suitability must be verified by qualified healthcare professionals. Users should not rely solely on application matching results when making medical decisions.



The application should be deployed with appropriate safeguards for personal information, authentication, authorization, and secure communications.



\## 🤝 Contributing



Contributions and suggestions are welcome.



1\. Fork the repository.

2\. Create a feature branch.

3\. Make and test your changes.

4\. Commit your changes with a descriptive message.

5\. Open a pull request describing the changes.



For example:



```bash

git checkout -b feature/improve-donor-search

git add .

git commit -m "Improve donor search"

git push origin feature/improve-donor-search

```



\## 👨‍💻 Author



\*\*Ayush\*\*



GitHub: \[@ayushhhtripathii](https://github.com/ayushhhtripathii)



Project repository: \[BloodLink — Blood Donor Finder](https://github.com/ayushhhtripathii/BloodLink)



\## 📄 License



A license has not yet been specified. Before distributing or reusing this project, choose an appropriate open-source license and add its corresponding `LICENSE` file.



\---



\*\*BloodLink — Bringing Donors and Recipients Closer Through Technology. 🩸\*\*



