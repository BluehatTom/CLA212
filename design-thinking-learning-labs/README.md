# Design Thinking Learning Lab — CLA 212

Six standalone, responsive HTML simulations. Each includes its own styling, teaching cases, practice interactions, and a built-in PDF exporter. The visual system uses red, white and neutral colors with Georgia/Arial typography and no institutional logo.

## Launch an individual lab

1. [Interview Simulator](01_Interview_Simulator.html) — Empathize: practice experience-based interviewing and follow-up routes.
2. [Problem Framing](02_Problem_Framing.html) — Define: sort evidence, challenge assumptions and revise the framing.
3. [Idea Generation](03_Idea_Generation.html) — Ideate: use creative methods and respond to constraints.
4. [Idea Selection](04_Idea_Selection.html) — Evaluate: score alternatives and explain tradeoffs.
5. [Rapid Prototyping](05_Rapid_Prototyping.html) — Prototype: construct and preview a service journey.
6. [Test & Iterate](06_Test_and_Iterate.html) — Test: run simulated feedback rounds, revise and compare outcomes.

Each file stands alone. Both fictional cases are available in every lab: **Jordan (campus events)** and **Elena (Riverbend customer pickup)**. Students can explore one or both, and each new lab begins with its own baseline evidence. Work is saved separately per case when browser storage permits.

## Student identity and downloadable artifacts

At the beginning of any lab, students enter their **First name** and **Last name**. These fields also appear when they work in a case. The student's name is printed inside the PDF and prepopulates its suggested filename — for example, `Bob Smith Lab 1.pdf`. The filename field can be edited, and the `.pdf` suffix is added automatically. The same first/last name is reused across these pages if browser storage is available.

**Download PDF of all work** appears near the beginning of the active case, including during a live interview, with a second download control at the bottom of most labs. The PDF is the only submitted learning-artifact format offered by the interface. The Interview Simulator exports the complete question-and-answer path, evidence, field notes, coach guidance (as a separate section), and reflection. Labs 2–6 export the baseline evidence, student inputs and decisions, stakeholder dialogue, scored criteria or prototype/testing rounds, review checkpoints, and the available decision history for that case. Downloads can be made before or after revising an idea. No completion-marking action is used.

The PDF exporter runs entirely in the browser, generates tagged PDFs with selectable English/Western-Latin text and heading/paragraph structure, and does not transmit student responses to a server. Tagged output alone is not a PDF/UA accessibility certification. See [Accessibility Report](Accessibility_Report.md).

## Instructional design

- Interview coaching is in a collapsed **Learning coach** area below the conversation. It does not float over or interrupt the simulated dialogue.
- The interview offers richer question branches and a 2–3-second pause with an immediate-reveal control.
- Each lab includes a **Review concepts and vocabulary** disclosure.
- Prototyping and Test & Iterate use explicit step navigation.
- Each idea bank entry must contain 15–600 characters; a case's bank can hold up to 15 ideas.
- Every footer identifies the fictional cases as **Developed with the help of AI (including ChatGPT)**.

## Canvas deployment

Published path: `https://bluehattom.github.io/CLA212/design-thinking-learning-labs/`

Link directly to a standalone file from each Canvas module or embed it in a titled, full-width iframe. Provide a direct-open link in addition to the embed. Test the new student-name fields, filename editing and **PDF download** in the institution's Canvas Student View, as iframe and third-party storage behavior depends on institutional settings.