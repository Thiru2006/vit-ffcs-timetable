# VIT FFCS Timetable Builder — Winter Semester 2026-27

A free, browser-based FFCS timetable planner for **VIT Chennai**. Search the offered
courses, pick your faculty, and the tool builds your timetable on the official slot
grid in real time — flagging any **slot clashes** instantly and pairing each **lab with
the same faculty as its theory**.

🔗 **Live site:** https://thiru2006.github.io/vit-ffcs-timetable/

![Winter Semester 2026-27](https://img.shields.io/badge/Semester-Winter%202026--27-574bd4) ![Courses](https://img.shields.io/badge/Courses-718-1f5f94) ![License](https://img.shields.io/badge/License-MIT-17935f)

## Features

- **Search 718 offered courses** by code or title, with a quick school filter.
- **Real-time timetable** rendered on the official VIT FFCS slot grid (A1–G2, theory
  slots, and labs L1–L60).
- **Instant clash detection** — overlapping slots turn red and a banner lists exactly
  which courses conflict and on which day/time.
- **Labs follow the theory faculty** automatically. If a faculty teaches more than one
  lab slot, you can switch between them from a dropdown.
- **Live credit & clash counters**, light/dark theme, and your plan is saved in the
  browser so it's there when you come back.
- **Off-grid handling** for law-school and postgraduate slot systems, so those courses
  still clash-check correctly even though they sit outside the B.Tech grid.

## How it works

1. Search for a course and click it.
2. Pick a section — a green dot means it's clash-free with your current plan, a red dot
   warns you before you add it.
3. The grid and credit total update immediately. Resolve any clash by switching the
   faculty, section, or lab slot.

## Data

Course data was parsed from the official **Winter Semester 2026-27 Course Offered List**
published by VIT. This is a planning aid only — always confirm your final slots in the
**VTOP** course registration portal, as offerings can change.

## Run locally

It's a single static page with no build step or dependencies. Clone and open `index.html`
in a browser, or serve the folder:

```bash
git clone https://github.com/Thiru2006/vit-ffcs-timetable.git
cd vit-ffcs-timetable
python3 -m http.server 8000   # then open http://localhost:8000
```

## Tech

Plain HTML, CSS, and vanilla JavaScript — no frameworks. All course data is embedded in
the page, so it works fully offline once loaded.

## License

[MIT](LICENSE) © 2026 Thirugnanam V S

---

*Not an official VIT product. Made by a student to make registration day less painful.*
