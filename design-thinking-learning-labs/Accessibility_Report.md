# Accessibility QA — Design Thinking Learning Lab

**Review date:** November 11, 2026  
**Target:** WCAG 2.2 Level AA; **not a conformance certification**.

## Checks reported as completed
- Automated end-to-end browser navigation for both the Jordan/campus-events and Elena/customer-pickup scenarios in all six standalone lab files.
- Interview JSON to Problem Framing import and progress-file transfer between later labs.
- Initial-screen checks for English language metadata, main landmark, H1, skip link, duplicate element IDs, and visible-control labels at 1280, 768 and 320 CSS-pixel widths.
- No document-level horizontal scrolling at 320 CSS pixels.
- Keyboard-usable buttons (including prototype reordering) and visible focus indication; Enter activates scenario and question choices.
- Reduced-motion and forced-colors CSS; no time limits or autoplay media.
- Representative contrast measurements: white/red 6.04:1; dark red/white 8.56:1; normal body text/white 16.10:1; muted text 7.62:1; slate 7.86:1; green/pale green 6.93:1.

## Not yet verified
- Manual NVDA, JAWS or VoiceOver screen-reader acceptance tests.
- Full axe-core and criterion-by-criterion WCAG audit.
- Browser zoom at 200% and 400%; mobile assistive technology and OS forced-colors testing.
- Safari and Firefox compatibility.
- Actual Canvas embedding restrictions, content-security policies, file input/download behavior and student persistence.

## Deployment recommendations
Give students a direct HTML link as well as any embedded iframe. Test keyboard and screen-reader flows in the deployed location, including file import, export and submission, with a student-role account. Fix identified issues before claiming WCAG conformance.
