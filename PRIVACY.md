# chat2repo Privacy Policy

**Effective Date:** December 3, 2025

## The Short Version

We don't collect anything. Your data stays yours.

- Your GitHub token stays in YOUR browser
- Your notes go directly to YOUR GitHub repository
- We run no servers
- We have no analytics
- We don't know who you are or what you save

## What We Store

### In Your Browser (chrome.storage.local)
- **GitHub Personal Access Token**: To authenticate with GitHub
- **Repository settings**: Owner, repo name, branch, base path
- **Default tags**: Your preferred tags

This data never leaves your browser except when making GitHub API calls.

### On GitHub (Your Repository)
- **Markdown files you create**: The notes you explicitly save
- **File metadata**: Timestamps, source URLs, tags you choose

This goes to YOUR repository. We have no access to it.

## What We Don't Collect

- Browsing history
- ChatGPT conversations you don't explicitly save
- Analytics or telemetry
- Personal information
- Usage patterns
- IP addresses
- Device fingerprints

## Data Flow

```
Your Browser → GitHub API → Your Repository
     ↑
  That's it. We're not in this picture.
```

## Permissions Explained

| Permission | Why We Need It |
|------------|----------------|
| `storage` | Save your settings locally |
| `contextMenus` | Right-click "Save to GitHub" menu |
| `activeTab` | Get page URL/title when you click capture |
| `chatgpt.com` | Add capture buttons to ChatGPT |
| `api.github.com` | Create files in your repository |

## Your Rights

### Access
View all your data in the extension settings page.

### Delete
- **Settings**: Clear via extension options or uninstall
- **Notes**: Delete from your GitHub repository
- **Everything**: Uninstall the extension

### Export
Your notes are standard markdown files. Use Git to export everything.

## Children's Privacy

This extension is not intended for children under 13.

## Changes

We may update this policy. Check the date above.

## Contact

**Email**: support@floutlabs.com
**Privacy concerns**: privacy@floutlabs.com

**Flout Labs**
Suite 100, Cave, Clarinbridge
Co. Galway, Ireland

---

**Bottom line**: We built this because we wanted our own notes in our own repos. We don't want your data. We don't have infrastructure to store it even if we did. Your knowledge stays yours.
