# How to Install chat2repo

Get up and running in 5 minutes.

---

## Step 1: Install the Extension

### Chrome Web Store (Recommended)
1. Visit [chat2repo on Chrome Web Store](#) <!-- Link when published -->
2. Click **"Add to Chrome"**
3. Click **"Add extension"** in the popup

### Manual Install (Developers)
```bash
git clone https://github.com/floutlabs/chat2repo
cd chat2repo
npm install
npm run build:extension
```
Then in Chrome:
1. Go to `chrome://extensions`
2. Enable **"Developer mode"** (top right)
3. Click **"Load unpacked"**
4. Select the `packages/extension/dist` folder

---

## Step 2: Create a GitHub Token

The extension needs permission to create files in your repository.

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Click **"Generate new token"**
3. Select **"Generate new token (classic)"**
4. Fill in:
   - **Note**: `chat2repo` (or any name you'll remember)
   - **Expiration**: Choose based on your preference (90 days, 1 year, or no expiration)
   - **Scopes**: Check only **`repo`** (Full control of private repositories)
5. Click **"Generate token"**
6. **Copy the token immediately** — you won't see it again!

### Why does it need `repo` scope?

The `repo` scope is the minimum permission that allows creating files. There's no "write-only" scope in GitHub's permission model. Your token is stored only in your browser and sent only to GitHub's API.

---

## Step 3: Create a Repository

If you already have a repo you want to use, skip to Step 4.

1. Go to [github.com/new](https://github.com/new)
2. **Repository name**: Something like `knowledge`, `notes`, `second-brain`, or `chat-notes`
3. **Description**: Optional, e.g., "My captured knowledge from ChatGPT"
4. **Visibility**:
   - **Private** — Only you can see it (recommended)
   - **Public** — Anyone can see your notes
5. Check **"Add a README file"** (initializes the repo)
6. Click **"Create repository"**

---

## Step 4: Configure the Extension

1. Click the **chat2repo icon** in your Chrome toolbar
2. Click **"Settings"** (or right-click the icon → "Options")
3. Enter your **GitHub Personal Access Token**
4. Click **"Add Repository"** and fill in:

| Field | What to enter | Example |
|-------|---------------|---------|
| **Label** | A friendly name for this repo | `My Notes` |
| **Owner** | Your GitHub username | `johndoe` |
| **Repository** | The repo name | `knowledge` |
| **Default Branch** | Usually `main` | `main` |
| **Base Path** | Folder for notes | `chat-notes` |

5. (Optional) Add **Default Tags** — comma-separated tags added to every note
6. Click **"Save Settings"**

---

## Step 5: Test It

1. Go to [chatgpt.com](https://chatgpt.com)
2. Start a conversation or open an existing one
3. Find any **assistant message** (ChatGPT's response)
4. Hover over it — you'll see a **send icon** appear
5. Click it
6. You should see a **green toast notification**: "Saved to GitHub!"
7. Check your repository — your note is there!

---

## Troubleshooting

### "Failed to save" error
- **Check your token**: Make sure it's correct and hasn't expired
- **Check repo permissions**: Your token needs `repo` scope
- **Check repo exists**: Make sure owner and repo name are spelled correctly

### Button doesn't appear on ChatGPT
- **Refresh the page**: Sometimes the content script needs a reload
- **Check extension is enabled**: Go to `chrome://extensions` and make sure chat2repo is on
- **Try a different conversation**: Some UI states may not show the button

### Token security concerns
- Your token is stored in `chrome.storage.local` (only your browser can access it)
- It's sent only to `api.github.com` over HTTPS
- We have no servers — we never see your token
- You can revoke it anytime at [github.com/settings/tokens](https://github.com/settings/tokens)

---

## Next Steps

You're all set up! Now learn [how to get the most out of chat2repo](GUIDE).

---

[← Back to Home](.)
