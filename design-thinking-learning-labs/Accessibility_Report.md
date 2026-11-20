# CLA 212 Design Thinking Learning Labs — Accessibility and Functional QA

**Revision:** 6 · **Date:** November 20, 2026 · **Target:** WCAG 2.2 AA. This report is a functional and technical check, not a formal conformance certification.

## Verified in this revision

| Check | Status and evidence |
|---|---|
| Browser execution | All six standalone HTML files executed in headless Chromium with no uncaught JavaScript exceptions in the 12 tested scenario paths. |
| Responsive layout | At the tested 1280 px desktop and 320 px mobile widths, both scenarios in every lab had no document-level horizontal overflow. |
| Identity and filenames | First name and last name controls were present for all six labs. Entering `Bob` and `Smith` prepopulated `Bob Smith Lab N`, and custom names such as `Bob Smith Lab 2 - campus.pdf` were honored on export. |
| PDF placement | Each active lab has exactly one PDF download button. The button and editable filename appear in a section at the bottom of the lab, following the practice work. All 12 case tests generated PDFs with the expected name and case information. |
| PDF text | PDF output was checked with `pdftotext`; headings, the student's name, case details and generated activity content were extractable. |
| PDF tags | Generated files carry a structure tree, document-language metadata, and tagged headings/paragraphs; PDF structure is not equivalent to PDF/UA certification. |
| Interview coaching | An **Open Interview Coach** button appears directly below the conversation transcript and before the next-question choices. It toggles an inline, separate panel. Open/close behavior, `aria-expanded`, panel visibility, and keyboard focus were tested. |
| Manual completion/HTML export | No **Mark this lab complete** or **Download HTML alternative** controls appear in any of the six tested active-case views. |
| Decisions and evidence | The later lab PDFs contain baseline evidence, stage-specific inputs, review results and recorded decision history. Interview PDF contains question/answer routes, evidence, student notes and separate coaching. |
| Accessibility-minded controls | Standard form labels, accessible focus, native buttons, direct response reveal, non-drag prototype step controls, and language metadata remain in the apps. |

## Open checks before formal Canvas deployment

1. Test complete keyboard-only and NVDA/JAWS/VoiceOver paths including the bottom-of-page filename edit, Interview Coach toggle, student identity saving, and PDF download announcement.
2. Check tagged-PDF reading order, structure, all long multi-page artifacts and non-Western-script input in a specialist PDF accessibility checker. The in-browser exporter primarily supports English/Western Latin text.
3. Validate PDFs within the institution's Canvas iframe, in Canvas Student View, and through a direct-open link. Browser storage and downloads may differ in third-party iframe environments.
4. Evaluate high zoom (200%/400%), reduced-motion, forced-colors and mobile screen readers across all case/activity stages.
5. Check that students understand the fictional nature of personas and that simulated test outcomes are not treated as empirical evidence.

**Conclusion:** The revised workflow and PDF controls passed the documented functional test cases. Do not claim full WCAG 2.2 AA or PDF/UA conformance without further manual verification.