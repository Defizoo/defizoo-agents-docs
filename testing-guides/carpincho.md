# Testing Guide: Carpincho (Coding Orchestrator)

**Channel:** #carpincho-techno
**What he does:** Development task management, code reviews, orchestrating coding sessions

> **Note:** Carpincho is the most technical agent. He orchestrates AI coding sessions (OpenCode) and multi-model code reviews. You'll get the most out of him if you have some familiarity with the development workflow, but you can still test many of his capabilities without deep technical knowledge.

---

## Level 1: Task Planning (Start Here)

These test Carpincho's ability to understand and plan development work.

1. "What repos are we currently working on?"
2. "Plan a task to add a new API endpoint for fetching user staking positions"
3. "What's the current status of any in-progress development tasks?"
4. "Break down 'add USDVE price oracle integration' into subtasks"
5. "What would be needed to build a Vaultedge dashboard showing TVL, mints, and liquidations?"

---

## Level 2: Code Review Requests

These test Carpincho's multi-model code review orchestration.

6. "Run a code review on the latest PR in [repo name]"
7. "Do a security-focused review of the liquidation bot code"
8. "Review the smart contract changes in the last commit -- focus on potential vulnerabilities"
9. "What's the current code review process? How many models are involved?"
10. "Prioritize the findings from the last code review -- which ones need immediate attention?"

---

## Level 3: Development Workflow

These test Carpincho's understanding of the full development lifecycle.

11. "Walk me through the task lifecycle from planning to completion"
12. "A task just finished the planning phase. What's the next step?"
13. "The QA tester found 3 issues in the latest implementation. How do we handle feedback injection?"
14. "What models do you use for code reviews and what does each one focus on?"
15. "How do you handle a situation where a coding task has been stuck for hours?"

---

## Level 4: Technical Coordination

These push Carpincho into cross-functional coordination.

16. "We need to add a new subgraph for Vaultedge. Plan the full implementation -- contracts, indexing logic, deployment, and testing."
17. "The frontend team needs a new API. Coordinate the backend task: plan it, scope it, and set up the review process."
18. "Create a technical spec for implementing sUSDVE (staked USDVE)"
19. "Plan the testing strategy for the Vaultedge launch: what needs to be tested, in what order, by whom?"
20. "We have a potential security vulnerability reported. Walk me through the response process."

---

## Things to Watch For

- **Task awareness:** Does he know what's currently in progress?
- **Technical depth:** Does he understand the codebase and architecture?
- **Review quality:** Are code review findings meaningful and prioritized?
- **Process adherence:** Does he follow the defined task lifecycle?
- **Safety:** Does he refuse to do destructive operations without confirmation?
