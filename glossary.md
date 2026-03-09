# Glossary & Lingo Guide

When talking to agents, using the right terminology helps them understand exactly what you want. Here's the vocabulary that matters.

---

## Core Concepts

### Skill
A specialized capability an agent has. Think of it like a trained workflow. For example, Miro has a **banner-studio** skill for creating graphics and an **openai-image-gen** skill for AI-generated images. When you ask an agent to do something that matches one of its skills, it activates that workflow automatically.

You can reference skills directly: "Use your banner-studio skill to create a Twitter card."

### Memory / Remember
Agents have persistent memory across conversations. When you say "remember this" or "keep this in mind", the agent stores it for future reference. This is how agents learn your preferences over time.

- "Remember that I prefer short tweets, max 200 characters"
- "Keep in mind that Vaultedge launched on Base on March 1st"
- "From now on, always use the Lynex brand colors for Lynex content"

### Heartbeat
A periodic self-check agents run automatically (usually every hour). During a heartbeat, agents review their goals, check for errors, and think about what they could proactively do. You don't need to worry about this -- it happens in the background.

### Retain / Recall
How agents save and retrieve important information from their long-term memory (called **Hindsight**). When something important happens in a conversation, the agent retains it. When they need context from past conversations, they recall it.

You can explicitly ask: "Recall what we discussed about the Vaultedge marketing strategy last week."

---

## Action Words That Agents Understand Well

### The most important distinction: "Propose" vs "Do"

This changes agent behavior fundamentally:

| What you say | What happens |
|---|---|
| "**Propose** a campaign strategy" | Agent outlines the plan and **waits for approval** |
| "**Suggest** 3 approaches" | Agent presents options, doesn't execute any |
| "**Create** a campaign strategy" | Agent **goes ahead and builds it** |
| "**Do** the social posts" | Agent **executes immediately** |

Use "propose" / "suggest" / "outline" when you want to review first. Use "create" / "do" / "execute" when you're ready for action. This is especially useful for high-stakes work -- always propose first, then approve.

### Create / Generate / Make
Produce something new. Works for content, files, graphics, presentations.
- "Create a Twitter thread about..."
- "Generate a banner for..."
- "Make a presentation covering..."

### Draft
Produce a first version for review. Implies you'll want to iterate.
- "Draft a partnership proposal for..."
- "Draft a campaign brief for..."

### Analyze / Review
Look at something and provide insights, feedback, or assessment.
- "Analyze our competitor's Twitter activity this week"
- "Review this budget breakdown and flag any concerns"

### Summarize
Condense information into key points.
- "Summarize the PTO policy"
- "Summarize what happened in the last DEX Sync meeting"

### Research
Look into a topic using available tools (web browsing, knowledge base, memory).
- "Research the top stablecoin protocols on Base"
- "Research what marketing strategies similar DeFi projects are using"

### Plan / Propose
Create a strategy or approach without executing it yet.
- "Plan a content calendar for March"
- "Propose a community engagement strategy for the launch"

### Execute / Do / Implement
Actually carry out an action (as opposed to planning it).
- "Execute the campaign plan we discussed"
- "Do the social posts we drafted yesterday"

### Iterate / Refine / Adjust
Modify a previous output based on feedback.
- "Make it more casual"
- "Shorten the headline"
- "Add the TVL numbers to the second point"

---

## Requesting Formats

Agents can produce output in different formats. Be explicit about what you want:

| What you say | What you get |
|-------------|-------------|
| "Write a tweet" | Short-form social post, Twitter-length |
| "Write a thread" | Multi-tweet thread with numbered posts |
| "Create a presentation" | PowerPoint (.pptx) file |
| "Design a banner" | PNG/JPEG image file |
| "Draft a doc" | Long-form document (can be uploaded to Google Drive) |
| "Give me bullet points" | Concise list format |
| "Create a table" | Structured comparison or data layout |

---

## Specifying Tone and Style

Agents respond well to tone guidance:

- "Keep it professional" -- formal, corporate-appropriate
- "Make it degen" -- crypto-native, meme-friendly, community slang
- "FAFO energy" -- bold, experimental, DeFiZoo culture
- "Keep it simple" -- no jargon, accessible to newcomers
- "Hype it up" -- enthusiastic, high-energy, launch vibes
- "Data-driven" -- focus on numbers, metrics, evidence

---

## Talking About Protocols

When referencing DeFiZoo protocols, use their names directly. Agents know all of them:

| Protocol | What it is |
|----------|-----------|
| **Vaultedge** | Stablecoin protocol (USDVE), primary strategic bet |
| **Lynex** | DEX (decentralized exchange) |
| **Catex** | DEX |
| **Pumex** | DEX |
| **Snap** | DEX |
| **Ocelex** | DEX |
| **ApeBond** | Bonding protocol (separate team under Lanky) |
| **Zoo Felines** | DEX portfolio brand |

---

## Multi-Agent Lingo

When you want agents to work together:

- "Loop in Miro" / "Ask Miro to..." -- involves another agent
- "Hand this off to Carl" -- transfers the task to another agent
- "Check with Aria" -- asks another agent for input
- "Tag @miro" -- directly mentions another agent

---

## Power User Tips

### Chained instructions
You can give multi-step instructions in one message:
"Research the top 3 DEXes on Linea by TVL, then draft a competitive analysis comparing them to Lynex, and finally create 3 tweets highlighting where Lynex wins."

### Context setting
Start a conversation by setting context that applies to everything that follows:
"For the rest of this conversation, we're planning the Vaultedge launch on Base. Target date is March 15. Target audience is DeFi power users who care about capital efficiency."

### Corrections are the strongest learning signal
When you correct an agent, it stores the correction with context and applies it going forward. Be specific:
- "No, the tone should be more casual -- we never say 'utilize', we say 'use'"
- "That's wrong, the TVL is $18M not $25M. Remember the correct number."
- "We never mention competitor names in public posts. Remember that as a rule."

The agent won't just fix the current message -- it'll avoid making the same mistake in future conversations.

### Ask for options
Instead of one output, ask for alternatives:
- "Give me 3 different tweet options for the launch announcement"
- "Propose 2 different campaign strategies -- one aggressive, one organic"

### Reference past work
Agents remember across sessions. Use that:
- "Use the same format as the tweet you wrote yesterday"
- "Apply the feedback from our last session"
- "Continue the campaign plan we started last time"
- "Recall what we discussed about the Vaultedge launch"

### Set persistent preferences
Tell agents your preferences once and they'll apply them going forward:
- "From now on, always write tweets under 220 characters"
- "I prefer bullet points over paragraphs for summaries"
- "Always use FAFO tone for community content"

### Ask agents to follow up
Agents track their own recommendations. You can ask them to check on previous work:
- "Did the campaign plan we discussed last week get implemented?"
- "Follow up on the partnership outreach we drafted"
- "What's changed since our last conversation about this?"
