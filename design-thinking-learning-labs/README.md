# Design Thinking Learning Lab — CLA 212

Six **standalone** interactive HTML learning simulations. Each file embeds its own CSS, JavaScript, fictional scenario evidence, and tagged PDF exporter. The labs share the same red/white color and Georgia/Arial typography without institutional logo or institutional branding.

## Open the labs

1. [Interview Simulator](01_Interview_Simulator.html) — Empathy: practice asking open, behavioral interview questions and follow-ups.
2. [Problem Framing](02_Problem_Framing.html) — Define: separate evidence from assumptions, challenge an explanation, and reframe the problem.
3. [Idea Generation](03_Idea_Generation.html) — Ideate: explore reverse thinking, analogy, and SCAMPER; build an idea bank.
4. [Idea Selection](04_Idea_Selection.html) — Evaluate: score alternatives, consider tradeoffs, and select what to prototype.
5. [Rapid Prototyping](05_Rapid_Prototyping.html) — Prototype: three-step guide to build and preview a service journey.
6. [Test & Iterate](06_Test_and_Iterate.html) — Test: plan a test, interpret a simulated observation, revise the prototype directly, and retest.

## Cases and sequence

Every lab includes the same two independently selectable fictional cases:

- **Jordan / Campus events:** A commuter student evaluates whether staying for a campus event is worthwhile, with concerns about schedule gaps, what happens on arrival, and navigating unfamiliar activities.
- **Elena / Riverbend customer pickup:** A first-time customer navigates online-order pickup, including where to go, acknowledgment, and order handoff.

Students can use one case or both. Each lab supplies its own **baseline findings**. No JSON upload, download, or progression between files is required. Work on either case is saved separately in local browser storage when permitted by the browser.

## Guidance and question flow

A **Review concepts and vocabulary** disclosure appears on every start screen and inside each case. Instructions include relevant examples, definitions, and learning steps.

The Interview Simulator retains rich branching and a visible 2–3 second pause before fictional respondents answer. Interview coaching is separated from the conversation transcript. Other labs include an **optional**, collapsed stakeholder follow-up section, rather than requiring every student to conduct a new interview at each design stage.

**Idea bank rule:** Each idea must contain **15–600 characters**. A bank holds at most 15 ideas; students are encouraged to contribute at least three ideas spanning two different techniques.

## Learning artifacts

Choose **Download accessible PDF** to create a tagged, text-based PDF directly in the browser. It includes heading/paragraph tags, document language, selectable text, and structured reading order. Every lab includes an HTML alternative; the Interview Simulator also offers TXT field notes. The PDF exporter is designed for English/Western Latin text. For other scripts or when assistive technology compatibility is uncertain, use the semantic HTML alternative.

**Important:** Tagged output is not automatically a PDF/UA or WCAG conformance certification. An assistive technology acceptance test is recommended before formal deployment. See [Accessibility Report](Accessibility_Report.md).

## Canvas deployment

The files are self-contained; no external scripts, API keys, servers, or student logins are required. The intended base GitHub Pages URL is:

`https://bluehattom.github.io/CLA212/design-thinking-learning-labs/`

Paste each file's direct HTTPS URL into a Canvas module or an approved iframe. For iframe embedding, use `width="100%"` and a descriptive `title`; always include an independent direct-open link for mobile and assistive technology users. Verify downloads and PDF usability in Canvas Student View.

Each page includes the footer disclosure: **Developed with the help of AI (including ChatGPT). All cases and simulated responses are fictional.**