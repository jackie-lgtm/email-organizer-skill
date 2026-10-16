# Gmail and Google Workspace

## Labels in Gmail

- Labels are like tags. An email can have several and **stays in the inbox** unless it's archived. That's what we want: label and keep.
- Label names here use a number prefix so they sort as a group in the sidebar (Gmail sorts them as text, so `10`–`14` appear right after `1`. That's normal.)
- **Never use `/` in a label name.** Gmail treats it as a sub-label.

### Creating the labels by hand (if you can't create them yourself)

On a computer, at mail.google.com:
1. In the left sidebar, scroll down and click **+** next to **Labels** (or **More → Create new label**).
2. Type the name exactly, e.g. `1:-to-respond`, and click **Create**.
3. Repeat for each label they chose.
4. Optional: hover over a label → **⋮** → **Label color**. Suggested: red for 1, yellow for 6, green for 7, gray for 8.

### Applying a label by hand

Tick the emails → click the **label icon** (tag shape) in the toolbar → tick the label → **Apply**.

## Filters: automatic sorting forever

A filter labels new mail from a sender the moment it arrives, without Claude. Build these after a sort, from senders that came up more than once.

### One at a time

Gmail → **⚙ Settings → See all settings → Filters and blocked addresses → Create a new filter** → put the sender in **From** → **Create filter** → tick **Apply the label** → pick the label → **Create filter**.

Do **not** tick "Skip the Inbox", "Mark as read", "Delete it" or "Never send it to Spam". Leave those off.

### Many at once: a filters file

You can write a file the user imports in one step. Create `my-gmail-filters.xml` like this, with one `<entry>` per rule:

```xml
<?xml version='1.0' encoding='UTF-8'?>
<feed xmlns='http://www.w3.org/2005/Atom' xmlns:apps='http://schemas.google.com/apps/2006'>
  <title>Mail Filters</title>
  <entry>
    <category term='filter'></category>
    <title>Mail Filter</title>
    <content></content>
    <apps:property name='from' value='newsletter@example.com'/>
    <apps:property name='label' value='8:-marketing'/>
  </entry>
  <entry>
    <category term='filter'></category>
    <title>Mail Filter</title>
    <content></content>
    <apps:property name='from' value='calendar-notification@google.com'/>
    <apps:property name='label' value='13:-meeting-update'/>
  </entry>
</feed>
```

Rules for the file:
- Only the `from` (or `subject`) and `label` properties. **Never** include `shouldTrash`, `shouldArchive`, `shouldMarkAsRead`, `forwardTo`, or `shouldNeverSpam`.
- `from` can be a full address or a whole domain, e.g. `@chase.com`.
- Only real senders seen in their mail. Never guess addresses.
- Show the list of rules in chat before making the file.

Import: **⚙ Settings → See all settings → Filters and blocked addresses → Import filters** (bottom of the page) → **Choose file** → **Open file** → review the list → **Create filters**. Create the labels first.

To undo a filter: same page → tick it → **Delete**. That removes the rule only and never touches email.
