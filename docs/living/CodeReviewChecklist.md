
`````markdown
# Code Review Guideline & Checklist

## 1. Overview & Guiding Principles

This document provides a comprehensive framework for conducting effective, collaborative, and context-rich code reviews. Its purpose is to ensure code quality, share knowledge, and foster a culture of continuous improvement.

> **Guiding Principle:** The primary goal of a code review is to improve the codebase and the team. It is a collaborative process, not an audit. Approach every review with empathy, curiosity, and a focus on constructive feedback.

---

## 2. Part I: For the Author (Engineering the Context)

A high-quality review starts with a high-quality Pull Request (PR). Before requesting a review, the author **must** provide the following context. Use this as your PR description template.

````markdown
### 1. What is the purpose of this change? (The "Why")

**Ticket:** `[Link to Ticket]`

### 2. What is the proposed solution? (The "How")

### 3. How can this be manually tested?

1.  `[Step 1]`
2.  `[Step 2]`
3.  `[Step 3]`

### 4. What is the impact of this change?

### 5. Screenshot / Screen Recording

### 6. Reviewer Checklist

-   [ ] I have personally reviewed my own code.
-   [ ] I have added and updated relevant tests.
-   [ ] I have updated the documentation.
-   [ ] I have confirmed the CI pipeline passes.
`````

-----

## 3\. Part II: For the Reviewer (The Reviewer's Guide)

Use the following sections to guide your review. Instead of just ticking a box, consider the guiding questions to form a holistic view of the change.

### 3.1. Correctness & Functionality

*Does the code do what it's supposed to do, and does it do it correctly?*

  - [ ] Does the code meet all acceptance criteria from the ticket?
  - [ ] Are edge cases and unhappy paths handled gracefully? (e.g., null inputs, empty lists, invalid data)
  - [ ] Is the error handling robust? Does it provide useful context for debugging?
  - [ ] Is there any potential for race conditions or unintended side effects?

### 3.2. Design & Architecture

*Does the code fit cleanly into the existing system? Is it simple, maintainable, and built for the future?*

  - [ ] Is the solution appropriately simple? Is there any unnecessary complexity? (**YAGNI**)
  - [ ] Does this change follow established design patterns and architectural principles? (**SOLID**, **DRY**)
  - [ ] Are the responsibilities of classes, functions, and modules clear and well-defined?
  - [ ] Could this change be made more generic or reusable if applicable?
  - [ ] Does this introduce any problematic coupling with other parts of the system?

### 3.3. Testability & Coverage

*Is the code well-tested and easy to validate?*

  - [ ] Is the new code covered by meaningful tests? (Aim for quality over raw percentage)
  - [ ] Do the tests cover the happy path, edge cases, and failure modes?
  - [ ] Are the tests easy to read and understand? Do they clearly state their intent?
  - [ ] Could any of the tests be written as smaller, more focused unit tests instead of large integration tests?

### 3.4. Security & Compliance

*Is the code secure by design?*

  - [ ] Does this change introduce any new security vulnerabilities? (e.g., SQL injection, XSS, insecure API endpoints)
  - [ ] Is all user input properly validated and sanitized?
  - [ ] Are there any hardcoded secrets or credentials?
  - [ ] Does this change affect data privacy or compliance requirements (e.g., GDPR, HIPAA)?

### 3.5. Performance & Scalability

*Will this code perform well under load?*

  - [ ] Are there any obvious performance bottlenecks? (e.g., N+1 queries, inefficient loops, large memory allocations)
  - [ ] Have the performance implications of database queries or external API calls been considered?
  - [ ] Will this scale effectively as data or traffic grows?

### 3.6. Observability

*Can we understand what this code is doing in production?*

  - [ ] Are there adequate logs to debug issues? Are the logs structured and provide good context?
  - [ ] Have relevant metrics been added to monitor the health and performance of this feature? (e.g., latency, error rates, usage counters)
  - [ ] If this is part of a distributed system, is tracing properly implemented?

### 3.7. Readability & Documentation

*Can another engineer understand and maintain this code a year from now?*

  - [ ] Is the code clear, concise, and easy to understand?
  - [ ] Are variable and function names descriptive and unambiguous?
  - [ ] Are comments present where the code's intent is not immediately obvious?
  - [ ] Has relevant documentation (e.g., `README.md`, Confluence) been updated?

-----

## 4\. Final Quality Gate (Definition of Done)

This checklist confirms the PR is ready to be merged.

  - [ ] At least one other engineer has approved the changes.
  - [ ] All review comments have been addressed or acknowledged.
  - [ ] The CI/CD pipeline is passing successfully.
  - [ ] The changes have been tested and verified in a staging environment (if applicable).
  - [ ] The author's PR checklist is complete.

<!-- end list -->

```
```
