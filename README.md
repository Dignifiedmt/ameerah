# TalentViolet - Job Tracking & Recruitment Platform

A modern, responsive job tracking and recruitment web application built with **React**, styled with **Tailwind CSS**, and featuring a signature **Light Purple & Lavender aesthetic**.

---

## 🌟 Key Features

### 👤 Job Seeker (Normal User) Experience
- **Explore & Filter Openings**: Real-time keyword search across job titles, company names, and tech skills. Filter by department (Engineering, Design, Product, Marketing), employment type (Remote, Full-time, Hybrid, Contract), and experience level.
- **Quick Filters**: One-click pills for *"⚡ Remote Only"*, *"💻 Engineering"*, *"🎨 UI/UX Design"*, and *"⭐ Senior Roles"*.
- **Comprehensive Job Details Modal**: View in-depth responsibilities, requirements, benefits & perks (401k, remote stipend, PTO), and technology tags.
- **Streamlined Application Form**:
  - Pre-filled candidate details or custom input.
  - Resume attachment simulator (supports PDF/DOCX with file size validation).
  - Years of experience, expected compensation, portfolio/LinkedIn link, and personalized cover letter.
- **"My Applications" Real-Time Tracker**:
  - Interactive 4-stage visual pipeline tracker:
    1. 📝 **Applied**
    2. 🔍 **Under Review**
    3. 🎙️ **Interviewing**
    4. 🎉 **Offer Extended / Decision**
  - Live status pills and recruiter feedback notes.
  - Option to view submitted details or withdraw an application.
- **Saved Roles**: One-click bookmarking to save opportunities for later review.

---

### 🛡️ Admin (Hiring Manager / Recruiter) Experience
- **Admin Dashboard & Live KPIs**:
  - Metrics overview: *Active Job Postings*, *Total Applicants*, *In Interview Stage*, and *Offers Extended*.
- **Job Postings Management**:
  - Create new job postings with rich configuration (title, department, workplace policy, salary min/max, deadline, description, requirements, benefits, and skill tags).
  - Edit existing job postings anytime.
  - Toggle job status between `Active` and `Paused` (paused postings are automatically hidden from normal users).
  - Delete postings with safety confirmation.
  - View applicant count badges per job.
- **Applicant Tracking System (ATS Pipeline)**:
  - Filter candidates by specific job opening or recruitment stage.
  - Candidate cards showing contact information, experience, desired compensation, resume attachment, and cover letter excerpt.
  - **Candidate Detail & Interview Notes Modal**:
    - Full candidate summary and contact links (Email, LinkedIn, Phone).
    - Status changer: advance candidates between `Applied` ➔ `Under Review` ➔ `Interviewing` ➔ `Offered` ➔ `Rejected`.
    - Internal hiring team notes field for feedback and evaluation notes (persisted to storage).

---

## 🎨 Design & Palette: Light Purple Aesthetic
- **Primary Brand Purple**: `#9D6BF7` / `#8643E8`
- **Soft Lavender Backgrounds**: `#FAF8FF` / `#F3ECFE`
- **Borders & Dividers**: Subtle soft violet `#E6D7FE` / `#D5BBFD`
- **Elevations**: Soft ambient purple glow shadows (`shadow-purple-sm`, `shadow-purple-md`)
- **Typography**: Clean, modern typography using *Plus Jakarta Sans* and *Inter*.

---

## 🚀 How to Run the Application

### Option 1: Direct Browser Launch (Zero Setup)
Simply double-click `start.bat` or open `index.html` directly in your browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Brave, etc.).
- No build tools, package managers, or local dependencies needed.
- Uses standard React 18 and Tailwind CSS CDN.

### Option 2: Local HTTP Server (PowerShell)
If you prefer running through `http://localhost:3000`:
1. Open PowerShell in this directory:
   ```powershell
   powershell -ExecutionPolicy Bypass -File .\server.ps1
   ```
2. The server will start on port 3000 and automatically open your default browser.

---

## 💾 Data Persistence
- All state (job postings, applications, recruiter notes, bookmarks, and user roles) is saved automatically in the browser's `localStorage` (`talentviolet_*`).
- Changes made as an applicant or admin remain saved across page refreshes.
- To restore the pre-seeded demo dataset at any time, click the **Reset (↺)** button in the top navigation bar.

