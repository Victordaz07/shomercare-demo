<div align="center">

<img src="assets/app-icon.png" alt="ShomerCare" width="110">

# ShomerCare
### Custodial Zone Management System

**A secure, offline-first PWA for managing custodial teams, shift coverage, and zone assignments — built entirely in a single HTML file.**

[![HTML](https://img.shields.io/badge/HTML-Single%20File-E34F26?style=flat-square&logo=html5&logoColor=white)](shomercare-demo.html)
[![CSS](https://img.shields.io/badge/CSS-Vanilla-1572B6?style=flat-square&logo=css3&logoColor=white)](shomercare-demo.html)
[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla%20ES6-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](shomercare-demo.html)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Built with](https://img.shields.io/badge/Built%20with-❤️%20%26%20Claude%20AI-7c6fff?style=flat-square)](https://claude.ai)

[📖 User Guide](#-in-app-user-guide) · [🔐 Security](#-security) · [📬 Contact](#-contact)

---

<img src="assets/dashboard-zones.jpg" alt="ShomerCare Dashboard" width="340">

</div>

---

## 🧩 The Problem It Solves

Managing a custodial team in a large facility is surprisingly complex. Supervisors face:

- **Coverage gaps** — not knowing which areas are uncovered until it's too late
- **Scheduling from memory** — no visual system to track who covers what, when
- **Day-off chaos** — when someone calls out, finding a replacement is manual and stressful
- **No communication tool** — schedules live on paper or in someone's head
- **Inflexible time windows** — different days have different available cleaning windows that must respect when the building is in use

ShomerCare was built specifically to solve all of this — in a single HTML file, with no server, no account, and no internet required.

---

## ✨ Features

### 🏛️ Zone Coverage Management

Real-time tracking across **5 critical zones** and **3 work windows per day**. Coverage percentage updates instantly as you assign people. Each zone shows its own status badge and alerts when uncovered.

<div align="center">
<img src="assets/dashboard-stats.jpg" alt="Coverage Stats" width="270"> &nbsp; <img src="assets/zone-modal.jpg" alt="Zone Assignment Modal" width="270">
</div>

- **5 critical zones** with per-zone, per-window visual tracking
- **3 work windows** (Morning · Midday · Evening) — all times fully editable
- Real-time coverage % with color-coded status badges
- Visual alert when any zone is uncovered

---

### 👥 Smart Team Profiles

Every collaborator gets a full profile with 4 tabs: **Info**, **Schedule**, **Zones**, and **Days Off**. The schedule grid lets you set exactly which day/window each person works. Zone assignments power the smart replacement engine.

<div align="center">
<img src="assets/team-info.jpg" alt="Team Profile Info" width="230"> &nbsp; <img src="assets/team-schedule.jpg" alt="Team Schedule Grid" width="230"> &nbsp; <img src="assets/team-zones.jpg" alt="Team Zone Assignments" width="230">
</div>

- Full profiles: name, ID, WhatsApp, type (Full/Part)
- **Per-day, per-window schedule grid** — precise availability per person
- Primary zone assignments for smart replacement suggestions
- Color-coded team chips across the entire interface
- Supervisor private notes per person

---

### 📅 Days Off & Smart Replacements

Add a day off for any collaborator with date and optional reason. The app instantly marks ⚠️ alerts in every slot that person was assigned and surfaces replacements in 3 tiers.

<div align="center">
<img src="assets/days-off-list.jpg" alt="Days Off List" width="230"> &nbsp; <img src="assets/add-day-off.jpg" alt="Add Day Off" width="230"> &nbsp; <img src="assets/person-picker.jpg" alt="Smart Person Picker" width="230">
</div>

- Add day-off dates with optional reason per collaborator
- Automatic red alert ⚠️ where the absent person was assigned
- **3-tier replacement system:**
  - 🟢 **Primary team** — zone teammates available this window
  - 🟡 **Available** — anyone else with open availability
  - 🔴 **Outside regular hours** — triggers 5-second override warning
- Non-destructive: original assignment restored when person returns

---

### 💾 Save, Share & Print

Every change auto-saves. Share the day's full schedule via WhatsApp with one tap. If coverage is incomplete, an override flow lets you share anyway with a note to the team.

<div align="center">
<img src="assets/progress-saved.jpg" alt="Progress Saved Toast" width="270"> &nbsp; <img src="assets/coverage-alert.jpg" alt="Day Not Fully Covered" width="270">
</div>

- **Auto-save** on every change + manual save button
- **Share Day** — WhatsApp message with full schedule + optional note
- **Share Week** — appears on Fridays when Mon–Fri are all complete
- Incomplete day sharing with override option and team note
- Day notes included in WhatsApp and printed output

---

### 🖨️ Print-Ready Weekly Schedule

Professional print layout — one table per day, color-coded team legend, day notes, day-off alerts (⚠️ red), and supervisor name + timestamp in the footer.

---

### 🌍 Trilingual Interface

Switch instantly between **English · Spanish · Tongan** from the header. All UI elements, messages, WhatsApp content, and print output translate completely.

---

### 🔄 Cross-Device Sync

<div align="center">
<img src="assets/sync-qr.jpg" alt="Sync and QR Code" width="320">
</div>

- **QR Code** — generate on PC, scan on phone to load all data instantly
- **JSON Export/Import** — send file via WhatsApp/email, import on any device
- 5-second countdown + explicit warning before any import (prevents accidental data loss)

---

### ⚙️ Fully Configurable

<div align="center">
<img src="assets/settings.jpg" alt="Settings and Configuration" width="320">
</div>

- Temple/facility name, supervisor info, photo
- Working days toggle (on/off per day)
- **Editable work windows** — change start/end times per day per window on the fly
- Reset to defaults option

---

### 🔐 PIN Lock System

<div align="center">
<img src="assets/splash.jpg" alt="Splash Screen" width="255"> &nbsp; <img src="assets/pin-lock.jpg" alt="PIN Entry Screen" width="255">
</div>

- Secure 6-digit PIN required to access the app
- First-launch PIN registration flow with confirmation
- 3-attempt limit with auto-reset and developer contact info
- Change PIN from a hidden menu (3-tap secret access)
- Lock app button from within the Easter egg panel

---

### 📖 In-App User Guide

<div align="center">
<img src="assets/user-guide.jpg" alt="In-App User Guide" width="320">
</div>

Built-in accordion tutorial covering every feature — no external docs needed.

---

### ⚛️ Easter Egg

Hidden React atom ⚛️ at the bottom of the dashboard. Tap it to reveal developer info and app controls.

---

## 🚀 Getting Started

**No installation. No server. No account.**

```bash
# 1. Clone the repo
git clone https://github.com/Victordaz07/shomercare-demo.git

# 2. Open the file in any modern browser
open shomercare-demo.html
# or just double-click the file
```

> ✅ Works on Chrome, Safari, Firefox — mobile and desktop.

### First Launch
1. Create your 6-digit PIN when prompted
2. Go to **⚙️ Sync** → enter your facility name and supervisor info
3. Configure **Working Days** and adjust window times if needed
4. Go to **👥 Team** → tap each person to set their schedule and zones
5. Return to **📊 Dashboard** → start assigning zones

---

## 🏗️ Architecture

```
shomercare-demo.html     ← entire application (single file)
│
├── CSS (~500 lines)     CSS variables, responsive layout, animations
├── HTML (~800 lines)    Views, modals, lock screen, nav
└── JavaScript
    ├── Translations     EN / ES / TO dictionary
    ├── Data Layer       localStorage with validation & sanitization
    ├── PIN System       Registration, unlock, change PIN, master key
    ├── Dashboard        Zone rendering, coverage calculation, FAB
    ├── Team Profiles    Rich profiles with schedule grid
    ├── Days Off         Date management, replacement suggestions
    ├── Sync             QR generation, JSON export/import
    ├── Print            Weekly schedule builder
    ├── Share            WhatsApp message builder
    └── Guide            In-app tutorial (accordion)
```

**No dependencies.** No npm. No build step. No framework.
One file. Open it. Done.

---

## 🔐 Security

ShomerCare handles sensitive personnel and scheduling data. Multiple layers of protection:

| Layer | Implementation |
|---|---|
| **Local-only storage** | All data stays on device — nothing sent to any server |
| **Content Security Policy** | `<meta>` CSP header blocks unauthorized scripts |
| **Input sanitization** | All user inputs stripped of HTML tags before storage |
| **Import validation** | JSON imports fully validated and sanitized before loading |
| **Photo validation** | Image uploads validated by type and size (2MB max) |
| **PIN lock** | 6-digit PIN required to access the app |
| **Destructive action countdowns** | 5-second forced delay on imports and overrides |
| **No-referrer policy** | Prevents data leakage when navigating to external URLs |

> ⚠️ **Note:** This is a client-side application. Data is stored in `localStorage`. Keep your device locked when not in use.

---

## 📁 Repo Structure

```
shomercare-demo/
├── shomercare-demo.html   ← Public demo (generic team, no master key)
├── assets/                ← App icon + 17 screenshots
├── README.md
└── LICENSE
```

> The production version (with real team data) is maintained in a private repository.

---

## 💡 Design Philosophy

> *"Everything a supervisor needs. Nothing they don't."*

ShomerCare was designed as a **vibe coding experiment** — starting from a basic Excel scheduling problem and evolving into a full-featured management system through iterative conversation with Claude AI.

Key decisions:
- **Single HTML file** — zero friction deployment, works offline, easy to share
- **No framework** — vanilla JS is fast, transparent, and requires no build tools
- **Mobile-first** — designed for a supervisor's phone, not a desktop workstation
- **Elegant aesthetic** — cream/gold palette inspired by the facility's sacred character
- **Trilingual** — serves diverse custodial teams natively

---

## 🛠️ Customization

ShomerCare is designed to be adapted for any facility with custodial zones:

1. **Rename zones** — edit the `ZIDS` and `ZONE_ICONS` arrays and translation strings
2. **Add/remove work windows** — edit `appSettings.windows` defaults
3. **Change language** — add entries to the `T` translation object
4. **Rebrand** — update app name, icon, and color variables in `:root`

---

## 📬 Contact

**Victor Ruiz** — Frontend Developer & Vibe Coder

[![GitHub](https://img.shields.io/badge/GitHub-Victordaz07-181717?style=flat-square&logo=github)](https://github.com/Victordaz07)
[![Email](https://img.shields.io/badge/Email-viruizbc%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:viruizbc@gmail.com)
[![Instagram](https://img.shields.io/badge/Instagram-@alfonsorb07-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://instagram.com/alfonsorb07)
[![Portfolio](https://img.shields.io/badge/Portfolio-portarts.dev-b8963e?style=flat-square&logo=safari&logoColor=white)](https://portarts.dev)

> Available for custom development, feature additions, and improvements on request.

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**Built with ❤️ and Claude AI · ShomerCare v1.0 · 2026**

*"Shomer" (שׁוֹמֵר) — Hebrew for Guardian, Protector, Keeper*

⚛️

</div>
