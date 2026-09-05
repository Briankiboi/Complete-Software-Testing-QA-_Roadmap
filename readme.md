# Complete QA Roadmap

A practical, end-to-end learning path for anyone who wants to become a **Quality Assurance (QA) Engineer** or level up their **software testing** skills. This repo covers fundamentals, test planning, roadmaps, tools, and hard-won advice from real-world testing experience.


---

## 📚 Contents

- [Introduction](#introduction)
- [How to Report and Document Software Issue )
- [Test Plan Sample](#test-plan-sample)
- [QA Learning Roadmap](#qa-learning-roadmap)
- [License](#license)

---

## Introduction

Testing is a critical phase in any product lifecycle—whether it's food manufacturing, automotive production, or software development. The goal is always the same: **ensure the final output matches expectations and satisfies the need it was created for.**

For QA engineers, this means:

- Understanding how software components work and integrate.
- Developing the mindset and skills to "break things" intentionally.
- Investigating software to uncover unintended behaviors that could lead to failures in production.

This repository provides a structured path to help you start and grow your **QA and software testing journey**.





---

# 🐞 How to Report and Document Software Issue / Bug using **Trello, Jira, GitHub Issues**, or any issue-tracking platform.

A structured guide for reporting, documenting, prioritizing, and tracking software defects 

---

## 🗂️ 01 — Where to Log Bugs

| Platform             | Workflow                 | Action             |
| -------------------- | ------------------------ | ------------------ |
| 📋 **Trello**        | Board → Backlog / Bugs   | ➕ New Card         |
| 🎯 **Jira**          | Project → Create         | 🐞 Issue Type: Bug |
| 🐙 **GitHub Issues** | Repository → Issues      | 🐞 New Bug Report  |
| 🔧 **Other Tools**   | Project → Issues/Tickets | 🐞 Create Bug      |

> 🏷️ **Always label defects as:** `bug`

---

## 📝 02 — Bug Report Structure

Use the following template when creating a bug ticket:

```md
# 🐞 Bug Report

## Summary
<!-- One-line description of the defect -->

## Steps to Reproduce
1.
2.
3.

## Expected Result
<!-- What should happen -->

## Actual Result
<!-- What actually happens -->

## Environment
- Environment: Dev / Staging / Production
- URL: https://your-app-url.com/path
- Browser / OS / Device:
- User Role:
- Build / Version:

## Evidence
- Screenshots:
- Screen Recordings:
- Logs / Console Errors:

## Severity / Priority
- Severity: Low / Medium / High / Critical
- Priority: Low / Medium / High

## Additional Notes
<!-- Related tickets, workarounds, or other information -->
```

---

## 🎯 03 — Severity vs Priority

### 💥 Severity — How Much Does It Impact the System?

| Level           | Impact                                        | Example                     |
| --------------- | --------------------------------------------- | --------------------------- |
| 🔴 **Critical** | System unavailable, data loss, security issue | Application completely down |
| 🟠 **High**     | Major functionality broken                    | Payment process fails       |
| 🟡 **Medium**   | Feature partially broken                      | Workaround available        |
| 🟢 **Low**      | Minor/cosmetic issue                          | Incorrect text or alignment |

### ⚡ Priority — How Quickly Should It Be Fixed?

| Level         | Action            | Meaning                 |
| ------------- | ----------------- | ----------------------- |
| 🔴 **High**   | Fix immediately   | Current release/sprint  |
| 🟡 **Medium** | Fix soon          | Next sprint / near-term |
| 🟢 **Low**    | Fix when possible | Nice-to-have            |

---

## 🔄 04 — Bug Reporting Workflow

```text
🔍 FIND DEFECT
      ↓
📝 DOCUMENT ISSUE
      ↓
🏷️ SET SEVERITY
      ↓
⚡ SET PRIORITY
      ↓
📎 ATTACH EVIDENCE
      ↓
👨‍💻 ASSIGN TO DEVELOPER
      ↓
🛠️ FIX IMPLEMENTED
      ↓
🧪 QA VERIFICATION
      ↓
✅ PASS → CLOSE
      ↓
❌ FAIL → REOPEN
```

---

## 🧪 05 — Filled Bug Example

### 🐞 `[BUG] Form accepts invalid input without showing error`

| Field            | Details                              |
| ---------------- | ------------------------------------ |
| **Summary**      | Required field validation is missing |
| **Environment**  | Staging                              |
| **Browser / OS** | Chrome / Windows                     |
| **User Role**    | Standard User                        |
| **Version**      | Latest                               |
| **Severity**     | 🟡 Medium                            |
| **Priority**     | 🟡 Medium                            |

### 🔁 Steps to Reproduce

1. Log in with a valid account.
2. Navigate to the relevant form.
3. Leave a required field empty or enter invalid data.
4. Click **Submit**.

### ✅ Expected Result

The form should display a validation error and prevent submission.

### ❌ Actual Result

The form submits successfully without displaying a validation error.

### 📎 Evidence

* 📸 Screenshot: Attach screenshot
* 🎥 Screen recording: Attach recording
* 🖥️ Console: No errors displayed

### 📌 Additional Notes

The issue affects all users and appears to be related to recent form changes.

---

## 📊 06 — Bug Documentation Checklist

| #  | Requirement              | Status |
| -- | ------------------------ | ------ |
| 01 | 📝 Clear bug summary     | ☐      |
| 02 | 🔁 Reproduction steps    | ☐      |
| 03 | ✅ Expected result        | ☐      |
| 04 | ❌ Actual result          | ☐      |
| 05 | 💻 Environment details   | ☐      |
| 06 | 📎 Evidence attached     | ☐      |
| 07 | 💥 Severity assigned     | ☐      |
| 08 | ⚡ Priority assigned      | ☐      |
| 09 | 👨‍💻 Developer assigned | ☐      |
| 10 | 🧪 Retested after fix    | ☐      |

---

## 💡 QA Principle

**Clear steps + reproducible results + strong evidence = faster fixes.**

A good bug report should allow a developer or QA engineer to understand and reproduce the defect **without needing additional clarification**.

---

📄 **Download:** [test_plan_sample.pdf](https://github.com/anas-qa/Quality-Assurance-Road-Map/blob/master/Test_Plan_Sample.pdf)


---


## Key Advice for Testers


- **Automation = documented manual tests, engineered for reuse.** Write clear, readable, and maintainable test scripts.
- **Ensure your tests actually validate behavior.** Avoid "happy path only" tests that don't challenge the system.
- **Your test code shouldn't need testing.** Keep it simple, deterministic, and easy to understand.
- **200 OK ≠ success.** Don't rely solely on HTTP status codes. An unauthorized API call returning 200 is a security risk.



---



## License

This project is open source and available under the [MIT License](LICENSE) (add your own LICENSE file if needed).

---

## QA Learning Roadmap

Below are visual roadmaps outlining the skills, tools, and knowledge areas essential for a modern QA Engineer in 2022 and beyond.

![QA Engineer Road Map 2022](https://i.imgur.com/cM9cM8T.png)  
![QA Engineer Road Map 2022](https://i.imgur.com/meodAKp.png)

These roadmaps cover:

- **Foundations:** SDLC, STLC, testing types, bug lifecycle.
- **Manual Testing:** Test cases, checklists, exploratory testing.
- **Automation:** Selenium, Playwright, Cypress, API testing tools.
- **CI/CD & DevOps:** Jenkins, GitHub Actions, Docker basics.
- **Performance & Security:** JMeter, OWASP, basic security testing.
- **Soft Skills:** Communication, documentation, collaboration with devs and product.

> 🧭 Use these as a guide, not a checklist. Focus on understanding concepts before jumping into tools.

---
