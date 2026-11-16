# Design Thinking Learning Lab — Accessibility QA Report

**Revision:** 4 · **Date:** November 16, 2026 · **Target:** WCAG 2.2 AA (not an audit certification)

## Scope

All six standalone HTML learning labs, including the Jordan/campus-events and Elena/customer-pickup scenarios, updated concept/vocabulary guidance, Prototyping/Test navigation, optional stakeholder dialogues, and downloaded artifacts.

## Verified in this revision

| Area | Result | Test performed |
|---|---|---|
| Responsive reflow | **Pass in tested views** | Chromium at 320, 768, and 1280 CSS pixels; two cases in all six labs; no document-level horizontal overflow |
| Duplicate HTML IDs | **Pass in tested views** | Inspected rendered home and case screens at three viewport widths |
| Interactive flows | **Pass in tested views** | Start, scenario selection, question/reveal, Prototyping steps 1→2→3, walkthrough, Test and Iterate initial round→observation→inline revision→second round |
| Optional stakeholder dialogue | **Pass in tested views** | Open, ask and reveal, and verify the optional panel stays open afterward |
| Interview coach separation | **Pass in tested views** | Coaching is outside the simulated conversation DOM and visibly labeled as coaching |
| Idea-bank rules | **Present and verified** | Minimum 15 characters, maximum 600, up to 15 entries; on-screen instructions and input validation |
| Concept and vocabulary panels | **Present and verified** | Expanded on home screens and included in active-case views; native accessible `details`/`summary` |
| Focus/keyboard controls | **Functional in tested paths** | Native buttons, form fields, tabindex-reachable page headings, button-operated prototype reordering, no drag-only requirement |
| PDF download and extraction | **Pass in tested outputs** | All six apps downloaded text PDFs; PDFs parsed by pypdf with selectable/extractable text; PDFs reported as tagged by `pdfinfo` |
| PDF document structure | **Pass structural checks** | `/StructTreeRoot`, `/ParentTree`, marked content, heading and paragraph roles, `/Lang (en-US)`, `/MarkInfo /Marked true` |
| Multi-page PDF | **Pass** | Generated a seven-page, 110-paragraph test PDF; all paragraphs extracted, no page losses |
| Script execution | **Pass in tested paths** | No uncaught browser JavaScript errors during six-app click-through tests |

## Accessibility design choices

- Native headings, labels, buttons, input controls, disclosure widgets, and visible focus outlines
- Animated response pauses include a direct **Show response now** control; typing is not necessary for these controls
- No game-critical dragging; prototype step order adjusted with buttons
- The coach feedback is separated from the interview transcript, reducing speaker attribution confusion
- Each file is self-contained; separate cases do not depend on browser-to-browser file transfers
- Tagged PDF learning artifact includes headings, paragraphs, metadata and a logical text order; semantic HTML export is offered as an alternative

## Known limits and required manual validation

**No claim of full WCAG 2.2 AA, PDF/UA, or institutional accessibility certification is made.** These steps remain to be tested with assistive technologies and in the final course environment:

1. Complete real NVDA/JAWS + Chrome/Edge and VoiceOver + Safari screen-reader acceptance tests of all major workflows, including wait states and download announcements.
2. Test browser zoom at 200% and 400%, Windows forced-colors mode, keyboard-only use from start to completion, and mobile assistive technology.
3. Test PDF tags, hierarchy and reading order using institutional PDF accessibility tools and assistive technologies; verify text alternatives where relevant. The exporter supports English/Western Latin characters and may simplify other scripts. Offer semantic HTML instead when characters do not preserve correctly.
4. Test Canvas iframe restrictions and direct-open links on the institution’s actual Canvas installation; verify PDF download/open/submission permissions in Student View.
5. Review all instructional prose and case responses with students for cognitive accessibility; avoid treating fictional outcomes as empirical validation.

## Conclusion

The revision resolves the observed usability problems in the tested flows and introduces tagged, selectable-text PDF export with HTML fallback. **It is ready for instructor pilot testing, but not yet for an accessibility-conformance claim.**