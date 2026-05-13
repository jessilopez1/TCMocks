## HR Mock Interview — Live Conductor

**Link [here](https://jessilopez1.github.io/TCMocks/hr_mock_conductor.html)** 

A browser-based tool for conducting HR Mock Interview sessions. No installation required — open the file in any browser.

### What it does

Covers the full session flow in a single interface:

- **Setup** — candidate name, programme, target role, company, and special case profile (career changer, upskiller, career gap, junior, non-native speaker, freelancer, repeat session)
- **Interview** — phase-by-phase conductor with timing, question bank, follow-up probes, and per-phase notes. Questions can be marked as used during the session.
- **Rubric** — 8-competency evaluation rubric with 1–4 scoring. Can be filled in during or after the session.
- **Checklist** — observer checklist with tick boxes, grouped by session phase.
- **Debrief** — verbal debrief scripts pre-drafted and adapted based on rubric scores. Placeholders indicate where to personalise.
- **Feedback** — structured written feedback form with auto-generated output ready to copy or send.
- **Export** — sends the session record to a shared Google Sheet, with a separate tab per coach.

### How to use it

1. Open `hr_mock_conductor.html` in a browser (Chrome or Safari recommended)
2. Fill in Setup before the session starts — including your name as coach/consultant/STL
3. Navigate between tabs during the session as needed
4. Export to Google Sheets at the end (see setup instructions below)

### Google Sheets setup (one-time, per coach)

This only needs to be done once. The same Google Sheet is shared across coaches — each coach's sessions go into a separate tab automatically.

1. Open the shared Google Sheet (link below — ask your team lead if you don't have it)
2. Go to **Extensions → Apps Script**
3. Delete the default code and paste the script from the **Export tab** inside the tool (click the code block to copy)
4. Click **Deploy → New deployment → Web app**
   - Execute as: **Me**
   - Who has access: **Anyone**
   - Click Deploy
5. Copy the deployment URL
6. Paste it into the **Export tab** of the tool — it saves in your browser for future sessions

> **Note:** Your consultant name (entered in Setup) determines which tab your records go to. Use the same name every session for consistent records.

### Who can access the Google Sheet

The sheet owner (team lead) has access to all tabs. Individual consultants only need access if it is shared with them directly. Records are not visible to learners at any point.

