# Δ Delta Report: [Brief Issue Title]

**Ticket:** `[Link to Jira/Linear Ticket]`
**Status:** Open / **In-Progress** / Resolved / Closed
**Lead Diagnostician:** The Diagnostician

---

### 1. Issue Definition
[Clear, one-sentence description of the reported problem.]

### 2. Replication Steps
[A precise, step-by-step guide to reliably reproduce the issue 100% of the time.]
1.  ...
2.  ...

### 3. State Snapshot (BEFORE)
**This section captures the broken state as verifiable proof.**
-   **Observed Behavior:** [Description of what happens when following the replication steps.]
-   **Relevant Logs/Errors:**
    ```
    (Paste the exact error messages or relevant log lines here.)
    ```
-   **Failing Test Output:**
    ```
    (Paste the output of the specific test that fails *before* the fix.)
    ```

### 4. Root Cause Analysis (RCA)
[A brief but precise explanation of the technical root cause of the issue, based on the evidence above.]

### 5. Proposed Solution
[The specific, planned code change to address the RCA.]

---
### 6. Implementation Proof
-   **Code Diff:**
    ```diff
    (Paste the code diff of the changes made here.)
    ```

### 7. State Snapshot (AFTER)
**This section captures the fixed state as verifiable proof.**
-   **Observed Behavior:** [Description of the new, correct behavior when following the replication steps.]
-   **Successful Test Output:**
    ```
    (Paste the output of the now-passing test that was failing before.)
    ```

### 8. Regression Verification
**This section proves the fix did not break other parts of the system.**
-   **Action:** Executed the full test suite (`npm test` or equivalent).
-   **Result:**
    ```
    (Paste the summary output of the full test suite run here.)
    ```
-   **Action:** Manually smoke-tested the following adjacent features: [e.g., User Profile Page, Logout Functionality].
-   **Result:** All adjacent features confirmed to be working as expected.

---
**Conclusion:** The root cause was addressed, and the fix is verified to be effective and non-regressive. The issue is considered resolved.
