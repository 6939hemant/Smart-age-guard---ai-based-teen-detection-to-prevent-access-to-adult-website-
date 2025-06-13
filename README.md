# Smart-age-guard-ai-based-teen-detection-to-prevent-access-to-adult-website-
# Smart AgeGuard – AI-Based Teen Detection to Prevent Access to Adult Websites

A smart, AI-powered web access control system that uses facial recognition and age estimation to block underage users (teens/kids) from accessing adult websites. This project replaces weak, traditional yes/no age verification with a more secure and ethical solution.

---

## Author's Note: A Dream Towards MIT

Hi, I’m **Hemant Khemraj Khekare**, a student deeply passionate about ethical technology, AI, and building real-world solutions to human problems.

This project is a part of my **independent research portfolio** and my heartfelt effort to demonstrate how meaningful innovations can make the internet safer — especially for vulnerable users like children and teens.

I’ve always dreamt of joining **MIT** — not just because it's the world’s top institute for engineering and innovation, but because I believe in MIT’s mission of using knowledge to serve humanity.

This project reflects the kind of student I aspire to be at MIT: someone who doesn’t just write code, but writes **impactful solutions**. I hope this project communicates my intent, creativity, and technical skills to the MIT admissions team, and inspires further development in the field of AI for safety.

Thank you for reading, and thank you to MIT for being the beacon that drives me forward.

---

## Table of Contents
- [Problem Statement](#problem-statement)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [System Architecture](#system-architecture)
- [Getting Started](#getting-started)
- [Step-by-Step Development Guide](#step-by-step-development-guide)
- [Future Improvements](#future-improvements)
- [Author's Note](#authors-note)
- [License](#license)

---

## Problem Statement
Traditional websites use simple checkboxes or text boxes to confirm if a user is 18+. This approach is ineffective as minors can easily bypass it. Our solution uses AI to verify age through facial features or behavior, creating a safer online environment for children and teens.

---

## Features
- AI-based face detection and age estimation using webcam
- Immediate blocking or redirection of underage users
- Admin/parent override panel with password protection
- Local processing for privacy-preserving age inference
- User-friendly and mobile-responsive UI

---

## Tech Stack
- **Frontend**: React.js, Tailwind CSS
- **AI Models**: TensorFlow.js or OpenCV (for browser-side inference)
- **Authentication**: LocalStorage or JWT (for Admin Panel)
- **Optional Backend**: Node.js or Flask (for storing admin settings)

---

## System Architecture

User ──> UI (React) ──> Face Detection (Webcam) ──> Age Estimation Model └──> Block / Allow Logic └──> Admin Panel ──> Override Controls

---

## Getting Started

### Prerequisites
- Node.js and npm installed
- Git installed

### Installation
```bash
git clone https://github.com/your-username/smart-ageguard.git
cd smart-ageguard
npm install

Run the app

npm start


---

Step-by-Step Development Guide

Step 1: Set up React App

npx create-react-app smart-ageguard
cd smart-ageguard
npm install

Step 2: Set up Tailwind CSS

Follow official Tailwind docs: https://tailwindcss.com/docs/guides/create-react-app

Step 3: Add Webcam Access

Install webcam package:

npm install react-webcam

Create a component to access webcam and capture image.

Step 4: Integrate Face Detection & Age Estimation

Use TensorFlow.js face landmarks detection

Or use a pretrained OpenCV DNN model with ONNX/TensorFlow model


Step 5: Decision Logic

If age < 18:

Show a blocking screen or redirect to safe content


If age ≥ 18:

Allow access or display adult content warning


Step 6: Admin/Parent Panel

Create login page with a hardcoded password

Allow admin to toggle detection ON/OFF

Save preferences in LocalStorage or a backend


Step 7: Ethical Disclaimer & Privacy Modal

Explain that face detection is local

Request user permission before using webcam



---

Future Improvements

Multi-factor verification (voice, behavior)

Better accuracy using a deep CNN or custom-trained model

Cloud storage for admin settings

Government ID-based override system

Real-time alerts to parents



---

License

MIT License
