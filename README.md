[*◉*Smart Attendance](#top)

[Features](#features)[Screens](#screens)[AI Pipelines](#ai)[Architecture](#arch)[Get started](#start)

[★ GitHub](https://github.com/muskxann/AI-attendance)

Face & voice biometrics

# Attendance that recognizes your class.

A smart AI tool that marks attendance using face and voice recognition. Teachers snap a photo or take a voice sample; students see their stats instantly. No roll calls. No paper registers.

[Get started →](#start) [View repository](https://github.com/muskxann/AI-attendance)

PythonStreamlitResemblyzerSupabase

Smart Attendance · Teacher dashboard

Teacher dashboard of the Smart Attendance app

*✅*

Student identifiedMarked present

*🎙️*

Speaker embeddingVoice attendance

Overview

## Everything attendance needs, in one app

Machine learning pipelines, biometric feature extraction, database operations and an interactive web interface — combined into a single Streamlit application.

🧑‍🎓

### Face recognition

Facial embeddings plus a trained classifier identify students from classroom photographs.

🎙️

### Voice attendance

Speaker embeddings extracted with Resemblyzer power a separate voice-based workflow.

🔗

### Links & QR codes

Share a class link or display a QR code so students can jump straight to enrollment.

Two portals

## Built for teachers and students

### 👨‍🏫 Teacher portal

- **Subject management** — create subjects with codes and sections
- **AI attendance** — pick a subject, add photos, run the analysis
- **Voice attendance** — a dedicated speaker-based workflow
- **Records** — timestamps, subjects and attendance statistics
- **Student overview** — enrollment counts per subject

### 🎓 Student portal

- **Sign up & log in** — plus a Face ID login workflow
- **Enroll** — via enrollment codes, shared links or QR scan
- **My subjects** — courses, codes and sections at a glance
- **Statistics** — total classes vs. classes attended
- **Course control** — unenroll whenever needed

Product tour

## See it in action

A walkthrough of the real application, from sign-up to attendance records.

Smart Attendance

AI & ML

## Two pipelines, two biometrics

Faces and voices are processed by separate pipelines. Each one turns raw input into numerical embeddings, then identifies the person.

🧑‍🎓 Facial recognition

Student photos

Face processing

Embeddings

Classifiertrained

Attendance

🎙️ Voice recognition

Voice input

Audio processing

Speaker embeddingResemblyzer

Identification

Attendance

Architecture

## Cleanly separated layers

Interface, workflows, AI pipelines and database operations each live in their own component.

**Streamlit UI**Forms, dashboards, subject cards and attendance tables in a lavender & purple theme.

**Portals**Teacher and student workflows: auth, enrollment, class sharing.

**Pipelines**Face embeddings + classifier, and Resemblyzer speaker embeddings.

**Supabase**Persistent storage for users, subjects, records and statistics.

Tech stack

PythonStreamlitUINumPyPillowimagesResemblyzervoiceSupabasedatabase

Database schema

Supabase schema with students, teachers, subjects, subject_students and attendance_logs tables

Five Supabase tables link teachers, subjects, students and attendance logs. Each student row stores a **face_embedding** and a **voice_embedding** as JSONB.

Quick start

## Up and running in five steps

*1*

#### Clone the repository

git clone https://github.com/muskxann/AI-attendance.git cd AI-attendance

*2*

#### Create a virtual environment

\# macOS / Linux python3 -m venv .venv source .venv/bin/activate # Windows PowerShell python -m venv .venv .\\.venv\\Scripts\\Activate.ps1

*3*

#### Install dependencies

pip install -r requirements.txt

*4*

#### Configure your database

SUPABASE_URL=your_supabase_project_url SUPABASE_KEY=your_supabase_key

*5*

#### Run the app

streamlit run app.py

Project structure

**AI-attendance/** ├── app.py ├── requirements.txt ├── assets/ └── src/ ├── components/ ├── database/ ├── pipelines/ ├── screens/ └── ui/

Handle biometrics with care

Facial and speaker embeddings are sensitive biometric data. Keep credentials out of source control, restrict database access, collect consent, and set clear retention policies before deploying.

M

Creator

### Muskan Mundra

Electronics & Instrumentation Engineering student and AI/ML developer, building practical AI-powered systems.

[@muskxann on GitHub](https://github.com/muskxann)

## Making attendance smarter, one classroom at a time.

Explore the code, try it locally, and give the project a star if you like it.

[★ Star on GitHub](https://github.com/muskxann/AI-attendance)

© 2026 Smart Attendance · Built with Python, Streamlit & AI/ML[github.com/muskxann/AI-attendance](https://github.com/muskxann/AI-attendance)