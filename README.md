Hi there, I’m Juchang Kim (JC) <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px">

# :wave: About Me

## :mortar_board: Education
Bachelor of Computer and Information Science (Feb 2023 – Dec 2025)
Auckland University of Technology (AUT), Auckland, New Zealand


## :computer: Technical Skills
Programming Languages: Proficient in Python, C, and Java (including data structures & algorithms)
Web Development: React.js (front end) and Node.js (back end)

### Cloud Computing:
AWS: Certified AWS Solutions Architect – Associate (SAA-C03)
Azure: Certified Azure Developer Associate (AZ-204)

### Database Management:
Relational DBs (Oracle SQL, MySQL, DerbyDB)
NoSQL DBs (MongoDB, Firebase)

### Networking: 
Knowledge of network design, switches, and routing (certified CCNA)

### Operating Systems: 
Linux (Ubuntu) environments, Windows

### Project Management: 
Familiar with Agile/Scrum methodologies, certified CAPM

### Testing and Debugging: 
Familiar with unit testing, TDD, integration testing, regression testing, API testing, E2E testing, automation testing and debugging processes (Jest, Junit, xUnit, Android testing, UAT, Playwright, Github Actions, Postman)

## :trophy: Certifications
- Certified Associate in Project Management (CAPM), PMI (Feb 2024)

- Cisco Certified Network Associate (CCNA), Cisco (Nov 2024)

- AWS Solutions Architect – Associate (SAA-C03), AWS (Dec 2024)


## :star2: Extracurricular Activities
- AUT Computer Science & Engineering Association Club (Feb 2023 – Dec 2025)

- AI Hackathon with She Sharp and Fisher & Paykel Healthcare (Jul 2024)


## :rocket: Projects

### Taxi Booking System (Full Stack + AI Chatbot)
[Live Demo Link](http://54.79.89.195)  
[GitHub Repository Link](https://github.com/JuchangKim/taxi-booking-system)

#### A complete taxi booking management system with:

- Customer booking form

- Admin booking assignment panel

- CSV export of booking history

- FastAPI chatbot integrated with Ollama (Llama3.2:3b)

- Docker Compose multi-service architecture

- MySQL, PHP backend

- Automatic CSV refresh for chatbot

- Deployed on AWS Lightsail

#### Technologies Used

- PHP (Apache)

- HTML, CSS, JavaScript

- MySQL

- FastAPI (Python)

- Ollama AI model

- Docker & Docker Compose

- AWS Lightsail hosting

#### Features

- Book a taxi

- Admin CRUD functions, search and assign

- CSV export

- Chatbot answers booking questions

- Real-time booking history

- Fully containerized deployment

---

### Fiserv Sign In (Typescript, React + C#, .NET + Android + Firebase + Label Printer - Hardware)

#### Executive Summary
Fiserv Sign‑In Tool is a modern visitor **sign‑in / sign‑out** solution replacing an older system at Fiserv Auckland. It provides **tablet‑based check‑in**, **admin web dashboard**, **audit logging**, and **label printing**, built with **Android (Kotlin)**, **React + TypeScript**, **.NET 8**, and **Firebase Firestore**. The product improves usability, accessibility, and security while enabling real‑time visibility for reception and administrators.



#### Objectives & Goals
- **Deliver a modern, user‑friendly sign‑in tool** that surpasses the legacy system.
- **Enhance security & compliance** (encrypted transport, mutable audit logs).
- **Integrate smoothly** with internal identity/access control (card/QR support).
- **Improve UX & reduce waiting times** through kiosk flows and admin tools.
- **Increase operational efficiency** with automation (printing, exports, filtering).



#### Scope — High‑Level Requirements
**Functional**
- Realtime **sign‑in/out** (tablet & dashboard)
- **RFID / Card / QR** assisted sign‑in/out with duplicate/invalid protection
- **Badge label printing** (Zebra ZD410 over BT/BLE)
- **Pre‑registration** & on‑site check‑in (tablet)
- **Notifications** (host aware — optional extension)
- **Audit history** (mutable events + who/when/what)
- **Search, filters, CSV export** (attendance, events, changes)
- **Admin profile editing** (with validation & toast feedback)

**Non‑Functional**
- Encrypted transport (**HTTPS**) across all layers
- Reliable realtime updates (**Firestore onSnapshot**)
- Responsive UI (desktop & tablet)

  
#### Architecture & Tech Stack
```
[Label Printer(Zebra ZD410)] <----[Android Tablet (Kotlin + Compose)]
              ▲                       │ (REST / HTTPS)
              |                       |
              |                       |
        [ASP.NET Core 8 API ]         |
            ▲  |          │           ▼      
            |  |          ▼                                   
            |  |         [Firebase Admin SDK (Firestore)] 
            |  |                 ▲
            |  ▼                 │
[React + TypeScript (Vite) Admin Dashboard]
```

**Technologies**
- **Frontend:** React, TypeScript, Vite, RTL/Vitest
- **Backend:** ASP.NET Core (.NET 8), SignalR, Swagger, HealthChecks, xUnit
- **Realtime DB:** Firebase **Firestore**
- **Mobile:** Android (Kotlin, Jetpack Compose)
- **Printing:** Zebra ZD410 via BT/BLE (backend REST)
- **CI/CD:** GitHub Actions (frontend, backend, Android)

#### Final Feature Set (Sprint 1 → 8)
- Manual visitor **Sign‑In/Out** (tablet + dashboard) with **confirmation**
- Robust **validation** (empty/format/date/time; sign‑in < sign‑out)
- **Realtime dashboard** (Firestore; no refresh)
- **Audit history** (mutable events: sign‑in/out, label prints)
- **Search & Filters** (type, name, date range), **CSV export**
- **Visitor type classification** (Contractor/Staff/Visitor/Other)
- **Admin profile editing** with toast feedback; **Delete** with confirm
- **QR sign‑out**, **Card access** (Card IDs) with duplicate prevention
- **Label printing** (connect/status/test/disconnect; reprint support)
- **Today’s Visitors** widget (Active vs Signed‑Out)
- **Same‑name sign‑out disambiguation** (phone fallback)
- **Bulk edit** in History with **audit trail**
- **Secure admin login** (multi‑admin)
- **HTTPS/SSL** end‑to‑end



#### Security & Compliance
- All traffic over **HTTPS** (local dev uses self‑signed certs).
- Firestore access via server **Admin SDK**; client reads follow security rules.
- **mutable audit** entries for compliance / forensics.
- Consistent **UTC** timestamps.

#### Testing & Quality Gates
- **Frontend:** Vitest + RTL (regression suite)
- **Backend:** xUnit + Coverlet
- **Android:** JUnit + Compose UI tests
- **E2E:** Playwright smoke
- **CI/CD:** GitHub Actions (builds, tests, artifacts)

Sprint‑8 metrics: Web **353/353** passing; Backend all passing (~36% coverage); Android all passing; E2E smoke green.

---

### HireHub - Job Hunting Website
[GitHub Repository Link](https://github.com/JuchangKim/HireHubWeb.git)

[Live Demo Link](https://hirehub-bbfsh4a5feexh3gt.newzealandnorth-01.azurewebsites.net/)

- Front end: React.js

- Back end: Node.js

- Database: MongoDB

- REST API for CRUD functionalities

- Authentication with JWT

- Deployed via Azure Web App

### Poker Game – Playing with Multiple Computer Players
- Developed in Java (NetBeans IDE)

- Utilized JDBC with Embedded Derby

- Implemented MVC pattern, simple unit tests, and a GUI

[GitHub Repository Link](https://github.com/JuchangKim/PokerApp.git)

[Click here to download `dist.zip` for Poker Game](https://github.com/JuchangKim/PokerApp/raw/main/Assignment1/dist.zip)


## :handshake: Let's Connect!
I’m always eager to explore new opportunities, collaborate on projects, or just talk tech. Feel free to reach out via LinkedIn(www.linkedin.com/in/juchang-kim).

Thanks for stopping by, and happy coding!

Created by Juchang Kim (JC)

Project - Fiserv Sign in Tool
[![wakatime](https://wakatime.com/badge/user/6dde0cf2-3771-48b7-966f-8af3d78cd884/project/d2f2d174-8a5a-4ae1-8728-1bf1b483cc04.svg)](https://wakatime.com/badge/user/6dde0cf2-3771-48b7-966f-8af3d78cd884/project/d2f2d174-8a5a-4ae1-8728-1bf1b483cc04)

Subproject - Label Printer
[![wakatime](https://wakatime.com/badge/user/6dde0cf2-3771-48b7-966f-8af3d78cd884/project/cf9e0d3d-c35e-4a04-a5b5-27a2910aab0e.svg)](https://wakatime.com/badge/user/6dde0cf2-3771-48b7-966f-8af3d78cd884/project/cf9e0d3d-c35e-4a04-a5b5-27a2910aab0e)

Project - Taxi Booking System
[![wakatime](https://wakatime.com/badge/user/6dde0cf2-3771-48b7-966f-8af3d78cd884/project/6725cd01-578c-4fc1-baa5-3998ffdfd891.svg)](https://wakatime.com/badge/user/6dde0cf2-3771-48b7-966f-8af3d78cd884/project/6725cd01-578c-4fc1-baa5-3998ffdfd891)


[![WakaTime](https://wakatime.com/share/@JCKim/7c6b8f23-ef4d-454a-90c7-f9b19da6e338.png)](https://wakatime.com/)


    
![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=JuchangKim)
<br>
<br>
![GitHub Streak](https://streak-stats.demolab.com?user=JuchangKim&theme=vue&mode=weekly)
