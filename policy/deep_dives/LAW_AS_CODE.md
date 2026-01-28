# TECHNICAL SPEC: Law as Code (Lex Cryptographia)
## The Operating System for the Algorithmic Republic
### The Human Standard (Version 0.9.1)

---

## Executive Summary

Natural language law (English, French, etc.) is buggy. It is ambiguous ("reasonable doubt"), recursive, and requires expensive human interpreters (lawyers) who are prone to error and corruption.

If AI is to administer the state (as proposed in `AI_GOVERNANCE.md`), the law must be machine-readable, logically consistent, and executable. We propose **Lex Cryptographia**: a formalized legal syntax where the Code *is* the Law.

---

## Part I: The Architecture

### 1.1 The Language (Catala++)
We adopt and extend **Catala**, a domain-specific language (DSL) designed for legislative logic.
*   **Feature:** Formal logic verification.
*   **Capacity:** Can mathematically prove that a set of laws is complete (covers all cases) and consistent (no contradictions).

### 1.2 The Compiler (The "Legislative Linter")
Before a bill is voted on, it must pass the Compiler.
*   **Input:** Proposed Statute (e.g., "Tax rate is 5% for income < $50k").
*   **Check:** Does this conflict with existing statutes? Does it violate the Constitutional Constraints (Five Laws)?
*   **Output:**
    *   *Pass:* Bill is valid.
    *   *Fail:* "Error: Line 40 conflicts with Civil Rights Act Section 2."
*   **Effect:** Legislators cannot pass logically broken laws.

### 1.3 The Execution Layer (The API)
Once passed, the law is not just published; it is **deployed**.
*   **The Law API:** `GET /law/tax/calculate?income=50000` -> `Returns: 2500`
*   **Universal Access:** Any citizen, company, or AI agent can query the API to know *exactly* what the law requires in their situation. No ambiguity. No "expensive lawyer needed to interpret."

---

## Part II: The Human Interface

We are not replacing human judgment; we are narrowing it to where it matters.

### 2.1 The "Natural Language" Wrapper
Citizens do not read code.
*   The system auto-generates a "Plain English" version of the statute from the code.
*   **The Rule:** The *Code* is the binding truth. The *English* is the explanatory comment. (Reversing the current reality where the text is binding but ambiguous).

### 2.2 The "Discretionary Gap"
Not all law is logic. "Self-Defense" depends on context.
*   **The Hybrid Model:**
    *   **Deterministic Law:** Taxes, Benefits, Speed Limits, Contract execution. -> **Fully Automated.**
    *   **Discretionary Law:** Criminal intent, Family custody, Free speech nuance. -> **Human Tribunal.**
    *   The Code explicitly defines *where* it hands off control to a human judge.

---

## Part III: The Github of Governance

### 3.1 Version Control for the State
*   **Repo:** `united-states/federal-code`
*   **Branching:** Parties propose "Pull Requests" (Bills).
*   **Merging:** A passed vote = A Merge to `main`.
*   **Blame:** `git blame` shows exactly which legislator added the loophole in line 452.

### 3.2 Regression Testing
*   **Simulation:** Before merging a tax cut, we run a simulation on the "Digital Twin" of the economy.
*   **Result:** "Warning: This change increases deficit by 4%."
*   **Accountability:** Politicians can no longer lie about the math. The Compiler checks the math.

## Conclusion

**Lex Cryptographia** turns the state into a transparent, deterministic software platform. It eliminates the "Interpretive Corruption" where laws mean one thing for the rich and another for the poor. In the Algorithmic Republic, the law executes exactly as written, for everyone.
