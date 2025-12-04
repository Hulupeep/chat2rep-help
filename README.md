# chat2repo

**Now Your *Ideas* Live where your *code* Lives.**

---

## Quick Links

| [Setup](INSTALL) | [Daily Use](GUIDE) | [Tags & Magic](TAG_SET_UP) | [Make YOU Amazing](PERSONAS) | [Pro Version](PRO) | [Talk to Us](#get-in-touch) |


---

## The Philosophy

### Your Knowledge Is Leaking

Every day, you lose knowledge. Not dramatically — quietly.

You debug a tricky issue and finally understand why it happens. A week later, you've forgotten. You have a conversation with ChatGPT that crystallizes your thinking on a problem. A month later, it's buried in history. You make a decision with careful reasoning. Six months later, you can't remember why.

This isn't a memory problem. It's a capture problem.

### The Capture Gap

You *could* write things down. But you don't. Not because you're lazy — because the friction is too high. Opening a notes app, deciding where to put it, formatting it, switching back to what you were doing... it takes 30 seconds and breaks your flow.

So you tell yourself "I'll remember this" or "I'll document it later." You won't.

### One Click Changes Everything

What if saving knowledge took one click? No app switching. No decisions about where to file it. No formatting. Just: see something valuable, click, done.

That's chat2repo. When the bar is low enough, you actually clear it.

### Why GitHub?

Your GitHub repositories are:

- **Searchable** — grep, GitHub search, your IDE
- **Readable by AI** — Claude Code, Copilot, and Codex can access your repos
- **Version controlled** — your knowledge evolves, and you can see how
- **Portable** — plain markdown files you can move anywhere
- **Permanent** — no subscription, no shutdown risk, no "freemium" limits
- **Github Actions -** literally do anything with your notes. Turn them into specs, products, send them, summarize them. 

Notes in Notion are Notion's. Notes in Apple Notes are Apple's. Notes in your GitHub repo are *yours*.

### Capture While Understanding

The magic moment is when you're actively thinking about something. That's when you're talking to ChatGPT. That's when documentation should happen — not later when you've forgotten half of it.

chat2repo turns your thinking-out-loud into persistent knowledge.

---

## Getting Started

### Step 1: Install the Extension

**Chrome Web Store** (Recommended)
- Visit [chat2repo on Chrome Web Store](#) <!-- Link when published -->
- Click "Add to Chrome"

**Manual Install** (Developers)
```bash
git clone https://github.com/floutlabs/chat2repo
cd chat2repo && npm install && npm run build:extension
# Chrome → Extensions → Developer mode → Load unpacked → select dist/
```

---

### Step 2: Create a GitHub Token

You need a Personal Access Token (PAT) so the extension can save files to your repo.

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Click **"Generate new token"** → **"Generate new token (classic)"**
3. Give it a name like "chat2repo"
4. Select the **`repo`** scope (full control of private repositories)
5. Click **"Generate token"**
6. **Copy the token** (you won't see it again!)

> **Why `repo` scope?** The extension needs to create files in your repository. This is the minimum permission that allows that.

---

### Step 3: Create a Repository for Your Notes

If you don't have one already:

1. Go to [github.com/new](https://github.com/new)
2. Name it something like `knowledge` or `notes` or `second-brain`
3. Make it **private** (unless you want your notes public)
4. Click **"Create repository"**

---

### Step 4: Configure the Extension

1. Click the chat2repo icon in your Chrome toolbar
2. Click **"Settings"** (or right-click → Options)
3. Paste your **GitHub token**
4. Add your repository:
   - **Label**: A friendly name (e.g., "My Notes")
   - **Owner**: Your GitHub username
   - **Repository**: The repo name (e.g., "knowledge")
   - **Branch**: Usually "main"
   - **Base Path**: Where notes go (default: "chat-notes")
5. Click **"Save Settings"**

You're ready!

---

### Step 5: Save Your First Note

1. Go to [chatgpt.com](https://chatgpt.com)
2. Have a conversation (or open an existing one)
3. Hover over any **assistant message**
4. Click the **send icon** that appears
5. Check your GitHub repo — your note is there!

---

## How to Use It

### Save from ChatGPT
1. Hover over any assistant message
2. Click the send icon
3. Done — it's in your repo

### Save from Any Web Page
1. Select any text on any webpage
2. Right-click → **"Save to GitHub"**
3. Done — saved with the source URL automatically

**What you can capture:**
- Stack Overflow answers that solved your problem
- Documentation snippets you keep coming back to
- Blog posts with insights you want to remember
- Error messages and their solutions
- API references and examples
- Anything you'd normally bookmark and lose

### What Gets Saved

```markdown
---
source: chatgpt
captured_at: 2025-12-03T14:30:00Z
url: https://chatgpt.com/c/abc123
tags:
  - chatgpt
---

[The message content you captured]
```

### Where It Goes

```
your-repo/
└── chat-notes/
    └── 2025/
        └── 12/
            └── 03/
                └── your-note-title.md
```

### Finding Your Notes Later

- **GitHub**: Search in your repo
- **Local**: `grep -r "keyword" ~/repos/knowledge/`
- **AI assistants**: They can search your repos when you give them access

---

## Five Ways People Use This

### 1. Programmers: Capture Your Hidden Infrastructure

You're the only one who knows why the staging server uses port 5433, how to regenerate the SSL certs, and what that 3am cron job does. When you explain it to ChatGPT, save it. Your replacement will thank you.

**From ChatGPT:** Architecture decisions, debugging sessions, code explanations
**From the web:** Stack Overflow solutions, GitHub issues that fixed your bug, documentation snippets

### 2. Artists: Build a Reference Library

Color theory, historical costume details, composition principles — save research conversations and build a searchable visual reference library.

**From ChatGPT:** Research conversations, technique explanations, historical context
**From the web:** Tutorial snippets, reference images descriptions, artist interviews

### 3. Writers: Externalize Your Style Guide

You've made hundreds of editorial decisions. Why active voice here, why this structure there. Capture the reasoning, and you've got a living style guide.

**From ChatGPT:** Style decisions, grammar explanations, structure discussions
**From the web:** Style guide excerpts, examples of good writing, editorial standards

### 4. Managers: Preserve Decision Context

"Why didn't we use MongoDB?" "Why did we hire for this role first?" Six months later, you won't remember. But if you saved the ChatGPT conversation where you thought it through, you've got the answer.

**From ChatGPT:** Decision reasoning, tradeoff analysis, strategy discussions
**From the web:** Competitor analysis, industry benchmarks, hiring frameworks

### 5. Product Builders: Document Your Thinking

Market insights, competitive analysis, feature prioritization — save the conversations where you developed your product intuition, and you'll have receipts when you need them.

**From ChatGPT:** Market analysis, user psychology, feature prioritization
**From the web:** User research quotes, competitor features, market data

---

## Ready for Pro?

We're building **chat2repo Pro** — from knowledge capture to automatic product creation.

**The hero feature: "Go Build This"**
Turn a conversation into a working MVP. Capture an idea, and a cloud agent scaffolds your project, stubs the UI, sets up the backend, and opens a PR. You get a notification: *"Your MVP is ready."*

Plus: Claude/Gemini support, unlimited repos, AI auto-tagging, team collaboration, Obsidian sync, and more.

**Beta spots available:** 25 (first come, first served)

[**See all Pro features & join the waitlist →**](PRO)

---

## Get In Touch

We'd love to hear from you.

### Feedback

**[Share your thoughts](https://forms.gle/xa1TzchiEi12phSB6)** — What's working? What's missing? What would make this 10x better?

### Support
Having issues? Questions about setup?
**Email**: support@floutlabs.com

### Collaboration
Want to integrate chat2repo with your tool? Have a partnership idea?
**Email**: hello@floutlabs.com

### Report a Bug
Found something broken?
- **GitHub Issues**: [Report an issue](https://github.com/Hulupeep/chat2rep-help/issues/new)
- **Email**: support@floutlabs.com

### Just Say Hi
Using chat2repo in an interesting way? We'd love to hear your story.
**Email**: hello@floutlabs.com

---

## Privacy

- **No servers** — We run nothing. Zero infrastructure.
- **No tracking** — No analytics. No telemetry. Nothing.
- **Your token stays local** — Stored in your browser, sent only to GitHub.
- **Your content is yours** — Goes directly to your repo. We never see it.

[Full Privacy Policy](PRIVACY)

---

## Legal

- [Privacy Policy](PRIVACY)
- [Terms of Service](TERMS)

---

Built by [Flout Labs](https://floutlabs.com)

*Your knowledge belongs in your repository.*
