# Testing Guide: ApeAI (Orchestrator)

**Access:** DM only (direct message the ApeAI bot)
**What he does:** Manages all other agents, fleet operations, system health

> **Note:** ApeAI is the admin-level orchestrator. Most team members won't interact with him daily. These tests are primarily for people managing the agent infrastructure. Admin approval is required for most operations.

---

## Level 1: Fleet Status (Start Here)

1. "List all active agents and their current status"
2. "Run a health check on all agents"
3. "Which agents are currently online?"
4. "Show me the agent registry"
5. "What skills does each agent have?"

---

## Level 2: Agent Management

6. "What's the current configuration for Mila?"
7. "Check if GregAIlia's memory is working properly"
8. "What Discord channels is each agent monitoring?"
9. "When was the last heartbeat for each agent?"
10. "Are all agents on the latest template version?"

---

## Level 3: Orchestration

11. "Send a message to all agents asking for a status update"
12. "Check if any agents have errors in their recent logs"
13. "Which agents have the presentations skill?"
14. "Propose an update to Miro's configuration to add a new channel"
15. "What would it take to create a new agent for customer support?"

---

## Things to Watch For

- **Authority:** ApeAI should require admin approval for config changes
- **Accuracy:** Does he correctly report agent statuses?
- **Safety:** Does he refuse destructive operations without explicit confirmation?
- **Fleet awareness:** Does he know all 9 agents and their capabilities?
