---
name: icloud-browser
description: Use iCloud web apps through ChatGPT's cloud browser for Mail, Calendar, Photos, Drive, Notes, Contacts, Reminders, and related Apple iCloud tasks. Apply when the user asks to view or manage data in iCloud.com; do not use for unrelated Gmail, Google Calendar, or local macOS app requests.
---

# iCloud Browser

Open `https://www.icloud.com/` in the cloud browser automatically, then enter the relevant iCloud web app. Use a direct iCloud app URL only when it is already known to be reliable. The user should not need to name the website or ask for browser use.

Reuse the existing signed-in cloud-browser session. If Apple requires sign-in or two-factor authentication, pause at the secure sign-in flow and ask the user to complete it there. Never ask the user to paste an Apple Account password or verification code into chat.

After access is available, route the request to the appropriate web app:

- **Mail:** read, search, organize, flag, archive, draft, reply, and send.
- **Calendar:** list, search, create, edit, move, and delete events.
- **Photos:** browse photos and albums, search with the filters exposed by the site, upload, download, organize, share, and delete.
- **Drive:** browse, search, upload, download, rename, move, and delete files and folders.
- **Notes:** browse, search, create, edit, move, and delete notes.
- **Contacts:** search, inspect, create, edit, and delete contacts.
- **Reminders:** browse lists, create or edit reminders, mark them complete, and delete them.
- **Other iCloud web apps:** use them when iCloud.com exposes the requested capability and the user's intent is clear.

Treat the data and state shown by iCloud.com as the source of truth. Do not claim success until the interface visibly confirms the requested result. Report when the web interface does not expose an operation available only in a native Apple app.

For sending mail, sharing content, creating or changing events, deleting data, or other consequential actions, preserve the user's requested details and follow the normal confirmation requirements. Stop if the account, recipient, item, or intent is ambiguous.

If a request spans iCloud and another connected provider, use that provider's app for its own data and the cloud browser for iCloud, then combine the results without mixing account state.

Do not start a local `mcp-icloud` process, require a Mac to stay online, request IMAP/SMTP credentials, or suggest renting a server unless the user explicitly asks for one of those approaches.
