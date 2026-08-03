# Doko E-Commerce — Manual QA Testing Project

Manual QA testing project performed on **Doko**, a college-built full-stack e-commerce web application covering shopping cart, checkout, and payment processing (plus registration/login, product browsing, order management, and admin panel).

This repository documents the complete manual testing lifecycle: test planning, requirement traceability, test case design, execution, defect logging, and reporting — built as a portfolio piece to demonstrate real-world manual QA skills.

##  Project Summary
- **Application under test:** Doko (E-Commerce web app)
- **Testing type:** Manual (Functional, UI/UX, Negative, Boundary, Regression)
- **Modules covered:** Registration & Login, Product Browsing/Search, Shopping Cart, Checkout, Payment Processing, Order Management, Admin Panel
- **Test cases designed:** 45
- **Bugs found:** 5 (1 Critical, 2 Major, 2 Minor)
- **Pass rate:** 84% (Cycle 1)

##  Tools Used
| Purpose | Tool |
|---|---|
| Test documentation | Excel / Google Sheets |
| Bug tracking | Excel log (adaptable to GitHub Issues / Jira) |
| Test execution evidence | Screenshots |
| Version control | Git & GitHub |

##  Repository Structure
```
doko-qa-project/
├── README.md
├── docs/
│   ├── test-plan.md
│   └── requirement-traceability-matrix.xlsx
├── test-cases/
│   └── test-cases.xlsx
├── bug-reports/
│   └── bug-log.xlsx
├── test-summary-report/
│   └── summary-report.md
└── screenshots/
    └── (execution & bug evidence)
```

##  Deliverables
- **[Test Plan](docs/test-plan.md)** — scope, approach, environment, entry/exit criteria
- **[Requirement Traceability Matrix](docs/requirement-traceability-matrix.xlsx)** — maps requirements to test cases
- **[Test Cases](test-cases/test-cases.xlsx)** — 45 manual test cases (positive, negative, boundary, UI)
- **[Bug Log](bug-reports/bug-log.xlsx)** — logged defects with severity, priority, and repro steps
- **[Test Summary Report](test-summary-report/summary-report.md)** — execution metrics, defect summary, recommendations

##  Testing Approach
- **Functional Testing** — validated core flows: add to cart, checkout, payment, order confirmation
- **Negative Testing** — invalid inputs, empty required fields, expired/invalid card details
- **Boundary Testing** — stock limits, minimum/maximum quantities, invalid pricing
- **UI/Usability Testing** — responsiveness and error message clarity across cart/checkout/payment
- **Regression Testing** — re-verification of related test cases after bug fixes

##  Key Defects Found
| ID | Title | Severity |
|---|---|---|
| BUG_002 | Payment form accepts expired card date without validation | Critical |
| BUG_001 | Cart total doesn't update after removing an item until refresh | Major |
| BUG_003 | Guest checkout redirects to login instead of allowing guest flow | Major |

Full details in [`bug-reports/bug-log.xlsx`](bug-reports/bug-log.xlsx).

##  Result Snapshot
- 45 test cases executed across 8 modules
- 38 Passed / 5 Failed / 2 Blocked
- Highest defect concentration in **Payment Processing** and **Checkout** modules

##  About Me
Doko was originally built as a college e-commerce project. This repository documents the manual QA testing I performed on it — test planning, test case design, execution and defect reporting — created to demonstrate real-world QA skills for my resume and portfolio.

**Chhyosang Lepcha**
https://www.linkedin.com/in/chhyosang-lepcha-088182215/ | chhyosanglepcha@gmail.com 
