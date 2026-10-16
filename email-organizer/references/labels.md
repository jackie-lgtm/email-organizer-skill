# The labels, and how to decide

Each email gets **one** label. Work down this list and use the **first** one that clearly fits.

## Decision order

1. **Calendar invite, accept, decline, or reschedule** → `13:-meeting-update`
   (Subjects starting "Invitation:", "Accepted:", "Declined:", "Updated invitation:", or `.ics` invites.)
2. **Call recording, transcript, or AI meeting notes** → `9:-call-recordings`
   (Zoom, Microsoft Teams, Google Meet recordings, Otter, Fireflies, Fathom, Read.ai, "Your meeting summary".)
3. **Contract or signature request** → `10:-contracts`
   (DocuSign, Adobe Sign, Dropbox Sign, PandaDoc, "please sign", agreements, SOWs, NDAs.)
   ⚠️ Fake DocuSign emails are a common scam. If the sender's address isn't the real service, flag it instead (see safety.md).
4. **Money** → `12:-finance`
   Bills, invoices, receipts, payment confirmations, bank and credit card statements, pay stubs, tax documents.
   ⚠️ A "bank" email asking you to click and verify, unlock, or confirm anything gets flagged, not filed.
5. **Comment or @mention from a shared tool** → `3:-comment`
   (Google Docs, Microsoft Word or Teams comments, Notion, Slack mentions, Canva.)
6. **Current client** (a sender or company the user has said is a client) → `11:-clients`
7. **Possible new business**: an inquiry, a lead, a "we'd like to talk about working together" → `5:-prospect-client`
8. **Coworker asking for help** (same work domain, a request) → `14:-internal-support-request`
9. **A real person wrote and wants a reply** → `1:-to-respond`
   Signs: written to the user personally, asks a question, or is a "Re:" thread they're part of.
10. **Newsletter, promotion, sale, or marketing** → `8:-marketing`
    (Has an unsubscribe footer, comes from "news@", "hello@" or "info@", or is about a sale or offer.) Newsletters are always marketing.
11. **Automated notice that isn't money or a meeting** → `4:-notification`
    (Shipping and delivery, password-changed notices, app updates, travel itinerary updates, school or HOA portal alerts.)
12. **Everything else a human sent that needs no reply** → `2:-fyi`

## Labels the user applies, not you

- `6:-awaiting-reply`: the user marks mail they've sent and are waiting on. You may *suggest* it when you can see they replied and the other person hasn't, but don't apply it on your own during a sort.
- `7:-actioned`: the user moves things here when they're done. Offer to move `1:-to-respond` items here when they tell you they've handled them.

## When unsure

Pick your best guess, and list it under "Not sure about" in the report with one line on why. Never invent a new label. If something truly fits nothing, leave it unlabeled and say so.

## Personal vs. work

On a personal account, 5, 10, 11 and 14 are often unused. If the user skipped them in setup, use the next best fit: a personal contract goes to `12:-finance` or `2:-fyi`, and a request from a friend goes to `1:-to-respond`.
