# MediRemind 🏥

> **Hackathon Project** — Medical Daily Medication Reminder & Appointment Reminder App

A hospital system that streamlines the doctor-to-patient prescription workflow, enabling patients to view their prescriptions and add medication and appointment reminders directly to their device calendar.

---

## 🎯 Objective

Bridge the gap between doctor consultation and patient compliance by:

- Allowing doctors to **issue digital prescriptions** directly after consultation
- Giving patients a clear, readable **prescription card** with medicine details and dosage
- Enabling patients to **set daily medication reminders** that sync to their device calendar
- Enabling patients to **set upcoming appointment reminders** with advance alerts

---

## ✨ Features

### 🩺 Doctor Side
- Fill in patient information (name, IC, age, gender)
- Enter diagnosis and attending doctor details
- Add multiple medicines with dosage, frequency, and duration
- Add doctor's notes and instructions
- Schedule next follow-up appointment (date, time, hospital, room)
- Issue the prescription to the patient with one click

### 📋 Patient Side
- View a formatted **digital prescription card** (Rx slip)
- See all prescribed medicines in a clear table with dosage badges
- View doctor's notes and next appointment details
- Navigate to the reminders screen

### ⏰ Reminder System
- **Daily Medication Reminder** — generates a `.ics` calendar file with a repeating daily event for each prescribed medicine, complete with an in-app notification alarm
- **Appointment Reminder** — generates a `.ics` calendar file for the upcoming appointment with two alerts:
  - 1 day before the appointment
  - 1 hour before the appointment
- Both `.ics` files are compatible with **iPhone Calendar**, **Android Calendar**, **Google Calendar**, and **Microsoft Outlook**

---

## 🚀 Getting Started

No installation or server required. This is a fully self-contained single-file web app.

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/bob-a-thon.git
   cd bob-a-thon
   ```

2. Open `index.html` in any modern browser:
   ```bash
   # macOS / Linux
   open index.html

   # Windows
   start index.html
   ```

That's it — the app runs entirely in the browser with no dependencies.

---

## 🗺️ Demo Flow

| Step | Action |
|------|--------|
| 1 | Doctor opens the app and fills in the prescription form (pre-filled for demo) |
| 2 | Click **"Issue Prescription to Patient"** |
| 3 | Patient view shows the formatted prescription card |
| 4 | Click **"Set Reminders"** |
| 5 | Click **"Add to Calendar"** for medication → `.ics` file downloads → open to add daily reminders |
| 6 | Click **"Add to Calendar"** for appointment → `.ics` file downloads → open to add appointment with alerts |

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | App structure |
| CSS3 | Styling and responsive layout |
| Vanilla JavaScript | App logic, screen navigation, form handling |
| iCalendar (.ics) format | Cross-platform calendar integration |
| Blob API | Client-side file generation and download |

---

## 📂 Project Structure

```
bob-a-thon/
├── index.html   # Complete single-file app (UI + logic)
└── README.md    # Project documentation
```

---

## 📱 Calendar Compatibility

The generated `.ics` reminder files work natively with:

- 🍎 Apple iPhone / iPad Calendar
- 🤖 Android Google Calendar
- 📧 Microsoft Outlook
- 📅 Google Calendar (import)

---

## 👥 Team

Built at **IBM Bob-a-thon Hackathon**

---

*Made with ❤️ and IBM Bob*
