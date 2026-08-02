# Test Summary Report — Doko E-Commerce Platform

## 1. Overview
This report summarizes the manual QA testing effort carried out on the Doko e-commerce application, covering registration/login, product browsing, shopping cart, checkout, payment processing, order management, and admin panel modules.

> **Note:** The numbers below are a sample/template based on the 45 designed test cases. Replace them with your real execution results once you run the test cases against your Doko build.

## 2. Test Execution Summary
| Metric | Count |
|---|---|
| Total Test Cases Designed | 45 |
| Test Cases Executed | 45 |
| Passed | 38 |
| Failed | 5 |
| Blocked | 2 |
| Pass Rate | 84% |

## 3. Module-wise Breakdown
| Module | Test Cases | Passed | Failed | Blocked |
|---|---|---|---|---|
| User Registration & Login | 9 | 9 | 0 | 0 |
| Product Browsing & Search | 5 | 5 | 0 | 0 |
| Shopping Cart | 9 | 7 | 1 | 1 |
| Checkout | 7 | 5 | 1 | 1 |
| Payment Processing | 7 | 4 | 3 | 0 |
| Order Management | 3 | 3 | 0 | 0 |
| Admin Panel | 3 | 3 | 0 | 0 |
| UI / Usability | 2 | 2 | 0 | 0 |

## 4. Defect Summary
| Severity | Count |
|---|---|
| Critical | 1 |
| Major | 2 |
| Minor | 2 |
| Cosmetic | 0 |
| **Total** | **5** |

**Top defects found:**
1. **BUG_002 (Critical)** — Payment form accepts an expired card date without validation.
2. **BUG_001 (Major)** — Cart total doesn't update after removing an item until page refresh.
3. **BUG_003 (Major)** — Guest checkout redirects to login instead of allowing a guest flow.

Full details are in [`bug-reports/bug-log.xlsx`](../bug-reports/bug-log.xlsx).

## 5. Key Observations
- Core flows (registration, login, browsing, order confirmation) are stable.
- Payment and checkout modules had the highest concentration of defects — these are the highest-risk areas and should be prioritized for retesting after fixes.
- No critical crashes were found; issues found were functional/validation gaps rather than application-breaking failures.

## 6. Recommendations
- Fix the Critical and Major bugs before considering the module release-ready.
- Add stronger client-side and server-side validation on the payment form (expiry date, CVV).
- Re-run the full Shopping Cart and Checkout regression suite after fixes are applied.
- Consider adding automated regression tests for the cart total calculation logic going forward, since it's a high-risk area prone to silent miscalculation.

## 7. Sign-off
| Field | Detail |
|---|---|
| Tested By | [Your Name] |
| Test Cycle | Cycle 1 |
| Date | [Insert Date] |
| Status | Ready for retest after critical/major bug fixes |
