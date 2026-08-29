<p align="center">
  <img src="skills/icloud-browser/assets/apple-mail.png" width="128" alt="iCloud Browser icon">
</p>

<h1 align="center">iCloud Browser for ChatGPT</h1>

<p align="center">
  <img src="assets/ai-generated.svg" height="32" alt="AI Generated">
</p>

A Codex/ChatGPT skill that opens iCloud web apps in the persistent cloud browser and reuses the signed-in session. It supports Mail, Calendar, Photos, Drive, Notes, Contacts, Reminders, and other capabilities exposed by iCloud.com without a local MCP server, rented server, or always-on Mac.

## Install

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
