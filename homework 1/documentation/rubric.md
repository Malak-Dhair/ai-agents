# CSE 491 — AI Agents: Homework 1 Rubric

This assignment is graded on a 100 point scale. All grading is based on your demo video.
## Functional Requirements

| # | Requirement | Points | How to demonstrate |
|---|-------------|--------|--------------------|
<<<<<<< HEAD
| 1 | App starts with `python app.py` and loads in the browser at `localhost:8080` | 50 | Show the terminal command, the startup output, and the browser loading the homepage |
| 2 | Resume page shows your own data (not the placeholder data) | 25 | Navigate to `/resume` — your institutions, positions, and experiences must appear |
| 3 | AI chat responds to a question using your resume content | 25 | Ask the chat a question and show the AI replying with information from your resume |
=======
| 1 | **Database Read Expert** — ask a question like "How long did they work at [institution]?" | 20 | Show the console printing the generated SQL query, and the chat replying with an accurate answer |
| 2 | **Database Write Expert** — ask to add a skill, e.g. "Add [skill] to [experience]" | 20 | Show the console printing the generated Python code, the skill appearing on the resume page right after the AI responds, and it still being there after you manually reload the page |
| 3 | **Orchestrator Coordination** — ask a compound request, e.g. "Does he know [skill]? If not, add it to [experience]." | 20 | Show the console printing the Orchestrator's plan, that the plan includes both a Database Read Expert call and a Database Write Expert call in the right order, and that both actually execute in that order |
| 4 | **Database Schema** — the `llm_roles` table | 20 | Show, via a query or a database browser, that `llm_roles` exists and contains all four expert configurations (Database Read Expert, Database Write Expert, Content Expert, Orchestrator) |
| 5 | **Concept Question** — Explain 3 different prompt engineering concepts that you tried and their effectiveness | 20 | Add a file called `prompt_engineering.md` |
>>>>>>> ee206e61f9d9ae18caf14d02e27996fc19bc5fe6

## Grading Policy

- Each requirement uses **all-or-nothing** grading. You receive the full points or zero — no partial credit.
- Points are awarded based on **functionality demonstrated in the video**, not code quality or implementation choices.
- Even if your app works perfectly, you receive **zero points** for any requirement not clearly shown in your video.

## Demo Video Structure

- State your full name at the start
<<<<<<< HEAD
- Say: *"I will now demonstrate the functional requirements for CSE 491 Homework 0"*
- Announce each requirement before demonstrating it
- Aim for under 3 minutes; clear audio and video required

## Submission Checklist

- [ ] CSV files updated with your own resume data
- [ ] `home.html` updated with your name, bio, and photo
- [ ] App runs from `python app.py` (no Docker required)
=======
- Say: *"I will now demonstrate the functional requirements for CSE 491 Homework 1"*
- Announce each requirement before demonstrating it
- Keep the console/terminal visible on screen for requirements 1–3 — the graded output includes what gets printed there
- Clear audio and video required

## Submission Checklist

- [ ] `llm.py` has the master template, `fill_template`, and all four expert-routing functions
- [ ] `database.py` has `getLLMRoles()` and `insertRows()`
- [ ] `llm_roles` table created and seeded with all four expert configs
- [ ] Chat now routes through the Orchestrator by default
- [ ] Resume panel refreshes automatically after a database write
>>>>>>> ee206e61f9d9ae18caf14d02e27996fc19bc5fe6
- [ ] Code pushed to your fork: `git push origin main`
- [ ] Fork URL included in your submission (e.g. `https://github.com/YOUR-USERNAME/ai-agents`) so the grader can access your code
- [ ] Demo video recorded and uploaded via the [homework submission form](https://docs.google.com/forms/d/e/1FAIpQLSdBfMvBMgC-xT34M_gv9plffbaf4Kh4LtWTvOsLT9I4RobNZg/viewform)
