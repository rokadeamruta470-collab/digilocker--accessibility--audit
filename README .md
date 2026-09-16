# DigiLocker Accessibility & Architecture Audit

## Project Overview

This project contains an accessibility audit and a monorepo-style project structure for the DigiLocker website.

## Audited Website

DigiLocker  
https://www.digilocker.gov.in/

## Audit Tools

- Google Lighthouse
- Keyboard-only navigation using Tab and Shift + Tab

## Lighthouse Results

| Category | Score |
|---|---:|
| Performance | 47 |
| Accessibility | 77 |
| Best Practices | 96 |
| SEO | 83 |

## Project Structure

```text
digilocker-audit/
├── client/
│   └── README.md
├── server/
│   └── README.md
├── docs/
│   └── audit-report.md
└── tests/
    └── README.md
    