# chat2repo

## Your Knowledge Deserves to Live

You've spent years building expertise. Debugging obscure issues. Setting up infrastructure. Learning hard lessons. Having conversations with AI that crystallized your thinking.

Where does all that knowledge go?

- **Notion** dies when you stop paying
- **ChatGPT history** disappears when you clear it
- **Slack threads** become unsearchable after 90 days
- **Your memory** fades faster than you'd like to admit

Meanwhile, your GitHub repositories will outlive most SaaS companies. They're searchable. They're version controlled. They're yours.

**chat2repo puts your knowledge where it belongs.**

---

## What This Actually Is

A Chrome extension that adds a button to ChatGPT messages. Click it, and that message becomes a markdown file in your GitHub repository.

That's it. No servers. No accounts. No subscription. Just your browser talking to your GitHub.

```
You: "Explain how I set up my backup system"
ChatGPT: [detailed explanation]
You: [click button]
→ github.com/you/knowledge/chat-notes/2025/12/03/backup-system.md
```

Now that knowledge is:
- Searchable by grep, GitHub search, or your AI coding assistant
- Discoverable by Claude Code, Codex, or any tool that reads your repos
- Version controlled forever
- Yours, not OpenAI's or Anthropic's

---

## Why This Matters

### Your Invisible Runbook

You have processes that exist only in your head. Scripts you wrote and forgot. Cron jobs running silently. Environment variables you set once. Workarounds for bugs nobody documented.

This is your invisible runbook. It's the difference between you and someone who just started. But it's fragile—one bout of illness, one long vacation, one job change, and it's gone.

**Make it visible.**

When you explain something to ChatGPT, you're already articulating it. That articulation is valuable. Capture it.

### Active Knowledge, Not Dead Notes

Notes in Notion sit there. Notes in your GitHub repository become part of your working environment.

When you ask Claude Code "how does my backup system work?", it can read your repository. When you search your codebase, your knowledge files are there. When you onboard someone, you can point them to actual documentation that you wrote while understanding the problem.

This isn't about hoarding information. It's about making your knowledge **active**—findable, usable, and integrated into your workflow.

---

## Five People, Five Ways to Use This

### 1. The Programmer: Capturing Your Hidden Infrastructure

**Sarah** has been at her company for three years. She's the only one who knows:
- Why the staging database is on a different port
- How to regenerate the SSL certificates
- What that mysterious cron job at 3am actually does
- Why there are two backup scripts and which one matters

Every few months, ChatGPT helps her remember or re-derive something. Now she captures it:

```
"Summarize why we use port 5433 for staging and what would break if we changed it"
→ Tag: #infrastructure #database #staging
```

When she goes on vacation, her knowledge stays. When she eventually leaves, her replacement has a fighting chance.

**The transformation**: Tribal knowledge becomes institutional knowledge.

---

### 2. The Artist: Building a Visual Reference Library

**Marcus** is a concept artist who uses ChatGPT to research visual references, historical accuracy, and design theory. He's had hundreds of conversations about:
- Color theory for specific moods
- Historical costume accuracy for different eras
- Composition principles for dynamic poses
- Material properties for realistic rendering

Before, these insights lived in his head or scattered across chat logs. Now:

```
"Explain the key differences between Victorian working-class and upper-class clothing that I should show in my illustrations"
→ Tag: #costume #victorian #research
```

When he starts a new project set in the same era, he doesn't start from scratch. He searches his repository and finds his own curated research.

**The transformation**: Research that would be lost becomes a growing reference library.

---

### 3. The Writer: Externalizing Your Editorial Voice

**Elena** is a tech writer who has developed strong opinions about documentation over years of practice. She knows:
- When to use active vs passive voice
- How to structure API references
- What makes error messages helpful
- Why certain analogies work and others fail

She often discusses writing decisions with ChatGPT. Now she captures her reasoning:

```
"I just explained to you why I prefer imperative mood in docs. Summarize my argument with the examples I gave"
→ Tag: #style-guide #writing #decisions
```

Her repository becomes her personal style guide—not abstract rules, but real decisions with real reasoning.

**The transformation**: Implicit editorial judgment becomes explicit and teachable.

---

### 4. The Manager: Preserving Decision Context

**David** leads an engineering team. Every quarter brings decisions:
- Why they chose Postgres over MongoDB
- Why they didn't hire that candidate
- Why the Q3 roadmap prioritized X over Y
- Why they structured the team the way they did

Most of this context evaporates. When someone asks "why don't we use MongoDB?", the answer is "I don't remember, we just don't."

Now, after strategic conversations with ChatGPT:

```
"Summarize the tradeoffs we discussed about database choices and why we landed on Postgres for this project"
→ Tag: #architecture #decisions #database
```

Six months later, when a new engineer asks "why Postgres?", the answer is a link.

**The transformation**: Decision amnesia becomes decision memory.

---

### 5. The Product Builder: Capturing Market Understanding

**Priya** builds products. She spends hours thinking about:
- Why users behave certain ways
- What the competition misses
- Which features are table stakes vs differentiators
- What the real job-to-be-done is

She processes a lot of this thinking with ChatGPT. The insights are valuable, but they scatter across conversations.

Now:

```
"You've helped me think through why our competitors focus on power users while the real opportunity is first-time users. Summarize my thesis with the evidence I gave"
→ Tag: #product #strategy #market
```

When she builds the pitch deck or writes the PRD, she has her own thinking to reference—not vague memories, but articulated arguments.

**The transformation**: Scattered product intuition becomes documented product strategy.

---

## How It Works

### Setup (5 minutes)
1. Install the extension
2. Create a GitHub Personal Access Token (Settings → Developer settings → Tokens)
3. Enter your token and repository in the extension settings
4. Done

### Daily Use (5 seconds)
1. Have a conversation with ChatGPT
2. See something worth keeping
3. Click the paper airplane icon
4. Optionally edit the auto-generated title
5. It's in your repository

### Finding Your Knowledge
- **GitHub search**: `repo:you/knowledge "backup"`
- **Local grep**: `grep -r "backup" ~/repos/knowledge/`
- **AI assistants**: They can read your repos when you give them access

---

## What Gets Saved

```markdown
---
source: chatgpt
captured_at: 2025-12-03T14:30:00Z
url: https://chatgpt.com/c/abc123
tags:
  - infrastructure
  - backup
  - runbook
---

Here's how your backup system works...

[The full content of the message you captured]
```

Files are organized by date:
```
your-repo/
└── chat-notes/
    └── 2025/
        └── 12/
            └── 03/
                └── backup-system-overview.md
```

---

## What This Is Not

- **Not a note-taking app**: We don't have a UI for browsing notes. Use GitHub or your editor.
- **Not a sync service**: We don't sync. We push to GitHub. One direction.
- **Not a backup tool**: Back up your repo separately. We just write to it.
- **Not cloud storage**: Everything goes to YOUR GitHub. We have no servers.

---

## Privacy

We don't have servers. We don't collect analytics. We don't know who you are.

Your GitHub token stays in your browser. Your content goes directly to GitHub's API. We never see it.

[Full Privacy Policy](PRIVACY.md)

---

## The Philosophy

### Knowledge That Works For You

The best note-taking system is the one that's actually useful. Notes that sit in an app, unsearchable by your tools, disconnected from your work—those aren't useful.

Notes in your GitHub repository are:
- Searchable by every tool you use
- Readable by AI assistants
- Version controlled
- Truly portable
- Truly yours

### Capture While Understanding

The best time to document something is when you're actively understanding it. That's exactly when you're talking to ChatGPT about it.

Don't context-switch to a note app. Click a button and keep going.

### Lower the Bar to Zero

If saving knowledge takes 30 seconds, you won't do it. If it takes one click, you might.

That's the whole design philosophy: make capture so frictionless that you actually do it.

---

## Getting Started

1. **Install**: [Chrome Web Store](#) <!-- Link when published -->
2. **Configure**: Add your GitHub token and repository
3. **Capture**: Click the button on any ChatGPT message
4. **Find**: Search your repository when you need something

---

## Support

**Email**: support@floutlabs.com
**Issues**: [GitHub Issues](https://github.com/floutlabs/chat2repo/issues)

---

## Legal

- [Privacy Policy](PRIVACY.md)
- [Terms of Service](TERMS.md)

---

Built by [Flout Labs](https://floutlabs.com)

*Your knowledge belongs in your repository.*
