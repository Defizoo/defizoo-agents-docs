# Testing Guide: Carpincho (Coding Orchestrator)

**Channel:** #carpincho-techno
**What he does:** Development task management, code reviews, orchestrating coding sessions

> **Note:** Carpincho is the most technical agent. He orchestrates AI coding sessions (OpenCode) and multi-model code reviews. You'll get the most out of him if you have some familiarity with the development workflow, but you can still test many of his capabilities without deep technical knowledge.

---

## Scope and Complexity

These tests evaluate Carpincho's ability to assess and communicate the scope of technical work.

1. "Estimate the complexity of adding flash loan support to Vaultedge. Break it down by contracts, testing, and integration."
2. "What are the potential ripple effects of changing the interest rate model in USDVE?"
3. "How long would it take to add Chainlink oracles to Vaultedge? Give me a rough timeline."
4. "Assess the complexity of migrating Vaultedge from Solidity 0.8 to 0.8.20. What needs to change?"
5. "What technical debt exists in the current Vaultedge codebase that we should address before launch?"
6. "Compare the scope of implementing a lending protocol vs a perpetual futures exchange. Which is more complex and why?"
7. "What would be involved in adding zk-rollup support to the protocol? Estimate timeline and team size needed."
8. "How complex would it be to add multi-chain support to Vaultedge? What chains should we prioritize?"
9. "Assess the effort required to implement EIP-4626 tokenized vault standard in Vaultedge."
10. "What's the scope of adding MEV protection to the protocol? What components need changes?"

---

## Requirements Gathering

These test Carpincho's ability to extract, clarify, and document requirements.

11. "A partner wants to integrate Vaultedge. What questions should we ask them before scoping the integration?"
12. "I'm not sure what I want yet -- just 'something better than our current APR.' Help me think through requirements."
13. "Document the requirements for a notification system that alerts users when their position is near liquidation."
14. "What information do you need from me to plan a new subgraph implementation?"
15. "Our frontend team says they need a 'simpler API.' Turn that into concrete requirements."
16. "Create a requirements doc for a multi-sig governance module for Vaultedge."
17. "A DAO member wants 'better UX.' Help me translate that into actionable requirements."
18. "What are the requirements for adding a gasless transaction feature? Think through edge cases."
19. "Document the full requirements for implementing a referral program in the protocol."
20. "The compliance team needs certain data retention capabilities. What questions do we need to ask them?"

---

## Focused Reviews

These test specific types of targeted code reviews.

21. "Run a gas optimization review on the Vaultedge liquidation logic."
22. "Do a reentrancy audit on all external calls in the USDVE contracts."
23. "Review the access control patterns across Vaultedge -- are there any privilege escalation risks?"
24. "Check the oracle integration code for front-running vulnerabilities."
25. "Review the test coverage for the stability fee calculation. Are edge cases covered?"
26. "Audit the emergency shutdown functionality -- does it handle all edge cases?"
27. "Review the arithmetic in the collateral ratio calculations. Look for overflow/underflow risks."
28. "Check the upgradeability proxy pattern implementation for storage collision risks."
29. "Review the signature verification logic for potential bypass vulnerabilities."
30. "Audit the bridge integration code for message forging vulnerabilities."

---

## Review Management

These test how Carpincho manages and coordinates review processes.

31. "Set up a review schedule for the next two weeks covering Vaultedge, Lynex, and Catex."
32. "How do you triage code review findings? Walk me through your prioritization process."
33. "The last review found 15 issues. Help me categorize them by severity and create an action plan."
34. "We have two PRs that depend on each other. How do you coordinate reviews for interdependent changes?"
35. "Create a code review report template we can use for all protocol reviews."
36. "Track the status of all open review findings from the last 3 reviews. Which are still unresolved?"
37. "Set up automated review reminders for pending PRs that haven't been reviewed in 48 hours."
38. "Create a SLA framework for different severity levels of code review findings."
39. "How would you manage a review where we have conflicting findings from two different review models?"
40. "Design a review rotation system to ensure all repos get equal attention."

---

## Model Coordination

These test how Carpincho orchestrates multiple AI models for comprehensive reviews.

41. "How many review models do you use? What are their specialties?"
42. "Coordinate a review where one model focuses on security, another on gas optimization, and another on code quality."
43. "When models disagree on a finding, how do you resolve the conflict?"
44. "Run a review using only security-focused models on the liquidation bot."
45. "Compare findings from two different review models on the same PR. What did each miss?"
46. "Create a model rotation schedule so different models review different parts of the codebase."
47. "What prompts do you use for each review model? Can you share the templates?"
48. "Design a scoring system to evaluate model performance on different review types."
49. "How do you prevent model fatigue from repeating the same findings across reviews?"
50. "Create a model specialization matrix showing which models excel at which review types."

---

## Troubleshooting

These test Carpincho's debugging and problem-solving capabilities.

51. "The tests are failing on main but not locally. How do you troubleshoot this?"
52. "A user reported their transaction keeps reverting. Walk me through the debugging process."
53. "Gas costs spiked 30% after the last deployment. What could cause this and how do we diagnose it?"
54. "The subgraph is out of sync. How do we identify and resolve the issue?"
55. "Describe your debugging workflow for intermittent test failures."
56. "Production is showing inconsistent state between nodes. What diagnostic steps do you take?"
57. "An integration test is timing out intermittently. How do you narrow down the root cause?"
58. "The protocol is consuming more gas than expected after a recent upgrade. How do you identify the culprit?"
59. "Flashbots shows our transactions are being frontrun. What's the debugging process?"
60. "A health check endpoint is returning 500 errors intermittently. Walk me through the investigation."

---

## System Design

These test Carpincho's architecture and system design skills.

61. "Design the architecture for a real-time dashboard showing Vaultedge protocol metrics."
62. "Propose a modular upgrade path for Vaultedge that minimizes governance overhead."
63. "Design an event-driven architecture for cross-contract communication in the protocol."
64. "What's the best way to structure tests for a protocol with multiple interacting contracts?"
65. "Design a rate limiting system for the Vaultedge API to prevent abuse."
66. "Architect a composable liquidation system that can handle multiple collateral types."
67. "Design a circuit breaker system that can pause protocol operations based on external conditions."
68. "Propose a modular interest rate model architecture that allows easy adjustment."
69. "Design a data availability solution for off-chain liquidations."
70. "Architect a cross-chain message passing system with fraud proof capabilities."

---

## Testing Strategy

These test Carpincho's understanding of comprehensive testing approaches.

71. "What's the difference between unit tests, integration tests, and fuzz tests? When should we use each?"
72. "Create a test coverage matrix for Vaultedge showing what each test type covers."
73. "How do you test edge cases that are hard to reproduce in unit tests?"
74. "Plan a testing strategy for a cross-chain implementation of Vaultedge."
75. "What's your approach to property-based testing for financial contracts?"
76. "Design a testing framework for validating upgrade safety."
77. "Create a formal verification roadmap for critical Vaultedge contracts."
78. "How would you test a governance upgrade before it goes live?"
79. "Design a chaos testing strategy for the protocol's Depeg scenarios."
80. "Plan a testing approach for flash loan attack simulation."

---

## Security Response

These test Carpincho's handling of security incidents and vulnerabilities.

81. "A whitehat reported a potential vulnerability via Immunefi. Walk me through the response process."
82. "How do you handle responsible disclosure when a vulnerability affects live user funds?"
83. "Create a security incident classification framework for the team."
84. "What are the immediate steps when a protocol exploit is detected in progress?"
85. "Plan a post-mortem process for security incidents that ensures we learn and improve."
86. "Design a bug bounty program structure for Vaultedge with severity-based payouts."
87. "Create a emergency response playbook for different attack scenarios."
88. "How do you coordinate with auditors during an active incident?"
89. "Plan a security drills schedule to practice incident response."
90. "Design a timelock configuration strategy for emergency pauses."

---

## Multi-Agent Collaboration

These test how Carpincho coordinates with other agents.

91. "Coordinate with Miro to create architecture diagrams for the Vaultedge codebase."
92. "Work with HATZO to document user-facing error messages and their technical causes."
93. "Plan a feature with Carl -- he handles partnerships, you handle technical implementation. How do you collaborate?"
94. "Coordinate a review cycle where Carpincho plans, Miro designs the review dashboard, and HATZO writes the findings report."
95. "Create a handoff document from Carpincho to the frontend team explaining the new API."
96. "Plan a release process involving all agents: Mila for announcements, HATZO for docs, Miro for dashboards."
97. "Coordinate with a new AI agent onboarding to the ecosystem. What's your handoff process?"
98. "How do you collaborate with external auditors during a formal audit engagement?"
99. "Design a cross-agent review process where findings flow through multiple verification stages."
100. "Create a shared workspace system for multi-agent collaboration on complex features."

---

## Tone and Approach Tests

These test how Carpincho adapts his communication style.

101. "Explain the Vaultedge liquidation mechanism to a non-technical stakeholder."
102. "Describe the same mechanism to a security researcher. What details would you emphasize?"
103. "Write a technical decision document explaining why we chose Chainlink over another oracle provider."
104. "When explaining a complex bug to the team, what's your preferred format?"
105. "How do you communicate technical tradeoffs to decision-makers who need to make budget/timeline calls?"
106. "Draft an incident report for the community explaining a recent protocol pause."
107. "Explain MEV to a non-technical DAO member. Keep it clear but accurate."
108. "Write a technical RFC for a proposed architecture change. Cover alternatives considered."
109. "How do you explain technical debt to stakeholders who want to ship features faster?"
110. "Create a developer onboarding document explaining the protocol's architecture. Use clear examples."

---

## Tool and Capability Tests

These test specific tools and integrations Carpincho uses.

111. "Use git to show me the commit history for the last month across all protocol repos."
112. "Create a project board showing current tasks, their status, and who owns them."
113. "Set up a PR review workflow that requires approval from at least two models before merge."
114. "Generate a codebase health report showing test coverage, complexity metrics, and technical debt."
115. "Configure automated alerts for when critical contracts haven't been reviewed in 90 days."
116. "Create a deployment checklist system with automated verification steps."
117. "Set up a CI/CD pipeline that runs security scans on every PR."
118. "Generate a changelog document summarizing all changes since the last release."
119. "Create a dependency vulnerability report for all npm/solc dependencies."
120. "Set up monitoring dashboards for protocol health metrics."

---

## Level 1: Task Planning (Start Here)

These test Carpincho's ability to understand and plan development work. Start with these for basic sanity checks.

121. "What repos are we currently working on?"
122. "Plan a task to add a new API endpoint for fetching user staking positions."
123. "What's the current status of any in-progress development tasks?"
124. "Break down 'add USDVE price oracle integration' into subtasks."
125. "What would be needed to build a Vaultedge dashboard showing TVL, mints, and liquidations?"
126. "Create a todo list for adding a simple token transfer feature."
127. "What's the standard task template you use for planning work?"
128. "Show me the current sprint board for Vaultedge development."
129. "Estimate the effort for fixing a specific bug in the liquidation math."
130. "What information do you need before starting a new task?"
131. "Plan a simple task to update the README with new deployment addresses."
132. "Break down 'add a pause button to the admin dashboard' into implementation steps."
133. "What's involved in adding a new test case for the collateral ratio calculation?"

---

## Level 2: Code Review Requests

These test Carpincho's multi-model code review orchestration.

134. "Run a code review on the latest PR in [repo name]."
135. "Do a security-focused review of the liquidation bot code."
136. "Review the smart contract changes in the last commit -- focus on potential vulnerabilities."
137. "What's the current code review process? How many models are involved?"
138. "Prioritize the findings from the last code review -- which ones need immediate attention?"
139. "Review this code snippet for common security pitfalls: [provide code]."
140. "Run a quick review on the test files -- do they cover the happy path and error cases?"
141. "Check if the new contract follows our established patterns and conventions."
142. "Review the event emissions -- are all state changes properly indexed?"
143. "What's the review turnaround time we can expect for a standard PR?"
144. "Review the error handling in the withdrawal function -- are all edge cases covered?"
145. "Run a code quality review focusing on gas optimization opportunities in the staking contract."

---

## Level 3: Development Workflow

These test Carpincho's understanding of the full development lifecycle.

146. "Walk me through the task lifecycle from planning to completion."
147. "A task just finished the planning phase. What's the next step?"
148. "The QA tester found 3 issues in the latest implementation. How do we handle feedback injection?"
149. "What models do you use for code reviews and what does each one focus on?"
150. "How do you handle a situation where a coding task has been stuck for hours?"
151. "Describe the branching strategy we use for protocol development."
152. "Walk me through the PR merge process from submission to production."
153. "How do you ensure code quality standards are maintained across the team?"
154. "What's the protocol for handling hotfixes to production?"
155. "Describe the rollback procedure if a deployment causes issues."
156. "How do you handle version conflicts when multiple PRs are targeting the same files?"
157. "Explain the continuous integration pipeline -- what checks run on each commit?"
158. "What's the process for deprecating old code or removing technical debt?"

---

## Level 4: Technical Coordination

These push Carpincho into cross-functional coordination and complex planning.

159. "We need to add a new subgraph for Vaultedge. Plan the full implementation -- contracts, indexing logic, deployment, and testing."
160. "The frontend team needs a new API. Coordinate the backend task: plan it, scope it, and set up the review process."
161. "Create a technical spec for implementing sUSDVE (staked USDVE)."
162. "Plan the testing strategy for the Vaultedge launch: what needs to be tested, in what order, by whom?"
163. "We have a potential security vulnerability reported. Walk me through the response process."
164. "Coordinate a protocol upgrade that touches contracts, tests, scripts, and documentation."
165. "Plan the technical integration with a new chain including deployment, testing, and monitoring."
166. "Design a feature freeze process for the protocol before a major audit."
167. "Create a launch checklist for the Vaultedge v2 upgrade."
168. "Coordinate the response to a reported vulnerability: triage, fix, audit, deploy, communicate."
169. "Plan a database migration for the backend API with zero downtime requirements."
170. "Coordinate a multi-repository refactor that affects shared libraries across 3 codebases."
171. "Design an integration testing strategy for a cross-contract interaction between Vaultedge and Lynex."

---

## Level 5: Advanced Scenarios

These test Carpincho's ability to handle complex, real-world situations. Use these to stress test capabilities.

172. "Three teams need the same smart contract modified in incompatible ways. How do you mediate and find a solution?"
173. "A critical bug was found in production. Walk me through the full incident response workflow."
174. "Plan a phased rollout strategy for a major protocol upgrade with backwards compatibility requirements."
175. "We need to onboard two new developers. What documentation and setup tasks should we prioritize?"
176. "Coordinate a cross-protocol integration between Vaultedge and an external DeFi protocol. Plan the full technical engagement."
177. "Audit the CI/CD pipeline for security vulnerabilities and suggest improvements."
178. "Create a disaster recovery plan for the protocol if the oracle fails."
179. "Plan a stress test suite that covers black swan scenarios for Vaultedge."
180. "Design a monitoring and alerting system for protocol health metrics."
181. "Coordinate a multi-chain expansion plan for the next 6 months."
182. "Plan a full protocol fork response: what if our main developer leaves unexpectedly?"
183. "Design a governance crisis response for when the community is deadlocked on an upgrade."
184. "Create a technical roadmap for achieving full decentralization of the protocol."
185. "Plan a protocol migration from a deprecated chain to a new L2."
186. "Coordinate a war room response to an active exploit in progress."
187. "Design a comprehensive incident playbook covering oracle failures, bridge exploits, and governance attacks."
188. "Plan a zero-knowledge proof integration for privacy-preserving transactions in Vaultedge."
189. "Coordinate a protocol rescue operation where a dependent protocol has been exploited and user funds are at risk."
190. "Create a technical contingency plan for regulatory compliance across multiple jurisdictions without compromising decentralization."

---

## Red Flags

These are warning signs that Carpincho may not be functioning well.

- **Ignores process:** Skips review steps or doesn't follow the task lifecycle.
- **Overconfident findings:** Reports critical vulnerabilities without evidence or reproducible steps.
- **Misses obvious issues:** Doesn't catch common vulnerabilities (reentrancy, overflow, access control).
- **Can't explain decisions:** Can't articulate why certain approaches were chosen.
- **Ignores safety:** Suggests destructive operations without warning or confirmation.
- **Lost context:** Forgets previous conversations or can't track task status.
- **Generic responses:** Gives boilerplate answers that don't address the specific codebase or context.
- **No tool integration:** Doesn't actually use git, boards, or reports when asked.
- **Model conflicts unresolved:** Shows no process for handling disagreement between review models.
- **Missing escalation:** Doesn't recognize when issues need human intervention.

---

## Pro Tips

Get the most out of testing with Carpincho.

- **Be specific about focus areas.** "Review for reentrancy" gets better results than "review this code."
- **Use real scenarios.** Test with actual code from the codebase, not hypotheticals.
- **Push on edge cases.** Ask "what if" questions to test depth of understanding.
- **Check his memory.** Ask about previous conversations or tasks to verify context retention.
- **Test the tools.** Verify he actually uses git, creates boards, and generates reports.
- **Cross-reference findings.** When he reports issues, ask follow-ups about severity and impact.
- **Use the 5 levels.** Start with Level 1 for basic sanity checks, escalate to Levels 4-5 for deep capability tests.
- **Mix in troubleshooting.** Unexpected bugs reveal more about his problem-solving than planned scenarios.
- **Test multi-agent coordination.** Verify he can effectively work with other agents in the ecosystem.
- **Challenge his architecture.** Ask him to defend design decisions and consider alternatives.

---

## Test Summary

| Level | Tests | Focus |
|-------|-------|-------|
| Level 1 | 13 | Task Planning |
| Level 2 | 12 | Code Review Requests |
| Level 3 | 13 | Development Workflow |
| Level 4 | 13 | Technical Coordination |
| Level 5 | 19 | Advanced Scenarios |
| **Total** | **190** | |

(End of file - total 552 lines)
