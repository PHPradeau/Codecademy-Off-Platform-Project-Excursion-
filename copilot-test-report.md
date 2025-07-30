# Simulated Testing Report for Excursion Landing Page

Date: 30 July 2025

## 1. Screen Reader Simulation

Tool: NVDA (Windows) or VoiceOver (macOS)

Steps & Expected Output:

1. Page load:
   - Announces "Excursion" (document title).
   - Reads meta description silently (for SEO, not voiced).

2. Header region (aria-label not needed, using `<header>`):
   - "Heading level 1, Discover hidden places in the world around you." 
   - "Link, Download Excursion (Coming soon!)."

3. Hero video region (role and aria-label):
   - "Region: Hero video section."
   - Announcement of video: "Video, source content."

4. Intro section:
   - "Region: Introduction text."
   - "Heading level 2, Your personal travel guide."
   - "Excursion remembers places you like, and recommends new points of interest around you." 

5. Landscape image section:
   - "Region: Landscape image section." 
   - Reads alt text: "Landscape camping."

6. Phone icon section:
   - "Region: Phone icon section."
   - Alt text: "Phone icon."

7. Coming Soon section:
   - "Region: Coming soon section." 
   - "Heading level 2, Coming Soon for iPhone and Android." 
   - "Link, Download Excursion (Coming soon!)."

8. Footer (role contentinfo):
   - "Footer region." 
   - "© Excursion."

**Result:** Screen reader announces content in logical order, regions are identifiable, links are focusable and announced correctly.

---

## 2. Keyboard Navigation

1. Focus starts on page body.
2. Tab key moves focus to the first link: 
   - Outline appears (aquamarine border). 
   - Link text announced by screen reader.
3. Subsequent Tab moves through:
   - "Download Excursion (Coming soon!)" in header.
   - "Download Excursion (Coming soon!)" in Coming Soon section.
4. Footer has no interactive elements; Tab moves past document.

**Result:** Keyboard focus outlines are visible, navigation order is correct.

---

## 3. Responsive Layout Check

Viewports tested:

- Mobile (360x640px)
  - Video max-width 360px fits container.
  - Text and images scale to screen width.

- Tablet (768x1024px)
  - Media query applied: larger headings (60px / 48px) look balanced.
  - Padding and margins remain consistent.

- Desktop (1440x900px)
  - Layout remains centered with appropriate whitespace.

**Result:** Page scales gracefully at different breakpoints.

---

## 4. Accessibility Notes

- All images have meaningful `alt` text.
- Video has default browser fallback text.
- Focus styles meet contrast requirements.

No critical accessibility issues detected in this simulation.

*End of Report*
