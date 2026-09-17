# Accessibility & Architecture Audit Report

## Website Audited

**Website:** DigiLocker  
**URL:** https://www.digilocker.gov.in/

**Audit Date:** 16 September 2026  
**Tool Used:** Google Lighthouse  
**Keyboard Test:** Manual keyboard-only navigation using Tab and Shift + Tab

## 1. Lighthouse Audit Results

| Category | Score |
|---|---:|
| Performance | 47 |
| Accessibility | 77 |
| Best Practices | 96 |
| SEO | 83 |

**Lighthouse capture:** 15 September 2026, 6:43 PM PDT

## 2. Accessibility Issues Identified

### WEB-001 – Buttons
**WCAG Reference:** 4.1.2 Name, Role, Value

**Evidence:** Lighthouse reports: "Buttons do not have an accessible name."

**Severity:** High

**User Impact:** Screen-reader users may not understand the purpose of some buttons.

**Recommended Fix:** Add a clear accessible name using visible text or an appropriate aria-label.

### WEB-002 – Images
**WCAG Reference:** 1.1.1 Non-text Content

**Evidence:** Lighthouse reports: "Image elements do not have [alt] attributes."

**Severity:** Medium

**User Impact:** Screen-reader users may miss important information conveyed by images.

**Recommended Fix:** Add meaningful alt text to informative images; use empty alt for decorative images.

### WEB-003 – Forms
**WCAG Reference:** 1.3.1 Info and Relationships

**Evidence:** Lighthouse reports: "Form elements do not have associated labels."

**Severity:** High

**User Impact:** Users of assistive technology may not know what information to enter in form fields.

**Recommended Fix:** Associate each form control with a clear label.

### WEB-004 – Keyboard Navigation
**WCAG Reference:** 2.4.3 Focus Order

**Evidence:** Lighthouse reports: "Some elements have a [tabindex] value greater than 0."

**Severity:** Medium

**User Impact:** Keyboard users may experience an unexpected focus order while navigating.

**Recommended Fix:** Remove positive tabindex values and use the natural DOM order for keyboard focus.

### WEB-005 – Headings
**WCAG Reference:** 1.3.1 Info and Relationships

**Evidence:** Lighthouse reports: "Heading elements are not in a sequentially-descending order."

**Severity:** Medium

**User Impact:** Screen-reader users may find the page structure harder to understand.

**Recommended Fix:** Organize headings in a logical hierarchy without skipping heading levels unnecessarily.

## 3. Keyboard Navigation Test

### Test Method

The DigiLocker homepage was navigated using only the keyboard with **Tab** and **Shift + Tab**, without using the mouse.

### Observation

The page provided visible keyboard focus through navigation items, accessibility controls, language selection, Login/Register, and document categories.

### Result

Keyboard navigation was available, but the focus order should be reviewed to ensure a logical and predictable sequence.

## 4. Conclusion

The audit identified several accessibility issues related to buttons, images, form labels, keyboard focus order, and heading structure. Addressing these issues would improve the usability of the website for users who rely on assistive technologies and keyboard navigation.
