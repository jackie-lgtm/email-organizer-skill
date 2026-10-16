# Connecting accounts, and what you can do with them

What Claude can do with email depends on how the account is connected. These tools change often, so **test, don't assume**, and tell the user plainly which mode you're in.

## Ways in

| Way | Where | Typically allows |
|---|---|---|
| **Gmail connector** | Claude → Settings → Connectors → Gmail | Search and read mail. Recent versions can also list, create and apply labels. Older versions or limited permissions may be read-only. |
| **Microsoft 365 connector** | Claude → Settings → Connectors → Microsoft 365 | Search and read Outlook mail for work and school accounts. Moving or categorizing may not be available. Personal Outlook.com and Hotmail accounts may not be supported. On a company Claude plan, an admin may need to turn it on. |
| **Claude in Chrome / Cowork** | The browser extension, or Cowork in the Claude desktop app | Works in the user's real Gmail or Outlook web page, so it can click labels and categories the same way a person would. Slower, but works when the connector is read-only. |
| **Filters and rules** | Gmail settings / Outlook rules | No Claude connection needed at all. Sorts new mail automatically, forever. |

## How to test (first run)

1. Try listing the account's labels (Gmail) or categories and folders (Outlook).
   - Works → you can at least read.
   - Fails or there's no tool → not connected. Walk them through **Settings → Connectors** and the **Connect** button. They sign in on Google's or Microsoft's own page, never in chat.
2. If you have a tool for applying labels, try it on **one** email the user picks, then re-check that the label is actually there.
   - Label is there → **Full mode**.
   - Error ("insufficient permissions", "scope", or no such tool) → **Read-only mode**. If the error mentions permissions, suggest disconnecting and reconnecting the connector once, since that sometimes grants the label permission. Then retest.
3. **Re-check every write.** A tool reporting success isn't proof. After labeling, search to confirm the label landed.

## Read-only mode: still useful

- Sort into a table and the user applies labels in a few clicks. In Gmail, select a group of emails, click the label icon, and pick the label.
- Or, if Claude in Chrome or Cowork is available, offer to do the clicking in their browser, with them watching.
- And build filters and rules (see gmail.md and outlook.md) so most of it is automatic from then on.

## Work accounts

Before connecting a work account, the user should confirm their employer allows it. Some companies block connectors entirely. If the connection is refused by their company, that's the company's choice. Don't look for workarounds. Sort the personal account only.
