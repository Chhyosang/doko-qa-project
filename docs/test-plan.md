# Test Plan — Doko E-Commerce Platform

## 1. Document Control
| Field | Detail |
|---|---|
| Project Name | Doko – E-Commerce Web Application |
| Document Version | 1.0 |
| Prepared By | Chhyosang Lepcha |
| Role | QA Engineer (Manual Testing) |
| Date | [2025] |

## 2. Introduction
Doko is an e-commerce web application built as a college project, allowing users to browse products, manage a shopping cart, check out and complete payments. This document defines the scope, approach, resources and schedule for manual QA testing of the application.

## 3. Objectives
- Verify that all core e-commerce functionalities work as intended.
- Identify, document, and track defects across major modules.
- Validate the application against functional, UI/UX, and negative/boundary test scenarios.
- Produce a portfolio-ready QA artifact set (test plan, RTM, test cases, bug reports, summary report).

## 4. Scope

### 4.1 In Scope
| Module | Key Features to Test |
|---|---|
| User Registration & Login | Sign up, login, logout, password validation, session handling |
| Product Browsing & Search | Product listing, category filter, search, sorting, product detail page |
| Shopping Cart | Add/update/remove items, quantity change, cart persistence, price calculation |
| Checkout | Address entry, shipping method selection, order summary, guest checkout |
| Payment Processing | Payment method selection, payment form validation, success/failure handling |
| Order Management | Order confirmation, order history, order status |
| Admin Panel (if applicable) | Product management, order management (basic checks) |

### 4.2 Out of Scope
- Automated testing / test scripting
- Performance, load, and stress testing
- Penetration/security testing (only basic negative-input checks are included)
- Third-party payment gateway's internal systems (only integration behavior from Doko's side is tested)
- Native mobile app testing (if Doko is web-only)

## 5. Test Approach / Strategy
Manual black-box testing will be performed using the following techniques:
- **Functional Testing** – Verify each feature works per requirements.
- **UI/UX Testing** – Check layout, responsiveness, alignment, and usability.
- **Negative Testing** – Invalid inputs, empty fields, wrong formats.
- **Boundary Value Testing** – Min/max limits (e.g., quantity, price, character length).
- **Smoke Testing** – Quick check of critical flows before a full test cycle.
- **Regression Testing** – Re-run relevant test cases after bug fixes.
- **Exploratory Testing** – Unscripted testing to catch issues test cases might miss.

## 6. Test Environment
| Item | Detail |
|---|---|
| Application URL | [Local/staging URL of Doko] |
| Browsers | Chrome, Firefox, Edge (latest versions) |
| Devices | Desktop (Windows), Mobile view via browser responsive mode |
| Test Data | Dummy user accounts, sample products, test card numbers (sandbox) |
| Tools | Browser DevTools, Excel/Google Sheets, GitHub Issues |

## 7. Roles & Responsibilities
| Role | Responsibility |
|---|---|
| QA Tester (You) | Test planning, test case design, execution, bug logging, reporting |
| Developer(s) | Fix reported bugs, support root-cause discussion |

## 8. Entry Criteria
- Doko application is deployed and accessible in the test environment.
- Requirements/user stories for the modules under test are available.
- Test cases have been written and reviewed.

## 9. Exit Criteria
- All planned test cases have been executed at least once.
- No open **Critical** or **High** severity bugs remain unresolved (or are documented as known issues).
- Test summary report has been prepared and shared.

## 10. Test Deliverables
1. Test Plan (this document)
2. Requirement Traceability Matrix (RTM)
3. Test Case Document
4. Bug Reports (GitHub Issues / bug log sheet)
5. Test Summary Report
6. Execution evidence (screenshots)

## 11. Risk & Mitigation
| Risk | Mitigation |
|---|---|
| Limited time as a solo tester | Prioritize test cases by module criticality (P0/P1 first) |
| Test environment instability (college project hosting) | Re-test flaky failures before logging as bugs |
| No dedicated staging/test payment gateway | Use sandbox/test card numbers where available; clearly log as assumption otherwise |
| Requirements not formally documented | Derive requirements from user stories / app walkthrough and note assumptions in RTM |

## 12. Schedule (Sample)
| Phase | Duration |
|---|---|
| Test Planning & RTM | 2 days |
| Test Case Design | 3 days |
| Test Execution – Cycle 1 | 3 days |
| Bug Logging & Retesting | 2 days |
| Regression Cycle | 2 days |
| Test Summary Report | 1 day |

## 13. Approval
| Name | Role | Signature/Date |
|---|---|---|
| [Chhyosang Lepcha] | QA Engineer | |

