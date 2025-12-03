# chat2repo

**Save ChatGPT conversations to your GitHub repository in one click.**

---

## Quick Links

| [Getting Started](INSTALL) | [How to Use](GUIDE) | [Pro Version](#roadmap-pro-version-coming-soon) | [Talk to Us](#get-in-touch) |
|:--------------------------:|:-------------------:|:-----------------------------------------------:|:---------------------------:|

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

## Why This Little Extension Matters

### Your Knowledge Is Disappearing

You've had hundreds of valuable conversations with ChatGPT:
- Debugging sessions that finally cracked a tricky bug
- Explanations that made complex concepts click
- Decisions you reasoned through with AI help
- Ideas you brainstormed and refined

Where are they now? Scattered across ChatGPT's history, unsearchable, inaccessible to your tools, one "Clear history" away from gone.

### The Problem with Note-Taking Apps

You could copy-paste into Notion, Obsidian, or Apple Notes. But:
- It takes 30 seconds each time (so you won't do it)
- Those notes sit in silos, disconnected from your code
- AI coding assistants can't read them
- If the company shuts down or you stop paying, they're gone

### Why GitHub Changes Everything

Your GitHub repositories are:
- **Searchable** — by grep, GitHub search, and your IDE
- **Accessible to AI** — Claude Code and Codex can read your repos
- **Version controlled** — see how your thinking evolved
- **Truly yours** — plain markdown files you can move anywhere
- **Permanent** — GitHub will outlive most startups

### One Click Changes the Equation

When saving takes one click instead of thirty seconds, you actually do it.

That's the whole insight. Make capture effortless, and you'll build a knowledge base without trying.

---

## How to Use It

### Save from ChatGPT
1. Hover over any assistant message
2. Click the send icon
3. Done — it's in your repo

### Save from Any Web Page
1. Select text on any page
2. Right-click → "Save to GitHub"
3. Done — captured with the source URL

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

### 2. Artists: Build a Reference Library

Color theory, historical costume details, composition principles — save research conversations and build a searchable visual reference library.

### 3. Writers: Externalize Your Style Guide

You've made hundreds of editorial decisions. Why active voice here, why this structure there. Capture the reasoning, and you've got a living style guide.

### 4. Managers: Preserve Decision Context

"Why didn't we use MongoDB?" "Why did we hire for this role first?" Six months later, you won't remember. But if you saved the ChatGPT conversation where you thought it through, you've got the answer.

### 5. Product Builders: Document Your Thinking

Market insights, competitive analysis, feature prioritization — save the conversations where you developed your product intuition, and you'll have receipts when you need them.

---

## Roadmap: Pro Version Coming Soon

We're building **chat2repo Pro** for teams and power users.

### Capture More

| Feature | Free | Pro |
|---------|------|-----|
| Save ChatGPT messages | Yes | Yes |
| Save web selections | Yes | Yes |
| Save from Claude | — | Yes |
| Save from Gemini | — | Yes |
| Bulk export ChatGPT history | — | Yes |
| Browser-wide capture hotkey | — | Yes |

### Organize Better

| Feature | Free | Pro |
|---------|------|-----|
| Multiple repositories | 1 | Unlimited |
| Custom file templates | — | Yes |
| Auto-tagging with AI | — | Yes |
| Custom folder structures | — | Yes |
| Link related notes | — | Yes |

### Work Together

| Feature | Free | Pro |
|---------|------|-----|
| Team shared repositories | — | Yes |
| Create GitHub Issues from chat | — | Yes |
| Turn conversations into PRs | — | Yes |
| Shared tag taxonomies | — | Yes |

### Integrate Everywhere

| Feature | Free | Pro |
|---------|------|-----|
| Obsidian sync | — | Yes |
| Raycast/Alfred extension | — | Yes |
| API access | — | Yes |
| Webhook notifications | — | Yes |

**Interested in Pro?** [Tell us what you need](https://forms.gle/xa1TzchiEi12phSB6)

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
- **GitHub Issues**: [Report an issue](https://github.com/floutlabs/chat2repo/issues)
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
