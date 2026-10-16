# Outlook and Microsoft 365

Outlook has no labels. The closest match is **categories**: colored tags, more than one per email, and mail stays in the inbox. Use categories with the same names as the Gmail labels, so the system is identical across accounts.

(Folders are the other option, but moving mail into folders takes it out of the inbox, which isn't how this system works. Use categories unless the user specifically wants folders.)

## Creating the categories by hand

**Outlook on the web (outlook.office.com or outlook.live.com):**
1. **⚙ Settings → Mail → Categories → + Create category**.
2. Type the name, e.g. `1:-to-respond`, pick a color, and **Save**.
3. Repeat for each one they chose.

**New Outlook / Windows:** right-click any email → **Categorize → Manage categories → + New category**.

**Outlook for Mac:** select an email → **Categorize** (toolbar) → **Edit Categories → +**.

Tip: in the categories list, **star** (favorite) them so they show in the left sidebar like Gmail labels.

## Applying a category by hand

Select the emails → **Categorize** in the toolbar → pick the category.

## Rules: automatic sorting forever

**Outlook on the web:** **⚙ Settings → Mail → Rules → + Add new rule** →
- Name it, for example "Marketing: Acme newsletter"
- **Condition:** *From* → the sender's address
- **Action:** *Categorize* → the category
- Leave **Stop processing more rules** ticked
- **Save**

Do **not** add actions that delete, move to Deleted Items, forward, redirect, or mark as read.

Outlook has no simple rules-import file like Gmail's, so give the user a short numbered list (sender → category) to enter one by one, starting with the senders that send the most.

## Work accounts

Company IT may restrict rules and categories, or connectors. If an option is missing or greyed out, that's likely a company setting. Tell the user it's probably locked by their workplace, and don't look for a way around it.
