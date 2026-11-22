# IT Portfolio — Milestone 2

Live site: https://mmckinney-cpu.github.io/my-portfolio/

## Accessibility improvements

- Added a visible-on-focus **Skip to main content** link to Home, About, and Projects so keyboard users can bypass repeated navigation; Contact already had this link.
- Added `id="main-content"` to each page's main landmark so the skip links have a working destination.
- Added explicit labels for the name, email, and message inputs so assistive technology announces their purpose.
- Grouped contact reasons in a `fieldset` with a `legend` so radio buttons are announced as one related choice.
- Added accessible validation with `aria-invalid`, inline error descriptions, and focus on the first invalid field so users can locate and correct errors.
- Added a live status message that explains the contact form opens an email draft rather than sending a message automatically.
- Added visible keyboard focus styling and responsive form controls.

## Gestalt principles

- **Proximity:** Related project details are grouped inside individual cards, and related form labels, controls, and errors appear together.
- **Similarity:** Repeated project and skills cards use the same shape, borders, spacing, and typography to communicate their shared purpose.

## Consistent visual design

All pages use the shared `css/style.css` file with deep teal (`#234E52`), warm gold (`#E6B566`), ivory (`#F7F5F0`), and charcoal (`#263238`). Reusable spacing and card styles create a consistent visual hierarchy.

## Contact form behavior

The form validates required fields and email format, then opens a draft in the visitor's default email application. It does **not** send messages to a server. Visitors must send the draft themselves. A direct email link is also available.

## Testing checklist — pending independent verification

- [ ] Run WAVE on Home, Projects, About, and Contact after GitHub Pages deploys; record and fix any remaining errors.
- [ ] Check every foreground/background combination with WebAIM Contrast Checker for WCAG AA.
- [ ] Test keyboard-only navigation, visible focus, form error announcements, and mobile layout.
- [ ] Verify email-draft behavior on a device with a configured email application.

**Note:** These code changes were reviewed and committed, but a completed WAVE scan and contrast audit have not yet been independently verified. Do not claim zero WAVE errors until those checks pass.
