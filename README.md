<div align="center">

<img src="https://img.shields.io/badge/Student%20Marks-Analyser-c84b2f?style=for-the-badge&logo=javascript&logoColor=white" alt="Student Marks Analyser Banner"/>

# 📊 Student Marks Analyser

### *Professional Grade Manager with Live Stats, Charts, Search & CSV Export*

<br/>

[![Live Demo](https://img.shields.io/badge/🌐%20Live%20Demo-GitHub%20Pages-c84b2f?style=for-the-badge)](https://manikanta-04.github.io/Students_marks_Analyser_website/)

<br/>

[![HTML5](https://img.shields.io/badge/HTML5-Structure-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Animations-1572B6?style=flat-square&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/Vanilla%20JS-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![localStorage](https://img.shields.io/badge/localStorage-Persistent-brightgreen?style=flat-square)]()
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-brightgreen?style=flat-square)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
![GitHub repo size](https://img.shields.io/github/repo-size/Manikanta-04/Students_marks_Analyser_website?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/Manikanta-04/Students_marks_Analyser_website?style=flat-square)

</div>

---

## 🚀 Live Demo

| Service | URL |
|---|---|
| 🌐 **Student Marks Analyser** | [manikanta-04.github.io/Students_marks_Analyser_website](https://manikanta-04.github.io/Students_marks_Analyser_website/) |

> 💡 Open and start managing student grades instantly — no login, no install, data persists via localStorage.

---

## 🎥 Demo Video

> 📽️ *(Add a Loom / YouTube demo walkthrough here)*
>
> [![Watch Demo](https://img.shields.io/badge/▶%20Watch%20Demo-YouTube-red?style=for-the-badge&logo=youtube)](https://youtube.com)

---

## 🧠 Problem Statement

Teachers and faculty managing student grades face daily friction with existing tools:

- 📋 Excel spreadsheets require manual formula setup — no auto-grading, no charts
- 🌐 Google Sheets needs internet + Google account just to view class averages
- 🐌 Full school ERP systems (like Fedena) are overkill for a single teacher's gradebook
- 📊 No lightweight tool offers instant grade badges, progress bars, and distribution charts together
- 💾 Browser-based tools reset data on refresh — no persistence

**Teachers need a zero-install gradebook that just works — fast, visual, and persistent.**

---

## 💡 Solution

**Student Marks Analyser** is a professional single-file gradebook packed into one `index.html`. Add students with up to 3 subjects, get instant grade badges, color-coded marks, progress bars, live dashboard stats, distribution charts, search/filter/sort, and CSV export — all persisted via `localStorage` with zero dependencies.

> *"Track every mark. See every trend."*

---

## 🖼️ Screenshots

| Main Dashboard | Grade Badges & Progress Bars |
|---|---|
| ![Dashboard](screenshots/dashboard.png) | ![Grades](screenshots/grades.png) |

| Score Distribution Chart | Grade Distribution |
|---|---|
| ![Chart](screenshots/chart.png) | ![Distribution](screenshots/distribution.png) |

| Add Student Form | CSV Export |
|---|---|
| ![Add](screenshots/add.png) | ![Export](screenshots/export.png) |

> 📌 *(Replace with actual screenshots from your deployed app)*

---

## 🏗️ Architecture

```
┌──────────────────────────────────────────────────────────┐
│              SINGLE FILE APP — index.html                 │
│                                                           │
│  ┌──────────────────────────────────────────────────┐     │
│  │              CSS LAYER                            │     │
│  │  Warm paper tone palette | Red accent (#c84b2f)   │     │
│  │  Editorial serif headings | Monospace data cells  │     │
│  │  Color-coded mark cells | Progress bar animations │     │
│  │  Sticky header | Responsive grid layout           │     │
│  └──────────────────────────────────────────────────┘     │
│                                                           │
│  ┌──────────────────────────────────────────────────┐     │
│  │         JAVASCRIPT DATA ENGINE                    │     │
│  │  studentStore[]      → in-memory + localStorage  │     │
│  │  addStudent()        → push + save + re-render   │     │
│  │  editStudent()       → update entry + re-render  │     │
│  │  deleteStudent()     → splice + save + re-render │     │
│  │  calculateGrade()    → average → A/B/C/D/F badge │     │
│  │  colorCodeMark()     → Green/Amber/Red per mark   │     │
│  │  updateDashboard()   → total, avg, highest, pass% │     │
│  │  renderCharts()      → score + grade distribution │     │
│  │  searchFilter()      → name/ID/subject/grade      │     │
│  │  sortTable()         → name/avg/ID ascending/desc │     │
│  │  exportCSV()         → Blob → download .csv       │     │
│  │  loadFromStorage()   → localStorage.getItem()     │     │
│  │  saveToStorage()     → localStorage.setItem()     │     │
│  └──────────────────────────────────────────────────┘     │
│                                                           │
│  CDN: Google Fonts (DM Serif Display + DM Mono + Syne)    │
└──────────────────────────────────────────────────────────┘
```

---

## ⚙️ Tech Stack

| Layer | Technology | Purpose |
|---|---|---|
| **Structure** | HTML5 | Single-page markup |
| **Styling** | CSS3 | Warm palette, animations, responsive grid |
| **Logic** | Vanilla JavaScript ES6+ | CRUD, grading, charts, search, sort |
| **Persistence** | localStorage API | Data survives page refresh |
| **Export** | Blob + URL API | CSV file download |
| **Fonts** | Google Fonts CDN | DM Serif Display + DM Mono + Syne |
| **Hosting** | GitHub Pages | Free static hosting |

> ⚡ **Zero local dependencies** — no npm, no Chart.js, no frameworks. Pure browser APIs only.

---

## ✨ Features

### 🎓 Student CRUD
- **Add** students with name, ID, subject, and up to 3 subject marks
- **Edit** any student record inline
- **Delete** students with a single click

### 📊 Live Dashboard Stats (auto-updates)
| Stat | Description |
|---|---|
| Total Students | Count of all registered students |
| Class Average | Mean average across all students |
| Highest Mark | Top score in the class |
| Pass Rate | % of students scoring above pass threshold |

### 🏅 Automatic Grade Badges
| Grade | Range |
|---|---|
| A | 90–100 |
| B | 75–89 |
| C | 60–74 |
| D | 45–59 |
| F | Below 45 |

### 🎨 Color-Coded Marks
| Color | Meaning |
|---|---|
| 🟢 Green | Good (above average) |
| 🟡 Amber | Average (near pass mark) |
| 🔴 Red | Below pass threshold |

### 📈 Visual Progress Bars
- Per-student horizontal progress bar
- Width reflects average score percentage
- Color matches grade band

### 📉 Distribution Charts
- **Score Distribution** — bar chart across 5 score bands (0–20, 21–40, 41–60, 61–80, 81–100)
- **Grade Distribution** — breakdown of A/B/C/D/F counts across the class

### 🔍 Search, Filter & Sort
- **Search** by student name or ID
- **Filter** by subject or grade
- **Sort** by name, average score (asc/desc), or student ID

### 💾 CSV Export
- Download full gradebook as `.csv`
- Includes all student fields, subject marks, averages, and grades

### 🗄️ localStorage Persistence
- All data saved automatically on every change
- Survives page refresh, browser close, and reopen
- No backend, no cloud — fully private

---

## 📊 System Design

```
Data Flow — Add Student:

[User fills Add Student form]
         │
         ▼
[addStudent() validates fields]
         │
         ▼
[calculateGrade(avg) → A/B/C/D/F assigned]
[colorCodeMark(mark) → green/amber/red class]
         │
         ▼
[push to studentStore[]]
[saveToStorage() → localStorage.setItem()]
         │
         ├── renderTable()       → rebuilds student rows
         ├── updateDashboard()   → recalculates all 4 stats
         └── renderCharts()      → redraws both charts
```

```
Search / Filter / Sort Flow:

[User types in search bar OR changes filter dropdown OR clicks sort]
         │
         ▼
[searchFilter() → filters studentStore[] by name/ID/subject/grade]
[sortTable() → sorts filtered array by selected column + direction]
         │
         ▼
[renderTable(filteredArray) → only matching rows displayed]
[studentStore[] unchanged — filter is non-destructive]
```

```
CSV Export Flow:

[User clicks ↓ Export]
         │
         ▼
[exportCSV() → maps studentStore[] to CSV string]
[Blob created → URL.createObjectURL()]
         │
         ▼
[<a> tag triggered → gradebook.csv downloaded]
```

**Student Data Schema:**

```javascript
{
  id:       "STU001",
  name:     "Student Name",
  subjects: [
    { name: "Maths",   mark: 85 },
    { name: "Science", mark: 72 },
    { name: "English", mark: 90 }
  ],
  average:  82.3,
  grade:    "B",
  passed:   true
}
```

---

## 🔄 Workflow

```
1. User opens index.html / visits GitHub Pages URL
2. localStorage checked → existing data loaded and rendered
3. User clicks + Add Student → form modal opens
4. Fills name, ID, subject names, and marks
5. On submit → grade auto-calculated → color codes assigned
6. Student row added to table → dashboard stats + charts update
7. User searches/filters → table narrows in real time
8. User sorts → table reorders (studentStore unchanged)
9. User edits → form pre-filled → save → re-render
10. User deletes → row removed → all panels refresh
11. User clicks Export → gradebook.csv downloaded
```

---

## 📈 Performance & Metrics

| Metric | Value |
|---|---|
| Total files | 1 (single `index.html`) |
| External CDN | 1 (Google Fonts) |
| Subjects per student | Up to 3 |
| Grade tiers | 5 (A / B / C / D / F) |
| Color tiers | 3 (Green / Amber / Red) |
| Chart types | 2 (Score + Grade distribution) |
| Export format | CSV |
| Persistence | localStorage (client-side) |
| Build step | None |
| Framework | None |
| Time to load | < 1s |

---

## 🧪 Testing

```bash
# Open directly in browser
open index.html

# Or serve locally
npx serve .
# Visit: http://localhost:3000

# Manual test checklist:
# ✅ Page loads with data from localStorage (if any)
# ✅ Add student → table + dashboard + charts all update
# ✅ Grade badge auto-assigned (A/B/C/D/F) correctly
# ✅ Color-coded marks appear (green/amber/red)
# ✅ Progress bar width matches average score %
# ✅ Edit student → form pre-filled → save updates data
# ✅ Delete student → row removed, stats recalculated
# ✅ Search by name/ID → table filters in real time
# ✅ Filter by subject/grade → correct rows shown
# ✅ Sort by average descending → highest first
# ✅ Export → gradebook.csv downloaded with correct data
# ✅ Refresh page → data restored from localStorage
# ✅ Responsive at 375px (mobile)
```

### Browser Compatibility

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Mobile Chrome | ✅ Full |

---

## 📋 How to Use

| Action | How |
|---|---|
| Add student | Click **+ Add Student** → fill form → submit |
| Edit student | Click **✎** on any row → update → save |
| Delete student | Click **✕** on any row → confirm |
| Search | Type in the search bar (name or ID) |
| Filter | Use dropdown to filter by subject or grade |
| Sort | Click column headers for name / average / ID |
| Export | Click **↓ Export** → downloads `gradebook.csv` |

---

## 📁 Project Structure

```
Students_marks_Analyser_website/
│
├── index.html      # Entire app — HTML + CSS + JS (all-in-one)
└── README.md       # Project documentation
```

> Everything — CRUD logic, grade engine, charts, search, localStorage, CSV export — lives in **one self-contained `index.html` file.**

---

## 🎨 Design System

| Token | Value |
|---|---|
| Primary Accent | `#c84b2f` (Warm Red) |
| Background | Paper-tone warm white |
| Display Font | DM Serif Display |
| Mono Font | DM Mono (data cells) |
| Accent Font | Syne |
| Pass Mark Color | 🟢 Green |
| Average Color | 🟡 Amber |
| Fail Color | 🔴 Red |
| Layout | CSS Grid + Flexbox |

---

## 🔐 Security

- **No user data sent anywhere** — fully client-side, localStorage only
- **No backend** — zero server-side attack surface
- **No eval()** — all JS is safe DOM manipulation
- **GitHub Pages HTTPS** — all traffic served over SSL
- **Data privacy** — all grade data stays in the user's own browser

---

## ⚙️ Local Development Setup

### Prerequisites

- Any modern browser
- No Node.js, Python, or runtime required

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Manikanta-04/Students_marks_Analyser_website.git
cd Students_marks_Analyser_website
```

### 2️⃣ Open in Browser

```bash
open index.html
# OR
npx serve .
# Visit: http://localhost:3000
```

---

## 🔑 Environment Variables

No environment variables required — fully static, localStorage-based app.

---

## 🚀 Deployment

### GitHub Pages *(Already deployed)*

1. Push `index.html` to `main` branch
2. Go to **Settings → Pages**
3. Source: `main` branch → `/ (root)`
4. Live at: `https://manikanta-04.github.io/Students_marks_Analyser_website/`

### Vercel / Netlify

| Setting | Value |
|---|---|
| Framework | Other / Static |
| Build Command | *(leave empty)* |
| Output Directory | `./` |

---

## 🔮 Future Improvements

- [ ] 📚 Unlimited subjects per student (not capped at 3)
- [ ] 📥 CSV import — bulk upload from Excel/Sheets
- [ ] 🖨️ Print-ready report card per student
- [ ] 📧 Email report card as PDF (EmailJS)
- [ ] 🏫 Multi-class support — switch between class groups
- [ ] 🔔 Alert teacher when class pass rate drops below threshold
- [ ] 📱 PWA support — installable as mobile app
- [ ] ☁️ Cloud sync with Supabase for cross-device access

---

## 🤝 Contributing

Contributions are welcome and appreciated!

```bash
# 1. Fork this repository
# 2. Create your feature branch
git checkout -b feature/your-feature-name

# 3. Commit with conventional commits
git commit -m "feat: describe your change"

# 4. Push and open a Pull Request
git push origin feature/your-feature-name
```

---

## 👨‍💻 Author

**Manikanta Naripeddi** — Full Stack & Creative Developer

[![GitHub](https://img.shields.io/badge/GitHub-Manikanta--04-181717?style=flat-square&logo=github)](https://github.com/Manikanta-04)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Manikanta%20Naripeddi-0077b5?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/manikanta-naripeddi-4326232a5/)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

- [localStorage API](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) — Client-side data persistence
- [Blob + URL API](https://developer.mozilla.org/en-US/docs/Web/API/Blob) — CSV file export
- [Google Fonts](https://fonts.google.com/) — DM Serif Display + DM Mono + Syne
- [GitHub Pages](https://pages.github.com/) — Free static hosting

---

<div align="center">

**Built with ❤️ for teachers who just want a gradebook that works**

⭐ **Star this repo** if Student Marks Analyser saved you from a spreadsheet!

[![GitHub Stars](https://img.shields.io/github/stars/Manikanta-04/Students_marks_Analyser_website?style=social)](https://github.com/Manikanta-04/Students_marks_Analyser_website)

---

*📊 Track every mark. See every trend.*

</div>
