# Email Organizer: a Claude skill for a calmer inbox

A free add-on ("skill") for Claude that sorts your unread email into a simple numbered label system: **1 to-respond**, **2 fyi**, **8 marketing**, **12 finance**, **13 meeting-update**, and more. You see what needs you at a glance. Works with **Gmail** and **Outlook**, for personal and work accounts.

**Safe by design:** email stays in your inbox and stays unread. Claude never deletes, sends, forwards, or clicks links, never asks for your password, and warns you about anything that looks like a scam.

## 👉 New here? Start with the [**Getting Started guide**](GETTING-STARTED.md)

About 15 minutes: install, connect your email, a guided setup chat, and your first sort.

## Quick install

1. Download [**email-organizer.zip**](https://github.com/jackie-lgtm/email-organizer-skill/releases/latest/download/email-organizer.zip). Don't unzip it.
2. claude.ai → **Settings → Capabilities** → turn on **Code execution and file creation** → **Skills → Upload skill**.
3. **Settings → Connectors** → connect **Gmail** or **Microsoft 365**.
4. New chat: **"Set up my email organizer."**

Check that your employer allows AI tools on work email before connecting it.

## What's in here

| File | What it does |
|---|---|
| `email-organizer/SKILL.md` | The instructions Claude follows |
| `email-organizer/references/labels.md` | The 14 labels and how each email is decided |
| `email-organizer/references/safety.md` | Phishing red flags |
| `email-organizer/references/connecting.md` | Connecting accounts, and what Claude can and can't do |
| `email-organizer/references/gmail.md` | Gmail labels and filters (including a one-click import file) |
| `email-organizer/references/outlook.md` | Outlook categories and rules |

**Don't put anything personal in this repository.** It's public. Your preferences live in your own Claude settings.

*Not affiliated with Google, Microsoft, or Anthropic.*
