## HR Mock Interview — Live Conductor

**Link [here](https://jessilopez1.github.io/TCMocks/hr_mock_conductor.html)** 

A browser-based tool for conducting HR Mock Interview sessions. No installation required — open the link in any browser. Works on any device with internet access.

---

### What it does

Covers the full session flow in a single interface:

- **Setup** — coach name, candidate name, programme, target role, company, job posting notes, and special case profile (career changer, upskiller, career gap, junior, non-native speaker, freelancer, repeat session)
- **Interview** — phase-by-phase conductor with timing, question bank, follow-up probes, and per-phase notes. Questions can be marked as used during the session.
- **Rubric** — 8-competency evaluation rubric with 1–4 scoring. Can be filled in during or after the session.
- **Checklist** — observer checklist with tick boxes, grouped by session phase.
- **Debrief** — verbal debrief scripts pre-drafted and adapted based on rubric scores.
- **Feedback** — structured written feedback form with auto-generated output ready to copy or send.
- **Export** — sends the session record to a shared Google Sheet, with a separate tab per coach.

---

### How to use it

1. Open the link above in any browser
2. Fill in **Setup** before the session starts — your coach name is the most important field, it determines which tab your records go to in Google Sheets
3. Navigate between tabs during the session as needed
4. At the end of the session, go to **Export** → click **Send to Google Sheets**
5. Check the Google Sheet to confirm the record arrived

> **If you try to close the browser without exporting**, you will get a warning asking you to confirm. This is intentional — it is a reminder to export before closing.

> **If your internet drops or your browser crashes mid-session**, when you reopen the conductor a banner will appear at the top offering to restore your unsaved session. The conductor saves a local backup every 30 seconds automatically.

---

### Google Sheets — how records are stored

All sessions from all coaches go to a single shared Google Sheet. Each coach's records are stored in a separate tab named after them. The tab is created automatically the first time a coach exports a session.

- The Google Sheets connection is pre-configured — no setup needed for coaches
- Your coach name (entered in Setup) determines which tab your records go to
- Use the same name every session for consistent records
- The sheet owner has access to all tabs. Coaches only see their own tab unless the sheet is shared with them directly.

---

### For the sheet owner — Apps Script setup (already done, for reference)

The Google Sheets integration uses a Google Apps Script deployment. If this ever needs to be reconfigured:

1. Open the Google Sheet → Extensions → Apps Script
2. Paste the script from the **Export tab** inside the conductor (click the code block to copy)
3. Deploy → New deployment → Web app → Execute as: **Me** → Who has access: **Anyone** → Deploy
4. The deployment URL is already hardcoded in the conductor — if it changes, update the `value` of the `sheetsUrl` input in the HTML file

---

### Updating the conductor

To update the tool:
1. Download the new version of `hr_mock_conductor.html`
2. Upload it to this repository, replacing the existing file
3. GitHub Pages updates automatically within 1–2 minutes
4. The URL stays the same — no need to share a new link

---

## Questions or issues

Raise them with the Career Services team lead.
