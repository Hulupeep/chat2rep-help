# How to Get the Most Out of chat2repo

You've installed it. Now here's how to actually build a useful knowledge base.

---

## The Core Insight

**Capture while understanding.**

The best time to document something is when you're actively thinking about it. That's exactly when you're talking to ChatGPT — or when you've finally found that Stack Overflow answer. Don't plan to "organize notes later" — you won't. Capture in the moment.

---

## Two Ways to Capture

### From ChatGPT
Hover over any assistant message → click the send icon → done.

Best for: explanations, decisions, debugging sessions, ideas you've refined through conversation.

![clicktosend](/images/clicktosend.png)

### From Any Web Page
Select text → right-click → "Save to GitHub" → done.

Best for:
- **Stack Overflow answers** that actually solved your problem
- **Documentation snippets** you keep looking up
- **Blog posts** with insights worth keeping
- **Error messages + solutions** you'll hit again
- **API examples** that work
- **Anything you'd bookmark** (and never find again)

---

## What to Capture

### Capture Explanations You'll Need Again

When ChatGPT explains something and you think "oh, that makes sense now" — save it. Future you will forget.

Good candidates:
- Why your code works the way it does
- How a library or API actually behaves
- The difference between two confusing concepts
- Debugging steps that finally fixed the issue

### Capture Decisions and Their Reasoning

You make dozens of decisions a week. Why this approach over that one? Why this tool? Why this structure?

When you discuss a decision with ChatGPT and reach a conclusion, save the reasoning. Six months later when someone asks "why?", you'll have the answer.

### Capture Your "Invisible Runbook"

The stuff only you know:
- Why the staging server is configured that way
- How to regenerate those certificates
- What that cron job actually does
- The workaround for that weird bug

When you explain these to ChatGPT (often to remember them yourself), save them. This is your institutional knowledge.

### Capture Ideas While They're Fresh

Had a product idea? A feature concept? A potential solution to a nagging problem?

Those shower thoughts fade fast. When you flesh them out with ChatGPT, save them before they disappear.

---

## How to Capture Well

### Ask ChatGPT to Summarize for You

Instead of saving a long back-and-forth, ask:

> "Summarize what we just discussed about [topic] in a way I can reference later"

Then save that summary. Cleaner, more useful.

### Add Hashtags Inline

**chat2repo automatically extracts hashtags from your content.**

Just include hashtags anywhere in the text:

> "Summarize our discussion #architecture #decisions #api-design"

Those become searchable tags automatically — no extra step needed.

This works great with ChatGPT:
- Ask: "Summarize this and add relevant hashtags at the end"
- ChatGPT responds with: "...summary... #react #debugging #hooks"
- You save it — tags extracted automatically

**Pro tip:** End your prompts with `#tags` you want:
> "Explain why we chose PostgreSQL #database #decisions #project-atlas"

### Use Tags Strategically

Tags make things findable. Some patterns that work:

**By type:**
- `#decision` — choices you made and why
- `#runbook` — operational knowledge
- `#debug` — problems and solutions
- `#idea` — things to explore later

**By project:**
- `#project-atlas`
- `#client-acme`
- `#side-project`

**By topic:**
- `#react` `#postgres` `#aws`
- `#writing` `#process` `#hiring`

Set your most common tags as defaults in Settings.

### Create a Capture Habit

The tool only works if you use it. Some triggers:

- "I'll probably forget this" → capture
- "Someone might ask me about this" → capture
- "I had to figure this out once before" → capture
- "This is exactly what I needed to understand" → capture

---

## How to Use Your Captured Knowledge

### Search on GitHub

GitHub's search is surprisingly good:
```
repo:yourusername/knowledge postgres migration
```

### Search Locally

Clone your repo and grep:
```bash
grep -r "migration" ~/repos/knowledge/
```

### Let AI Assistants Read It

This is the superpower.

When you give Claude Code or GitHub Copilot access to your repos, they can read your knowledge base. Ask:

- "How did I set up the backup system?"
- "What was my reasoning for choosing Postgres?"
- "Find my notes about React hooks"

Your past thinking becomes accessible to your AI tools.

### Review Periodically

Once a month, browse your recent captures. You'll:
- Rediscover ideas you forgot
- See patterns in what you're learning
- Find notes to expand or connect

---

## Power User Patterns

### The Decision Log

Every significant decision gets captured with:
- What options you considered
- Why you chose what you chose
- What would make you reconsider

Tag: `#decision`

### The Learning Journal

When you learn something new, capture:
- The concept explained simply
- An example that made it click
- Common mistakes to avoid

Tag: `#learned`

### The Debug Diary

When you fix a tricky bug:
- Symptoms you saw
- What you tried that didn't work
- What actually fixed it
- Why it happened

Tag: `#debug`

Future you (or your teammates) will hit the same bug.

### The Project Context

At the start of a project, capture:
- Goals and non-goals
- Key decisions and constraints
- Architecture overview

As you go, capture updates. When the project ends, you'll have documentation that actually reflects what happened.

---

## Common Mistakes to Avoid

### Capturing Everything

Not every ChatGPT message is worth saving. Be selective. If it's generic information you could Google in 10 seconds, skip it. Save the stuff that's specific to your context.

### Never Reviewing

A knowledge base you never look at is just digital hoarding. Set a monthly reminder to browse recent captures.

### Perfectionism

Don't edit extensively before saving. Capture fast, in the moment. You can always improve notes later (you probably won't, and that's fine).

### Forgetting Tags

Untagged notes are hard to find. Use inline hashtags (`#like-this`) — they're extracted automatically. Or set default tags in Settings for tags you always want.

---

## Building a Second Brain

chat2repo is one piece of a "second brain" — an external system that holds your knowledge so your actual brain doesn't have to.

The full pattern:
1. **Capture** — Get information out of your head (chat2repo does this)
2. **Organize** — Structure it so you can find it (tags and folders)
3. **Review** — Regularly revisit what you've captured
4. **Use** — Actually reference it when you need it

Most people fail at step 1 because it's too much friction. chat2repo solves that. The rest is up to you.

---

## What's Next

### Free Version
- Save ChatGPT messages ✓
- Save web selections ✓
- One repository ✓

### Pro Version (Coming Soon)
- Multiple repositories
- Custom file templates
- AI-powered auto-tagging
- Team shared repositories
- Bulk export from ChatGPT history
- Claude and Gemini support

[Join the Pro waitlist](#) or [contact us](mailto:hello@floutlabs.com) with feature requests.

---

[← Back to Home](.) | [Installation Guide](INSTALL)
