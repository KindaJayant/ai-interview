# 🎙️ Prepwise – AI Mock Interview Platform

An AI-powered mock interview platform built with **Next.js, Firebase, Vapi Voice Agents, and Google Gemini**.

Prepwise allows users to simulate real job interviews using AI voice agents, receive structured feedback, and track their performance through a personalized dashboard.

---

## 🚀 Live Demo

Link: 

---

## 🧠 Overview

Prepwise is a full-stack web application designed to help users prepare for job interviews through interactive AI voice sessions.

The platform:

* Generates interview questions dynamically
* Conducts voice-based mock interviews
* Transcribes conversations in real time
* Uses AI to generate structured performance feedback
* Stores interview history for review and improvement

This project demonstrates real-world integration of:

* AI voice workflows
* Generative AI APIs
* Authentication systems
* Scalable backend architecture
* Modern UI component systems

---

## 🛠 Tech Stack

**Frontend**

* Next.js (App Router)
* Tailwind CSS
* shadcn/ui

**Backend**

* Next.js API Routes
* Firebase (Authentication + Firestore)
* Firebase Admin SDK

**AI & Voice**

* Vapi AI (Voice Agent Workflows)
* Google Gemini (Question generation + feedback analysis)

**Validation**

* Zod

---

## ✨ Features

### 🔐 Authentication

* Email/password authentication via Firebase
* Protected dashboard routes
* Persistent session handling

### 🎙 AI Mock Interviews

* Dynamic interview generation
* AI voice agent conducts the interview
* Real-time transcript capture

### 🧠 AI Feedback Engine

* AI analyzes transcript
* Structured feedback:

  * Communication
  * Technical clarity
  * Confidence
  * Areas of improvement
* Score breakdown system

### 📊 Dashboard

* View all past interviews
* Track improvement over time
* Access detailed transcripts and feedback

### 📱 Responsive UI

* Fully responsive layout
* Clean, modern interface
* Accessible component system

---

## 📂 Project Structure

```
prepwise/
│
├── app/
│   ├── (auth)/
│   │   ├── sign-in/
│   │   └── sign-up/
│   │
│   ├── (root)/
│   │   ├── dashboard/
│   │   ├── interview/
│   │   │   └── [id]/
│   │   │       ├── page.tsx
│   │   │       └── feedback/
│   │   │           └── page.tsx
│   │
│   ├── api/
│   │   ├── vapi/
│   │   │   └── generate/
│   │   │       └── route.ts
│   │   └── interviews/
│   │
│   ├── layout.tsx
│   └── page.tsx
│
├── components/
│   ├── ui/
│   ├── InterviewCard.tsx
│   ├── FeedbackCard.tsx
│   └── Navbar.tsx
│
├── lib/
│   ├── actions/
│   │   └── general.action.ts
│   ├── firebase/
│   │   ├── client.ts
│   │   └── admin.ts
│   ├── utils.ts
│   └── validators.ts
│
├── public/
│
├── styles/
│   └── globals.css
│
├── .env.local
├── tailwind.config.ts
├── next.config.js
└── package.json
```

---

## ⚙️ Environment Variables

Create a `.env.local` file in the root directory:

```env
# Vapi
NEXT_PUBLIC_VAPI_WEB_TOKEN=
NEXT_PUBLIC_VAPI_WORKFLOW_ID=

# Google Gemini
GOOGLE_GENERATIVE_AI_API_KEY=

# App URL
NEXT_PUBLIC_BASE_URL=

# Firebase (Client)
NEXT_PUBLIC_FIREBASE_API_KEY=
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=
NEXT_PUBLIC_FIREBASE_PROJECT_ID=
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=
NEXT_PUBLIC_FIREBASE_APP_ID=

# Firebase (Admin)
FIREBASE_PROJECT_ID=
FIREBASE_CLIENT_EMAIL=
FIREBASE_PRIVATE_KEY=
```

Make sure:

* Firebase Authentication is enabled
* Firestore database is created
* Vapi workflow is configured
* Gemini API key has proper access

---

## 🧪 How It Works

### 1️⃣ Interview Creation Flow

1. User selects job role
2. Backend calls Gemini API
3. Structured interview questions are generated
4. Vapi workflow is initialized
5. Voice session begins

---

### 2️⃣ Interview Feedback Flow

1. Transcript collected after interview
2. Transcript sent to Gemini
3. AI generates:

   * Overall score
   * Category scores
   * Improvement suggestions
4. Feedback stored in Firestore
5. Displayed on feedback page

---

## 🏗 Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/prepwise.git
cd prepwise
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Add Environment Variables

Create `.env.local` and add your credentials.

### 4. Run Development Server

```bash
npm run dev
```

Visit:

```
http://localhost:3000
```

---

## 📈 Future Improvements

* Interview difficulty levels
* AI-generated resume-based questions
* Analytics dashboard with charts
* Leaderboard system
* Performance trend visualization
* Role-based interview templates
* Real-time speech sentiment analysis

---

## 🧱 Architectural Decisions

* App Router used for scalable routing
* Firebase Admin SDK for secure server operations
* Action-based abstraction in `lib/actions`
* Component-based UI architecture
* Reusable AI prompt utilities
* Zod schema validation for API inputs

---

## 🧩 Key Learnings

* Voice AI integration in production systems
* Secure Firebase Admin usage in Next.js
* Designing AI prompts for structured output
* Managing async voice workflows
* Building scalable full-stack architecture

---

## 👨‍💻 About Me

**Jayant**
AI Engineer Intern
Focused on building AI-powered systems, scalable web applications, and backend architecture.

You can connect with me here:

* LinkedIn: (add link)
* GitHub: (add link)
* Portfolio: (add link)


