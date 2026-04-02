# Local MCP — Claude Code Plugin

> Connect Claude Code to Mail, Calendar, Contacts, Teams, OneDrive, and 80+ macOS tools. All data stays on your Mac.

[![npm](https://img.shields.io/npm/v/local-mcp)](https://www.npmjs.com/package/local-mcp)
[![platform](https://img.shields.io/badge/platform-macOS-blue)](https://local-mcp.com)

## Install

From Claude Code:

```
/plugin install local-mcp@claude-plugins-official
```

Or add manually to your MCP config:

```json
{
  "mcpServers": {
    "local-mcp": {
      "command": "npx",
      "args": ["-y", "local-mcp@latest"]
    }
  }
}
```

## What you get

82 MCP tools across 14 macOS services:

| Service | What Claude can do |
|---------|-------------------|
| **Mail** | Read, search, send, reply, move, save attachments |
| **Calendar** | List, create, delete events across all accounts |
| **Contacts** | Search and list from Contacts.app |
| **Teams** | Read chats, channels, messages (no tokens needed) |
| **OneDrive** | List, read, write, search, move, delete files |
| **Documents** | Create and read Word, Excel, PowerPoint, PDF |
| **Outlook** | Read, search, send emails, manage calendar events |
| **Reminders** | List, create, complete (includes Microsoft To Do sync) |
| **OmniFocus** | Tasks, projects, tags — create and complete |
| **Notes** | List, read, search, create in Apple Notes |
| **Messages** | List chats, read and search iMessages |
| **Stocks** | Real-time quotes, charts, symbol search |
| **Finder** | Search and list files |
| **Safari** | List bookmarks |

## Privacy

All data stays on your Mac. No cloud servers, no API tokens, no data leaves your machine. GDPR and CCPA compliant by design.

## Safety

- Email send/reply shows a preview before sending
- Calendar events require explicit calendar name
- All destructive operations require confirmation

## Requirements

- macOS 12 Monterey or later (Apple Silicon and Intel)
- Node.js 18+

## Links

- [Website](https://local-mcp.com)
- [npm package](https://www.npmjs.com/package/local-mcp)
- Support: support@local-mcp.com
