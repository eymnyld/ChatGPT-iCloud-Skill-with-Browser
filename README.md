<p align="center">
  <img src="skills/icloud-browser/assets/apple-mail.png" width="128" alt="iCloud Browser icon">
</p>

<h1 align="center">iCloud Browser for ChatGPT</h1>

<p align="center">
  <img src="assets/ai-generated.svg" height="128" alt="AI Generated">
</p>

A Codex/ChatGPT skill that opens iCloud web apps in the persistent cloud browser and reuses the signed-in session. It supports Mail, Calendar, Photos, Drive, Notes, Contacts, Reminders, and other capabilities exposed by iCloud.com without a local MCP server, rented server, or always-on Mac.

## Install with an AI agent

Paste this prompt into Codex, ChatGPT Work, Claude Code, or another agent with GitHub, shell, or plugin access:

```prompt
Download and install the iCloud Browser plugin from:
https://github.com/eymndev/ChatGPT-iCloud-Skill-with-Browser

If the client supports personal or Agent Plugins, install the repository root using
.codex-plugin/plugin.json. If it supports only standalone skills, install the
skills/icloud-browser directory instead. Preserve agents/openai.yaml and all assets,
including the icon.

Verify that the installed skill is named "icloud-browser" and is available in future
sessions. Do not configure mcp-icloud, IMAP/SMTP credentials, a local Mac service, or
a rented server. This skill uses the client's persistent cloud browser and should ask
me to sign in to iCloud securely only when Apple requires it.
```
(Note: in ChatGPT recommended $skill-installer skill)

## Manual install

Install this repository as a personal plugin, or upload the `skills/icloud-browser` folder as a skill in ChatGPT Work.

## Requirements

- Access to ChatGPT's cloud browser
- An Apple Account with iCloud Mail
- Interactive sign-in or two-factor authentication when Apple requests it

Passwords and verification codes must be entered only through the secure sign-in flow, never in chat.

## Contents

- `skills/icloud-browser/SKILL.md` — workflow instructions
- `skills/icloud-browser/agents/openai.yaml` — name, icon, color, and default prompt
- `.codex-plugin/plugin.json` — personal plugin manifest

## Attribution

The Apple Mail icon and AI-generated badge were supplied by the repository owner. Apple and iCloud are trademarks of Apple Inc.; this project is not affiliated with or endorsed by Apple.
