# Project 1 — OpenCart Demo Manual Testing

**Website:** https://demo.opencart.com  
**Type:** E-Commerce Web Application  
**Test Type:** Manual Black-box Functional Testing  
**Date:** December 2025  
**Tester:** Pragati Kumar Chaudhary

---

## About This Project

OpenCart Demo is a free, publicly available demo of the OpenCart e-commerce platform. I used it as my first manual testing project to practise writing test cases, finding bugs, and documenting the testing process properly.

The focus was on the most common user actions on an e-commerce site — creating an account, logging in, searching for products, and managing the shopping cart.

---

## What Was Tested

| Module | What I Tested | Test Cases |
|--------|--------------|------------|
| User Registration | Valid registration, missing email, duplicate email, password masking, privacy policy | TC_001 – TC_005 |
| User Login | Valid login, wrong password, empty fields, forgot password link, logout | TC_006 – TC_010 |
| Search | Valid search, no results, empty search bar | TC_011 – TC_013 |
| Add to Cart | Add product, cart badge count | TC_014 – TC_015 |
| Shopping Cart | Remove item, update quantity | TC_016 – TC_017 |
| Wishlist | Add when logged in, redirect when guest | TC_018 – TC_019 |
| Contact Us | Submit form with valid inputs | TC_020 |
| **Total** | | **20 test cases** |

---

## Bugs Found

| Bug ID | Where | What the Bug Is | Severity |
|--------|-------|-----------------|----------|
| BUG_001 | Search | No helpful message shown when search bar is submitted empty | Minor |
| BUG_002 | Wishlist | Guest user redirected to login with no explanation | Minor |
| BUG_003 | Shopping Cart | No hint telling user to click Update after changing quantity | Minor |

All three bugs are minor — they don't break the site but they affect user experience.  
Full details (steps to reproduce, expected vs actual) are in `OpenCart_TestCases.xlsx` → Bug Report sheet.

---

## Files in This Folder

### `OpenCart_TestPlan.docx`
The test plan document. Contains:
- Introduction and purpose
- Scope (what was tested) and out of scope (what was not)
- Test environment details — browser, OS, URL
- Test objectives
- Test case summary table
- All 3 bug reports written out in full
- Entry and exit criteria
- Risks and assumptions

### `OpenCart_TestCases.xlsx`
The main working file. Has 3 sheets:
- **Test Cases** — all 20 test cases with ID, module, pre-conditions, steps, expected result, actual result, and status columns
- **Bug Report** — the 3 bugs logged with severity, priority, steps to reproduce, expected vs actual
- **Test Summary** — a summary template to fill in after running the tests

### `OpenCart_RTM.csv`
Requirements Traceability Matrix. Maps each business requirement (REQ_001 to REQ_020) to the test case that covers it. Can be opened in Excel or Google Sheets.

---

## How to Use the Test Cases

1. Open `OpenCart_TestCases.xlsx`
2. Go to the **Test Cases** sheet
3. Open https://demo.opencart.com in Chrome
4. Follow the steps in column F for each test case
5. Write what actually happened in the **Actual Result** column
6. Mark the **Status** as Pass, Fail, or Blocked
7. Take a screenshot for any failed test cases

---

## Key Things I Learned from This Project

- How to write test cases that are clear enough for anyone to follow
- The difference between a test case failing and a bug being logged
- How to describe a bug properly so a developer can reproduce it
- Why the RTM is useful — it shows nothing was missed
