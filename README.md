# EduPulse — Student Curriculum & Attendance System

EduPulse is a web-based academic tracking prototype that brings student attendance, curriculum progress, and study notes together in one place. It provides separate student and teacher portals, attendance analytics, and visual indicators to help students understand their attendance status before exams.

**Live Demo:** https://edupulse-one-fawn.vercel.app/

## Project Overview

Manual attendance registers, disconnected syllabus records, and late shortage warnings can make academic tracking difficult. EduPulse presents attendance and curriculum progress through a unified interface designed for students, faculty, and academic administrators.

## Key Features

### Student Portal
- View overall and subject-wise attendance percentages.
- Review attendance history through a 30-session visual heatmap.
- See whether attendance is **Safe (75% or above)**, **At Risk (65%–74%)**, or **Critical (below 65%)**.
- Estimate how many classes can still be missed or how many consecutive classes are needed to reach 75%.
- Track curriculum topics with unit-wise checklists and progress indicators.
- Read subject-specific study notes.
- Add or remove subjects from the student's dashboard.

### Teacher Portal
- Mark students as **Present**, **Absent**, or **Late**.
- Submit attendance by subject and date.
- Use keyboard shortcuts (`P`, `A`, and `L`) to mark attendance, with arrow-key navigation between student cards.
- Review the class average and identify students below the 75% attendance threshold.
- Sort the student roster by attendance percentage.
- Mark curriculum units as taught so students can follow syllabus progress.

### Interface
- Responsive layout for desktop and mobile screens.
- Light and dark theme options.
- Demo-data reset option.
- Attendance records and interface state are stored in the browser's local storage in this prototype.

## Subjects Included

| Code | Subject | Credits |
|---|---|---:|
| MFC | Mathematics for Computation | 4 |
| PJ | Programming in Java | 4 |
| DDCA | Digital Design and Computer Architecture | 4 |
| LSE | Language Skills for Engineering | 2 |

## Demo Login

The current prototype includes sample credentials for demonstration.

**Teacher**
- Email: `teacher01@edupulse.in`
- Password: `Teach@123`

**Students**
- Email: `aarav@edupulse.in`, `diya@edupulse.in`, `rohan@edupulse.in`, and other sample student usernames shown in the login form.
- Password for sample student accounts: `Student@123`

Select the appropriate role on the sign-in screen, then use the demo credentials. These are public demonstration credentials, not secure production credentials. Do not use real or sensitive information with this prototype.

## Attendance Calculation

The prototype counts a **Present** session as full credit and a **Late** session as half credit when the half-attendance setting is enabled. The attendance percentage is calculated as:

`Attendance % = (Present sessions + 0.5 × Late sessions) / Total sessions × 100`

The dashboard displays status bands:
- **Safe:** 75% or higher
- **At Risk:** 65% to 74%
- **Critical:** below 65%

The calculator provides an estimate of classes that may be missed while remaining at 75%, or the number of consecutive classes to attend to recover to 75%.

## Technology

- **HTML5** — page structure
- **CSS3** — styling, responsive layout, themes, and transitions
- **JavaScript** — interface rendering, attendance calculations, curriculum tracking, and interactions
- **Browser Local Storage** — persistence of prototype data in the current browser
- **Vercel** — live web deployment

The uploaded prototype is implemented as a standalone HTML file with embedded CSS and JavaScript.

## Run Locally

1. Download or clone this repository.
2. Open `EduPulse.html` in a modern web browser.
3. Select **Sign in**, choose the Student or Teacher role, and use the demo credentials above.

No build step is required for the standalone HTML prototype. An internet connection may be needed to load the external Google Fonts used by the interface.

## Project Team

| Team Member | Student ID |
|---|---|
| Jayanth Talari | `2620090100` |
| Vinay | `2620030387` |
| Vikas Chinta | `2620030391` |
| Mokshit Reddy | `2620030124` |
| Charan | `2620080093` |
| Navaneeth | `2620030694` |

## Project Context

- **Course:** Design Thinking for Innovation & Entrepreneurship (DTIE)
- **Project Batch:** Batch-A
- **Project Name:** EduPulse — Student Curriculum & Attendance System

## Future Improvements

- Connect a secure backend and database for shared, persistent records.
- Add real authentication, password management, and role-based authorization.
- Introduce automated attendance-shortage notifications.
- Support institution-wide deployment and multiple colleges.
- Add audit logs, data export, and administrative reporting.

## Important Note

EduPulse is a demonstration prototype. Its current sample data and browser-based storage are intended for showcasing the workflow; they should not be treated as a secure, institution-ready attendance system.

---
Made with care by **Team EduPulse**.
