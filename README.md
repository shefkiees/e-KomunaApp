# e-Komuna
## Municipal Service Mobile Application – Project Proposal

---

## Project Overview

### App Name
**e-Komuna**

---

### One-Sentence Description
A mobile application that allows citizens to access municipal services, view local announcements, and report community issues directly from their smartphone.

---

## Problem Statement
Citizens often struggle to find up-to-date information about municipal services and announcements. Reporting issues such as broken streetlights, trash problems, or other local concerns usually requires visiting offices or making phone calls, which is time-consuming and inefficient.

---

## Target Users
- **Primary Users:** Residents of the municipality (citizens aged 18+)  
- **Secondary Users:** Municipal staff (admins)  
- **Potential Users:** Thousands of residents in a town or city  

---

## Why They Need This App
Citizens need a simple, centralized way to access information, submit requests, and report issues without wasting time or effort.

---

## The Problem
- **Pain Point:** Fragmented information and slow communication with municipal authorities  
- **Current Handling:** Websites, social media, phone calls, or in-person visits  
- **Inadequacy:** Existing solutions are not mobile-friendly, are time-consuming, and often result in delays or miscommunication  

---

## Solution & Features

### Core Features (MVP)

#### User Authentication
Citizens can create an account and log in securely.  
**User Story:**  
_As a citizen, I want to log in so that I can access personalized municipal services._

---

#### Municipal Announcements
View official announcements and local news published by the municipality.  
**User Story:**  
_As a citizen, I want to see municipal announcements so that I stay informed about community updates._

---

#### Issue Reporting
Citizens can report local issues with a text description and optional photo.  
**User Story:**  
_As a citizen, I want to report local problems so that the municipality can address them promptly._

---

#### Service Requests
Submit requests for municipal services such as appointments or document requests.  
**User Story:**  
_As a citizen, I want to request municipal services online so that I avoid visiting offices physically._

---

#### Admin Dashboard
Municipal staff can view and manage submitted reports.  
**User Story:**  
_As a municipal employee, I want to manage citizen reports so that I can respond efficiently._

---

### Secondary Features
- Push notifications for new announcements  
- Status tracking for reported issues  
- Map view to locate reported issues  

---

### Out of Scope
- Online payments  
- Legal document processing  
- Multi-city support  
- Integration with government backend systems  

---

## Technical Architecture

### User Authentication
- Supabase Authentication (Email & Password)  
- User Roles: **Citizen**, **Admin**

---

### Database Schema (Supabase – PostgreSQL)

**users**
- id  
- name  
- email  
- role  
- created_at  

**announcements**
- id  
- title  
- description  
- created_at  

**reports**
- id  
- user_id  
- category  
- description  
- image_url  
- status  
- created_at  

---

### External API
- **Google Maps API** for tagging locations of reported issues

---

## Key Technologies
- **Frontend:** React Native with Expo  
- **Backend:** Supabase (PostgreSQL Database, Authentication, Storage)  
- **Libraries:**  
  - React Navigation  
  - Expo Image Picker  
  - Expo Location  

---

## User Flow & Screens

### Main User Journey
1. Open app and log in or register  
2. Home screen displays announcements  
3. User navigates to report an issue  
4. User submits report and receives confirmation  
5. Admin reviews and updates report status  

---

### Screens
- Login / Register  
- Home (Announcements Feed)  
- Report Issue Screen  
- My Reports Screen  
- Admin Panel  
- Profile Screen  

---

## Challenges & Risks
- Image upload might be slow or fail  
- Feature creep during development  

### Backup Plan
If image upload is too complex, the app will allow text-only issue submissions.

---

## Success Metrics
- Core features work on both iOS and Android  
- Data persists correctly  
- Intuitive UI and smooth navigation  
- Team understands the full codebase and maintains a proper Git workflow  

---

## Why This Project Matters
- **Personal Motivation:** Frustration with current municipal communication systems  
- **Real-World Impact:** Citizens save time and municipalities improve responsiveness  

---
