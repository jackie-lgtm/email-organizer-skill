# Getting Started with Email Organizer

About **15 minutes**, done once. Each step says what you should see, so you know it worked.

**What it does:** Claude puts a numbered label on each unread email (1 to-respond, 8 marketing, 12 finance…) so you can see what matters at a glance. Your email **stays in your inbox and stays unread.** It **never deletes, sends, or forwards anything.**

You'll need a computer with a web browser for setup. After that it works on your phone too.

---

## Before you start: your work email

**Check that your employer allows AI tools to connect to your work email.** Many companies have a policy, and some need IT to approve it. If you're not sure, set up your **personal email first** and ask before adding work. Connecting work mail your company doesn't allow could put you in a bad spot. It isn't worth it.

---

## Part 1: Install the skill (about 3 minutes)

### Step 1. Download the file

Click: **[Download email-organizer.zip](https://github.com/jackie-lgtm/email-organizer-skill/releases/latest/download/email-organizer.zip)**

✅ **You should see:** `email-organizer.zip` in your Downloads folder. **Don't unzip it.**

### Step 2. Upload it to Claude

1. Go to **claude.ai** and sign in.
2. Click your **name** (bottom left) → **Settings** → **Capabilities**.
3. Make sure **Code execution and file creation** is **on**. (It's just a setting name. You're not writing code.)
4. Under **Skills**, click **Upload skill** → choose `email-organizer.zip`.

✅ **You should see:** **email-organizer** in your skills list, switched **on**.

> Already installed Travel Booker? This is the exact same process.

---

## Part 2: Connect your email (about 3 minutes)

### Step 3. Connect Gmail and/or Outlook

1. In **Settings**, click **Connectors**.
2. Find **Gmail** (for personal Gmail or work Google accounts) or **Microsoft 365** (for work Outlook), and click **Connect**.
3. A **Google** or **Microsoft** sign-in page opens. Sign in **there**, on their page.
4. Review what it asks permission for, and click **Allow**.

✅ **You should see:** the connector marked **Connected**.

🔒 **Never type your email password into a Claude chat.** Signing in only ever happens on Google's or Microsoft's own page.

> **No Connectors option, or your work account says it's blocked?** That's fine. Claude can still set up automatic sorting rules for you (Part 3 covers this), or use Plan B at the bottom.

---

## Part 3: Your first chat (about 10 minutes)

### Step 4. Start setup

Start a **new chat** and type:

> **Set up my email organizer.**

✅ **You should see:** Claude explains what it will and won't do, then asks:

- Which accounts you're using, and which is personal or work
- Which labels you want (it'll suggest skipping the business ones on personal email)
- Whether there are people whose mail you read but never answer (e.g. family). Those can be filed as **2 fyi**.

Claude also checks what it's allowed to do with your account and tells you plainly: either it can **label for you**, or it can **only read**, and then it shows you the sort and you click the labels in (it'll show you how).

### Step 5. Create your labels

Claude either creates the labels for you (after asking) or walks you through making them. It takes about 2 minutes.

✅ **You should see:** labels like `1:-to-respond` and `8:-marketing` in your Gmail sidebar, or as categories in Outlook.

### Step 6. Your first sort

Type:

> **Sort my unread email.**

✅ **You should see:**
1. How many unread emails it found
2. A table of what it plans to label each one, **before it does anything**
3. After you say OK: a summary, with **"Needs you"** at the top

If Claude gets one wrong, just tell it: *"That's finance, not marketing."* It fixes it and remembers the rule for your setup note.

### Step 7. Save your setup

At the end, Claude gives you a **"My email setup"** note. Copy it, then go to **Settings → Profile** and paste it into the box about what Claude should know about you. **Save.**

### Step 8 (optional, recommended): make it automatic

Type:

> **Make filters for the senders you saw.**

Claude makes a list of rules (sender → label). For Gmail, it gives you a file to import in a few clicks. For Outlook, you get a short list to enter. After that, new mail from those senders sorts itself, **even when Claude isn't open.**

**You're set.** 🎉 From now on, just say *"sort my email"* whenever you like.

---

## What the labels mean

| Label | Means |
|---|---|
| **1 to-respond** | Someone's waiting on a reply from you. **Start here.** |
| 2 fyi | Good to know, nothing to do |
| 3 comment | Comments and @mentions from shared docs |
| 4 notification | Automated alerts: shipping, app notices |
| 5 prospect-client | Possible new business |
| 6 awaiting-reply | You're waiting on someone (you add this one) |
| 7 actioned | Done (you move things here) |
| 8 marketing | Newsletters and promotions |
| 9 call-recordings | Call recordings and meeting notes |
| 10 contracts | Contracts and e-signatures |
| 11 clients | Current clients |
| 12 finance | Bills, receipts, statements |
| 13 meeting-update | Calendar invites and changes |
| 14 internal-support-request | Coworkers asking for help |

---

## Your safety promise

Claude will **never**:
- delete an email, or empty your trash
- send, reply to, or forward anything
- click links or "unsubscribe" in emails
- ask for your password or a texted code
- move mail between your personal and work accounts

If an email looks like a scam, Claude **leaves it alone and warns you** in a "Watch out" section. And if an email ever contains instructions aimed at Claude, it ignores them and tells you.

---

## If something doesn't work

| Problem | Fix |
|---|---|
| Download link doesn't work | Go to the [Releases page](https://github.com/jackie-lgtm/email-organizer-skill/releases/latest) and click `email-organizer.zip` |
| Claude says it can only read, not label | Normal for some accounts. Claude gives you the sort and you click labels in, and Step 8 makes most of it automatic. Or try disconnecting and reconnecting the connector once |
| Work account won't connect | Your company may block it. Use the personal account only, and ask IT if you'd like work added |
| Claude doesn't seem to use the skill | **Settings → Capabilities**: check email-organizer is on, then start a **new** chat |
| Still stuck | Text Jackie a screenshot |

---

## Plan B: no Skills option, or no connector

1. Download the zip, **double-click** to unzip it.
2. In Claude: **Projects → Create project** → name it **Email**.
3. Add `SKILL.md` and every file in `references` to **Project knowledge**.
4. In **Instructions**, paste: *Follow SKILL.md in every conversation.*
5. Start chats in that project. Without a connector, ask Claude to **"help me set up my labels and filters"**. Claude walks you through creating them and builds the filter list, and Gmail or Outlook does the sorting from then on.
