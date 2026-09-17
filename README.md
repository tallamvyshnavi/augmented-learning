# augmented-learning
# Augmented Learning Workbench

A browser tool for running the Augmented Learning (remedial class) process at VFSTR: identifying students who need academic support, scheduling the classes, and producing Annexures I–IV, the student notices and the faculty pack.

## Live Site

https://YOUR-USERNAME.github.io/augmented-learning/

## What it does

1. **Roster** — reads the branch-wise student master workbook from the Dean's office. All sheets are merged and duplicate registration numbers removed.

2. **FA-1 / FA-2 marks** — reads the assessment workbooks exactly as faculty send them. Course names, course codes, which assessment it is and the maximum marks are taken from the file's own header rows, so FA-1 out of 10 and FA-2 out of 20 need no configuration.

3. **Data check** — absent students, courses whose marks have not arrived, and registration numbers that do not match the roster are all surfaced for a decision. Nothing is corrected silently.

4. **Criteria** — Module-1 below 50% and backlog (I/R) are the primary criteria from the circular. CGPA and attendance are optional and off by default.

5. **Subject-wise lists** — a student appears once per subject they need help in. The section total counts each student once, never the sum of the columns.

6. **Time-table** — one subject per day, with checks for students expected in two places, double-booked faculty or rooms, and classes before 3:10 PM.

7. **Annexures I–IV** — in the prescribed layout, exportable.

8. **Notices and faculty pack** — student documents carry registration number, name, subject, day, time, room and faculty only. No marks, no CGPA, no backlog, no reason.

## Privacy

Everything runs in the browser. No student data is uploaded, transmitted or stored anywhere. Closing the tab clears it. There is no server, no database and no account.

Because of this, nothing is saved between visits — the files are uploaded again each session.

## Hosting

`index.html` is a single self-contained file. Every library it needs is built in, so it works with no internet connection. Serve the file from any static host, or open it by double-clicking.

No build step. No dependencies to install. No server-side code.

## Publishing on GitHub Pages

1. Create a repository, for example `augmented-learning`.
2. Upload `index.html`, `.nojekyll` and this README to the default branch.
3. Go to **Settings → Pages → Source: Deploy from a branch → main / root → Save**.
4. Wait about a minute, then open:

   `https://YOUR-USERNAME.github.io/augmented-learning/`

Use a public repository if you want colleagues to reach it without a GitHub account. The tool holds no data, so a public repository exposes no student information.

## Checking it before you roll it out

Run one section end to end and confirm the figures against annexures that have already been signed off.

For BCA II-A, BCA III-A and MCA II-A in the 2026–27 first semester these were 32, 18 and 21 unique students.
