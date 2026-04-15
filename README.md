# LMCP — Claude Code Plugin

> Give Claude Code native access to Mail, Calendar, Contacts, Teams, OneDrive, Notes, OmniFocus and 92 macOS tools. All data stays on your Mac.

[![npm](https://img.shields.io/npm/v/local-mcp)](https://www.npmjs.com/package/local-mcp)
[![platform](https://img.shields.io/badge/platform-macOS-blue)](https://local-mcp.com)
[![smithery badge](https://smithery.ai/badge/@lanchuske/local-mcp)](https://smithery.ai/server/@lanchuske/local-mcp)

---

## Install

**Option 1 — Claude Code plugin:**

```
/mcp add local-mcp
```

**Option 2 — Manual config** (`.claude/mcp.json` or `~/.claude.json`):

```json
{
  "mcpServers": {
    "local-mcp": {
      "command": "npx",
      "args": ["-y", "local-mcp@latest", "stdio"]
    }
  }
}
```

**Option 3 — Full setup** (also configures Cursor, Windsurf, VS Code):

```bash
curl -fsSL https://local-mcp.com/install | bash
```

---

## What Claude Code can access

| Service | Tools |
|---------|-------|
| **Mail** | Read, search, send, reply, move emails · Save attachments · Multiple accounts |
| **Calendar** | List, create, delete events · Multi-account (iCloud, Google, Exchange) |
| **Contacts** | Search and list from Contacts.app |
| **Microsoft Teams** | Read chats and channels · No tokens or OAuth needed |
| **OneDrive** | List, read, write, move, delete, search files |
| **Microsoft Outlook** | Read, search, send emails · List and create calendar events |
| **Word / Excel / PowerPoint** | Read and create Office documents |
| **PDF** | Extract and summarize text |
| **Reminders** | List, create, complete · Includes Microsoft To Do via macOS sync |
| **OmniFocus** | Tasks, projects, tags · Create and complete |
| **Notes** | List, read, search, create in Apple Notes |
| **Messages** | List chats, read and search iMessages |
| **Finder** | Search and list files on your Mac |
| **Safari** | List bookmarks |
| **Stocks** | Real-time quotes, charts, symbol search |

92 tools total.

---

## Example prompts with Claude Code

```
Search my emails for the Figma invoice and save it to my Downloads folder

Create a calendar event: "Deploy review" tomorrow at 11am in my Work calendar

What did the #backend channel in Teams say about the outage?

Read the contract PDF in my OneDrive Legal folder and list the key dates

Add a reminder to follow up with Marco on Friday at 9am

Create a new Apple Note with a summary of what we discussed today
```

---

## Safety

- **Read operations** run immediately with no confirmation
- **Destructive operations** (send email, delete event, write file) show a preview and ask for confirmation before executing
- No tool can take any action without a preceding read to verify the correct target

---

## Privacy

All data stays on your Mac. No cloud servers process your emails, files, or messages. The only network requests are:
- License validation to `local-mcp.com`
- Cloud Relay tunnel (optional, encrypted, only if you enable it)

GDPR and CCPA compliant by architecture.

---

## Requirements

- macOS 13 Monterey or later
- Apple Silicon or Intel
- Node.js 18+

---

## Links

- [Website](https://local-mcp.com?utm_source=claude-plugin)
- [npm](https://www.npmjs.com/package/local-mcp)
- [Smithery listing](https://smithery.ai/server/@lanchuske/local-mcp)
- Support: support@local-mcp.com
