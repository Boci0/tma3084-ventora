# Proposal pitch: script and slide outline

Due with the proposal report: **Fri 16 Oct 2026**. Recording is **10 minutes at most** (aim for 9:30). Upload to YouTube as **Unlisted**, test the link while logged out, and paste it into the submission.

Fill in everything in [BRACKETS] from your proposal report. The pitch must match the report (rubric B1), so copy names, FR-IDs and dates from it and do not change them.

## What the rubric rewards

| Rubric | Marks | What it needs |
|---|---|---|
| B1 Content | 4 | Problem, solution, AI feature, scope and plan as one story. Same facts as the report. Mockups or wireframes for key features. |
| B2 Delivery | 3 | Every member speaks a fair share and understands the project. Talk, do not read a script. |
| B3 Visuals and time | 3 | Short slides, clear audio and video, working YouTube link, finished within the time limit. |

## Slide plan (11 slides, 9:30)

| # | Slide | Time | Speaker | Show on the slide |
|---|---|---|---|---|
| 1 | Title | 0:20 | Team Leader | App name, team name, client, group number |
| 2 | Our team | 0:40 | Team Leader | Photo and name of each member, their TSPi role, the feature they own |
| 3 | The client | 0:40 | Planning Manager | Client logo or photo, what they do, who will use the app |
| 4 | The problem | 1:10 | Planning Manager | 2 or 3 problems (P1 to P3), each with one piece of evidence (number or quote) |
| 5 | Our solution | 0:50 | Support Manager | One sentence, plus a phone mockup of the home screen |
| 6 | Users and scope | 1:00 | Support Manager | User types, then in scope and out of scope in two short columns |
| 7 | Key features | 1:00 | Quality Manager | 3 to 4 Must-have FR-IDs, each with a screen mockup or wireframe |
| 8 | The AI feature | 1:30 | Development Manager | Input and output example, why it helps, cost, privacy, key protection |
| 9 | How it is built | 0:50 | Development Manager | Architecture diagram (Figure 1 from the report), Flutter, backend, AI service |
| 10 | Plan and risks | 1:10 | Support Manager (plan, 0:40), Quality Manager (risks, 0:30) | Gantt chart, milestones M1 to M4, top 2 risks with mitigations |
| 11 | Close | 0:20 | Team Leader | Summary line, what we will deliver, thank you |

Total: 9:30. If your team has 4 members, give slides 5 and 6 to the Planning Manager and move slide 3 to the Team Leader.

Slide rules: at most 5 short lines per slide, large text, one picture per slide, no paragraphs. Use the Gantt chart from the report (`gantt.png`) on slide 10.

## Script

Say it in your own words. These lines are a base to start from. Read them out loud twice, then speak from the slide.

### Slide 1: Title (Team Leader, 0:20)
"Hello, we are [TEAM NAME] from group [NUMBER]. Our project is [APP NAME], a mobile app for [CLIENT NAME]. We will show you the problem, our solution, the AI feature we will build, and our plan for this semester."

### Slide 2: Our team (Team Leader, 0:40)
"Our team has [5] members. [NAME] is our Planning Manager and owns [FR-IDs]. [NAME] is our Development Manager and owns [FR-IDs]. [NAME] is our Quality Manager and owns [FR-IDs]. [NAME] is our Support Manager and owns [FR-IDs]. I am [NAME], the Team Leader, and I own [FR-IDs]. Everyone writes code and everyone reviews each other's pull requests."

### Slide 3: The client (Planning Manager, 0:40)
"Our client is [CLIENT NAME], [POSITION] at [ORGANISATION]. They [WHAT THE ORGANISATION DOES]. About [NUMBER] people will use the app, mainly [USER TYPES]. We met them on [DATE] and they agreed to work with us until the end of the semester."

### Slide 4: The problem (Planning Manager, 1:10)
"Today, [DESCRIBE HOW THEY WORK NOW]. This causes three problems.
First, [P1]. For example, [NUMBER OR QUOTE FROM CLIENT].
Second, [P2]. The client told us, '[SHORT QUOTE]'.
Third, [P3]. This costs them [TIME OR MONEY OR MISTAKES]."

### Slide 5: Our solution (Support Manager, 0:50)
"So we will build [APP NAME], a Flutter mobile app that [WHAT IT DOES] using AI to [WHAT THE AI DOES]. On the screen you can see the home screen. With this app, [USER] can [MAIN BENEFIT] in [TIME OR STEPS] instead of [OLD WAY]."

### Slide 6: Users and scope (Support Manager, 1:00)
"There are [2 to 4] types of users. [USER TYPE 1] needs to [GOAL]. [USER TYPE 2] needs to [GOAL].
This semester we will deliver [LIST 3 TO 4 IN-SCOPE ITEMS]. We will not deliver [LIST 2 TO 3 OUT-OF-SCOPE ITEMS], because [SHORT REASON]. We agreed this boundary with the client so we can finish on time."

### Slide 7: Key features (Quality Manager, 1:00)
"Here are our main Must-have features. [FR-01] lets a [USER] [DO SOMETHING] so that [BENEFIT], and this is the screen. [FR-02] lets a [USER] [DO SOMETHING]. [FR-03] lets [USER] [DO SOMETHING]. Each feature has its own GitHub issue and its own tests, and we need at least 50 test cases with 60 percent coverage by the end."

### Slide 8: The AI feature (Development Manager, 1:30)
"Our AI feature is [AI CAPABILITY, e.g. image recognition, chatbot, recommendation]. A user [INPUT], and the app shows [OUTPUT]. This solves [P-ID] because [REASON IT IS USEFUL, NOT A GIMMICK].
We use [AI SERVICE]. We thought about three limits. Cost: [HOW YOU STAY WITHIN FREE TIER OR BUDGET]. Privacy: [WHAT DATA IS SENT AND WHAT IS NOT]. Key safety: the AI key is not inside the app. The app calls our own backend, and only the backend holds the key. If the AI is down, the app shows [FALLBACK]."

### Slide 9: How it is built (Development Manager, 0:50)
"The app is built with Flutter. It talks to [BACKEND, e.g. Firebase] for login and data, and to our small backend for the AI requests. We chose [TECH CHOICE] because [REASON]. This diagram is the same as Figure 1 in our report."

### Slide 10: Plan and risks (Support Manager 0:40, then Quality Manager 0:30)
Support Manager: "We use Scrum with two-week sprints and Git Flow on GitHub. Every change goes through an issue, a branch, a pull request with a review, and a passing CI check. Here is our plan. M1 is this proposal on 16 October. M2 is the SRS and a prototype in week 9. M3 is design, the working app and tests in week 13. M4 is the final release, version 1.0.0, before the 2 January deadline."
Quality Manager: "Our two biggest risks are [R1] and [R2]. For the first, we will [MITIGATION]. For the second, we will [MITIGATION]."

### Slide 11: Close (Team Leader, 0:20)
"To sum up, [APP NAME] will help [CLIENT] [MAIN BENEFIT], with an AI feature that [SHORT DESCRIPTION], delivered by [DATE]. Thank you for watching."

## Recording tips

- Record in a quiet room. Do a 20 second test and listen with headphones before the full take.
- Use one screen recording (for example Teams or Zoom with everyone joined, or OBS) so all members' voices are clear. Show each speaker's name on screen the first time they talk.
- Do not read the script word for word. The rubric marks heavy reading as a weak delivery.
- Each member must speak. Check the final video for at least 1 to 2 minutes from everyone.
- Practise once with a timer. If you go over 10:00, cut words from slides 4 and 8, not from the plan.
- After uploading: set to Unlisted, open the link in a private window, check audio, and check the length is under 10 minutes.

## Before you record

- [ ] Every fact, FR-ID, date and name matches the proposal report
- [ ] Mockups or wireframes ready for slides 5 and 7
- [ ] Client has agreed to being named and to any logo or photo
- [ ] AI key or client data is not visible on screen
- [ ] AI use for the slides or script is written in LOGAI
