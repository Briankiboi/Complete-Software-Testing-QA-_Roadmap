# 🧪 Complete QA Roadmap

A practical, end-to-end learning path for anyone who wants to become a **Quality Assurance (QA) Engineer** or level up their **software testing** skills.

This repository covers **testing fundamentals, test planning, bug reporting, API testing, automation, CI/CD, performance testing, security testing, QA tools, and practical testing advice**.

---

## 📚 Contents

* [Introduction](#introduction)
* [🐞 How to Report and Document Software Issues / Bugs](#-how-to-report-and-document-software-issues--bugs)

  * [🗂️ 01 — Where to Log Bugs](#️-01--where-to-log-bugs)
  * [📝 02 — Bug Report Structure](#-02--bug-report-structure)
  * [🎯 03 — Severity vs Priority](#-03--severity-vs-priority)
  * [🔄 04 — Bug Reporting Workflow](#-04--bug-reporting-workflow)
  * [🧪 05 — Filled Bug Example](#-05--filled-bug-example)
  * [📊 06 — Bug Documentation Checklist](#-06--bug-documentation-checklist)
  * [💡 QA Principle](#-qa-principle)
* [🌐 HTTP Status Codes — QA Quick Reference](#-http-status-codes--qa-quick-reference)
* [🧪 What QA Should Remember](#-what-qa-should-remember)
* [🏆 QA Golden Rules](#-qa-golden-rules)
* [📄 Test Plan Sample](#test-plan-sample)
* [🧭 QA Learning Roadmap](#qa-learning-roadmap)
* [📜 License](#license)

---

## Introduction

Testing is a critical phase in any product lifecycle whether it's food manufacturing, automotive production, or software development.



For QA engineers, this means:

* Understanding how software components work and integrate.
* Developing the mindset and skills to **"break things" intentionally**.
* Investigating software to uncover unintended behaviors that could lead to failures in production.
* Validating that software behaves correctly under expected and unexpected conditions.
* Communicating defects clearly so they can be reproduced and fixed.

This repository provides a structured path to help you start and grow your **QA and software testing journey**.

---

# 🐞 How to Report and Document Software Issues / Bugs

A structured guide for reporting, documenting, prioritizing, and tracking software defects using the issue-tracking platforms below.



### 🛠️ Supported Issue-Tracking Platforms

1. **📋 Trello** — Create and manage bug cards using boards, lists, labels, and checklists.
2. **🎯 Jira** — Create detailed bug issues, assign severity/priority, track status, and manage the defect lifecycle.
3. **🐙 GitHub Issues** — Report bugs directly within a repository using issues, labels, milestones, and assignments.
4. **🔧 Other Issue-Tracking Platforms** — Apply the same structured approach using your team's preferred tool.


---

## 🗂️ 01 — Where to Log Bugs

| Platform             | Workflow                   | Action             |
| -------------------- | -------------------------- | ------------------ |
| 📋 **Trello**        | Board → Backlog / Bugs     | ➕ New Card         |
| 🎯 **Jira**          | Project → Create           | 🐞 Issue Type: Bug |
| 🐙 **GitHub Issues** | Repository → Issues        | 🐞 New Bug Report  |
| 🔧 **Other Tools**   | Project → Issues / Tickets | 🐞 Create Bug      |

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

| Level         | Action            | Meaning                  |
| ------------- | ----------------- | ------------------------ |
| 🔴 **High**   | Fix immediately   | Current release / sprint |
| 🟡 **Medium** | Fix soon          | Next sprint / near-term  |
| 🟢 **Low**    | Fix when possible | Nice-to-have             |

> **Severity = Impact**
> **Priority = Urgency**

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
   ┌───────────────┐
   │               │
   ▼               ▼
✅ PASS         ❌ FAIL
   ↓               ↓
 CLOSE           REOPEN
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

# 🌐 HTTP Status Codes — QA Quick Reference

| Status                            | Meaning                                     | What QA Should Check                                             |
| --------------------------------- | ------------------------------------------- | ---------------------------------------------------------------- |
| 🟢 **200 OK**                     | Request successful                          | Verify response data and business logic                          |
| 🟢 **201 Created**                | Resource successfully created               | Verify the new resource exists and contains correct data         |
| 🟢 **202 Accepted**               | Request accepted for processing             | Verify background/asynchronous processing                        |
| 🟢 **204 No Content**             | Successful request with no response body    | Verify the operation completed successfully                      |
| 🔵 **301 Moved Permanently**      | Resource permanently moved                  | Verify redirect behavior                                         |
| 🔵 **302 Found**                  | Temporary redirect                          | Verify the user is redirected correctly                          |
| 🟡 **304 Not Modified**           | Resource has not changed                    | Verify caching behavior                                          |
| 🔴 **400 Bad Request**            | Invalid request                             | Test missing, malformed, or invalid parameters                   |
| 🔴 **401 Unauthorized**           | Authentication required/failed              | Test missing, expired, and invalid credentials/tokens            |
| 🔴 **403 Forbidden**              | Access denied                               | Test users accessing resources without permission                |
| 🔴 **404 Not Found**              | Resource does not exist                     | Test invalid URLs, IDs, deleted resources, and missing endpoints |
| 🔴 **405 Method Not Allowed**     | HTTP method is not supported                | Test GET / POST / PUT / PATCH / DELETE restrictions              |
| 🔴 **409 Conflict**               | Request conflicts with current state        | Test duplicate records and conflicting updates                   |
| 🔴 **415 Unsupported Media Type** | Unsupported request format                  | Test incorrect `Content-Type` values                             |
| 🔴 **422 Unprocessable Content**  | Request format is valid but data is invalid | Test validation rules and business constraints                   |
| 🔴 **429 Too Many Requests**      | Rate limit exceeded                         | Test throttling and retry behavior                               |
| ⚫ **500 Internal Server Error**   | Unexpected server failure                   | Verify errors are handled safely and no sensitive data leaks     |
| ⚫ **502 Bad Gateway**             | Invalid response from upstream server       | Test service-to-service failures                                 |
| ⚫ **503 Service Unavailable**     | Server/service temporarily unavailable      | Test downtime, retries, and graceful error handling              |
| ⚫ **504 Gateway Timeout**         | Upstream service timed out                  | Test timeout handling and recovery                               |

---

# 🧪 What QA Should Remember

## 1. **200 OK ≠ Successful Test**

A `200 OK` only tells you the HTTP request succeeded.

Always validate:

* Response body
* Business logic
* Data accuracy
* Permissions
* Error handling
* Database changes
* UI behavior
* Response schema

> ⚠️ An unauthorized API request returning `200 OK` while exposing protected data is still a **security defect**.

---

## 2. **Test More Than the Happy Path**

Don't test only:

```text
Valid Input → 200 OK → Pass
```

Also test:

```text
Missing Input
Invalid Input
Boundary Values
Duplicate Data
Unauthorized User
Expired Token
Invalid Token
Wrong HTTP Method
Non-existent Resource
Large Payload
Empty Response
Server Failure
Network Failure
Rate Limiting
```

---

## 3. **Status Code + Response = Real Validation**

For API testing, validate:

```text
HTTP Status
      +
Response Body
      +
Headers
      +
Schema
      +
Business Rules
```

Example:

```text
Expected:

POST /users
      ↓
201 Created
      ↓
User ID Returned
      ↓
Correct User Data
      ↓
Database Record Created
```

A `201 Created` response alone does **not** prove the feature works correctly.

---

## 4. **Always Test Negative Scenarios**

A strong QA engineer asks:

> **"What happens when something goes wrong?"**

Test:

* ❌ Invalid credentials
* ❌ Missing required fields
* ❌ Invalid data types
* ❌ Expired sessions
* ❌ Unauthorized access
* ❌ Duplicate requests
* ❌ Invalid IDs
* ❌ Deleted resources
* ❌ Server unavailable
* ❌ Slow network
* ❌ Unexpected input

---

## 5. **Security Is Part of Testing**

Always verify that APIs do not expose:

* 🔐 Passwords
* 🔑 Authentication tokens
* 🪪 Personal information
* 💳 Payment information
* 🗄️ Internal database details
* 🖥️ Server paths
* ⚠️ Stack traces

Check:

* Authentication
* Authorization
* Input validation
* Access control
* Session management
* Sensitive data exposure

---

## 6. **Reproduce Before You Report**

A good bug should answer:

```text
What happened?
        ↓
Where did it happen?
        ↓
How can I reproduce it?
        ↓
What should happen?
        ↓
What actually happened?
        ↓
What evidence proves it?
```

---

## 7. **Automation Should Validate, Not Just Execute**

Good automated tests should be:

* ♻️ Reusable
* 🎯 Deterministic
* 📖 Readable
* 🧩 Maintainable
* ⚡ Fast
* 🔍 Focused on behavior

Don't automate a test simply because you can. Automate tests that provide **repeatable and valuable coverage**.

---

# 🏆 QA Golden Rules

| Rule                                  | Principle                                                     |
| ------------------------------------- | ------------------------------------------------------------- |
| 🔍 **Don't trust the UI**             | Validate the API, database, and actual system behavior        |
| 🌐 **Don't trust status codes alone** | Validate status + response + business logic                   |
| 🚫 **Don't test only happy paths**    | Negative testing finds real defects                           |
| 🔐 **Always test authorization**      | Authentication does not equal permission                      |
| 🧪 **Reproduce bugs**                 | A reproducible defect is easier to fix                        |
| 📎 **Capture evidence**               | Screenshots, logs, requests, and responses strengthen reports |
| 🔄 **Retest fixes**                   | A fixed bug must be verified                                  |
| 📈 **Test boundaries**                | Min, max, empty, zero, negative, and unexpected values matter |
| 🗄️ **Verify data integrity**         | Confirm the correct data was created, updated, or deleted     |
| 🤖 **Automate wisely**                | Automate stable, repeatable, high-value scenarios             |

---

# 📄 Test Plan Sample

📥 **Download:** [Test Plan Sample](https://github.com/anas-qa/Quality-Assurance-Road-Map/blob/master/Test_Plan_Sample.pdf)

A test plan typically defines:

* Test scope
* Testing objectives
* Testing approach
* Test environment
* Resources
* Testing schedule
* Risks
* Entry and exit criteria
* Test deliverables

---

# 🧭 QA Learning Roadmap

Below are visual roadmaps outlining the skills, tools, and knowledge areas essential for a modern QA Engineer.

![QA Engineer Road Map 2022](https://i.imgur.com/cM9cM8T.png)

![QA Engineer Road Map 2022](https://i.imgur.com/meodAKp.png)

---
## 🗺️ QA ENGINEERING LEARNING ROADMAP

A structured path covering the core knowledge, testing techniques, tools, and professional skills needed to grow as a modern **QA Engineer**.

---

### 📚 01 · QA FOUNDATIONS

| 🔹 Core Concepts          | 🔹 What to Learn                         |
| ------------------------- | ---------------------------------------- |
| 🔄 **SDLC**               | Software Development Life Cycle          |
| 🧪 **STLC**               | Software Testing Life Cycle              |
| 🎯 **Testing Principles** | Core QA & testing principles             |
| 🧩 **Testing Types**      | Functional & non-functional testing      |
| 🐞 **Bug Lifecycle**      | Identify → Report → Fix → Retest → Close |
| ⚙️ **QA Processes**       | QA workflows, standards & documentation  |

---

### 🧪 02 · MANUAL TESTING

| 🔹 Testing Area            | 🔹 Skills & Techniques               |
| -------------------------- | ------------------------------------ |
| 📝 **Test Cases**          | Writing clear & effective test cases |
| 📋 **Checklists**          | Feature & release checklists         |
| 🎯 **Test Scenarios**      | Positive & negative scenarios        |
| 🔍 **Exploratory Testing** | Discovering unexpected behavior      |
| 🔄 **Regression Testing**  | Validating existing functionality    |
| 💨 **Smoke Testing**       | Build & release verification         |
| 🩺 **Sanity Testing**      | Focused change verification          |
| 👥 **UAT**                 | User Acceptance Testing              |

---

### 🌐 03 · API TESTING

| 🔹 API Area               | 🔹 Skills & Concepts                       |
| ------------------------- | ------------------------------------------ |
| 📡 **HTTP Methods**       | GET · POST · PUT · PATCH · DELETE          |
| 🔢 **HTTP Status Codes**  | 2xx · 3xx · 4xx · 5xx                      |
| 🔗 **REST APIs**          | Endpoints, resources & API architecture    |
| 📦 **Request / Response** | Headers, parameters, payloads & validation |
| 🔐 **Authentication**     | Tokens, credentials & sessions             |
| 🛡️ **Authorization**     | Roles, permissions & access control        |
| 🚀 **Postman**            | Collections, environments & test scripts   |
| 🤖 **API Automation**     | Automated API validation & regression      |

---

### 🤖 04 · TEST AUTOMATION

| 🔹 Automation Area         | 🔹 Skills & Tools                      |
| -------------------------- | -------------------------------------- |
| 🌐 **Selenium**            | Browser automation                     |
| 🎭 **Playwright**          | Modern end-to-end testing              |
| 🌲 **Cypress**             | Web application testing                |
| 🌐 **API Automation**      | Automated API test suites              |
| 🧩 **Test Frameworks**     | Test structure, assertions & reporting |
| 🏗️ **Page Object Model**  | Maintainable automation architecture   |
| 📊 **Data-Driven Testing** | Reusable tests with multiple datasets  |

---

### ⚙️ 05 · CI/CD & DEVOPS

| 🔹 Technology          | 🔹 QA Application              |
| ---------------------- | ------------------------------ |
| 🌿 **Git**             | Version control                |
| 🐙 **GitHub**          | Source control & collaboration |
| ⚡ **GitHub Actions**   | Automated test workflows       |
| 🔧 **Jenkins**         | CI/CD automation               |
| 🐳 **Docker**          | Consistent test environments   |
| 🔄 **CI/CD Pipelines** | Build → Test → Deploy → Verify |

---

### ⚡ 06 · PERFORMANCE TESTING

| 🔹 Performance Area           | 🔹 What to Learn                        |
| ----------------------------- | --------------------------------------- |
| 📈 **Load Testing**           | System behavior under expected load     |
| 💥 **Stress Testing**         | System limits & failure points          |
| 🚀 **Spike Testing**          | Sudden increases in traffic             |
| ⏱️ **Endurance Testing**      | Stability over extended periods         |
| 🛠️ **JMeter**                | Performance test creation & execution   |
| 📊 **Performance Monitoring** | Response time, throughput & bottlenecks |

---

### 🔐 07 · SECURITY TESTING

| 🔹 Security Area               | 🔹 What to Test                                |
| ------------------------------ | ---------------------------------------------- |
| 🔑 **Authentication**          | Login, tokens & credentials                    |
| 🛡️ **Authorization**          | Roles & access permissions                     |
| 🧹 **Input Validation**        | Malicious & unexpected input                   |
| 🛡️ **OWASP Top 10**           | Common web application vulnerabilities         |
| 🔒 **Sensitive Data Exposure** | Passwords, tokens & personal data              |
| 🔄 **Session Testing**         | Session expiry, invalidation & hijacking risks |

---

### 💬 08 · QA PROFESSIONAL SKILLS

| 🔹 Skill                          | 🔹 Why It Matters                               |
| --------------------------------- | ----------------------------------------------- |
| 🗣️ **Communication**             | Clearly communicate defects & findings          |
| 📄 **Technical Documentation**    | Create useful test & defect documentation       |
| 🧠 **Problem Solving**            | Investigate and isolate defects                 |
| 🔎 **Analytical Thinking**        | Identify patterns, risks & edge cases           |
| 🤝 **Team Collaboration**         | Work effectively within Agile teams             |
| 👨‍💻 **Developer Collaboration** | Reproduce, explain & verify defects             |
| 📦 **Product Collaboration**      | Understand requirements & business expectations |

---



---

# 📜 License

This project is open source and available under the **MIT License**.

See the [`LICENSE`](LICENSE) file for details.

---


### 🧪 Keep Testing. Keep Learning. 

> **A good tester doesn't just verify that software works  they discover how it can fail.**
