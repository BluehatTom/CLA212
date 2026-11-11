# Accessibility report - Design Thinking Learning Lab

**Review date:** November 11, 2026

**Files:** Six standalone HTML simulations, revised version 3.

**Design target:** WCAG 2.2 AA. This report documents checks; it is **not a WCAG conformance certification**.

## Automated and functional checks completed

- 12 case-by-lab browser click-throughs: Jordan and Elena across all six apps. Every test completed without a JavaScript page error.
- Interview question followed by visible thinking indicator, immediate-reveal alternative and subsequent response; additional topic choice and reflection route verified.
- The supplementary question-and-follow-up exercise tested in both scenarios for each of the five later apps.
- Test & Iterate: selected method, visible simulated-observation delay, immediate reveal, and results displayed. A starter prototype is provided independently of earlier files.
- 18 responsive structural checks on home and in-lab screens at 1280, 768 and 320 CSS pixels. No horizontal document overflow, duplicate IDs, unlabeled buttons or unlabeled form controls detected on the checked views.
- Accessible `lang=en`, one main landmark and level-one heading per view, skip-to-content link, and live status region verified on tested views.
- Keyboard navigation: skip link receives initial Tab focus, the Interview Simulator question can be activated with Enter, focus outlines visible and response revealed by keyboard.
- Contrast ratios calculated from representative declared palette values: white on red #C41230 = 6.04:1; red on white = 6.04:1; dark red on white = 8.56:1; body text on white = 16.10:1; muted text on white = 7.62:1; green on pale green = 6.93:1. These exceed 4.5:1 for the representative normal-text combinations tested.
- A reduced-motion CSS preference is supported; typing dots become static under reduced motion. The same information is available as text, and the wait may always be skipped.
- Prototype step reordering has explicit Move up and Move down buttons; drag-and-drop is not required.
- Both scenarios and all labs can start independently without JSON import or export.

## Remaining acceptance tests

- Manual NVDA/Chrome or Edge and VoiceOver/Safari end-to-end tests, including every expanded branch and changing keyboard focus after updates.
- Full automated axe-core or equivalent audit with manual criterion-by-criterion review, including dynamic states beyond those sampled.
- 200% and 400% zoom, mobile touch assistive technology, and actual forced-colors system setting.
- Firefox and Safari browser verification and downloads through the deployed GitHub Pages and Canvas iframe contexts.
- Check local storage persistence and resume behavior in Canvas's actual embedded origin; browser partitioning may change it.
- Verify long transcripts, feedback sections and educational comprehension with students using a range of access needs.

## Recommendations for Canvas

Provide a descriptive title on each iframe and a direct-open HTML link. Do not depend on iframe height resizing across origins. Prefer a new-tab option for phone-sized screens and file downloads. Test with a student-role account in the course before deployment.