# Vex 🖤
### Your Automated Daily Executive Assistant — powered by Claude Cowork

Vex is a free AI executive assistant that runs inside [Claude Cowork](https://claude.ai). It scrapes your Slack, Gmail, and meeting notes every morning, weaves in your Google Calendar, auto-drafts client email responses, logs action items to Todoist, and delivers 5 structured briefs straight to your Slack DMs — so you start every day with full context and zero inbox anxiety.

Built by [@sofia.angeles](https://www.instagram.com) for busy professionals who are tired of drowning in messages.

---

## What Vex delivers every day

| Time | Brief | What it covers |
|------|-------|----------------|
| 6:00 AM | 💬 Slack digest | DMs + channels + unanswered messages |
| 6:00 AM | 📧 Gmail digest | Inbox scan + auto-drafted email responses |
| 6:00 AM | 🗒️ Meeting recap | Yesterday's notes + today's calendar |
| 12:00 PM | ☀️ Midday check-in | Task progress + afternoon schedule + new items |
| 5:00 PM | 🌇 EOD wrap-up | Day summary + tomorrow's first meetings |

All action items are auto-logged to Todoist with a clear priority system:

| Priority | Meaning |
|----------|---------|
| ⚫ P0 Critical | Immediate action — do not wait |
| 🔴 P1 High | Urgent — act today |
| 🟠 P2 Med | Action required — not same-day critical |
| ⚪ P3 Low | FYI or low stakes |
| ✅ Done | Completed — shown in midday + EOD |

Every task is tagged with its source (`vex-slack` / `vex-gmail` / `vex-meetings` / `manual`) so you always know where it came from. Vex also deduplicates — if the same topic appears in multiple briefs, it merges the context instead of creating duplicate tasks.

---

## What you'll need

Before installing Vex, connect these tools in Claude Cowork:

| Connector | Required? | What it does |
|-----------|-----------|--------------|
| **Slack** | ✅ Required | Reads channels + sends your DM briefs |
| **Gmail** | ✅ Required | Scans inbox + creates draft responses |
| **Google Calendar** | ✅ Required | Weaves your schedule into every brief |
| **Todoist** | ✅ Required | Logs and tracks all action items |
| **Granola** | Optional | Pulls meeting notes for the morning recap |

> **Don't have all of these?** Vex will still work — it just skips the steps that need missing connectors and lets you know.

---

## How to install

**Step 1 — Download the skill file**

Download [`vex-public.skill`](./vex-public.skill) from this repo.

**Step 2 — Install in Claude Cowork**

Drop the `vex-public.skill` file into Claude Cowork. It will appear as an installable skill with a **Save skill** button.

**Step 3 — Set up Vex**

Once installed, open Claude Cowork and say:

> "Set up Vex for me"

Vex will ask for:
- Your name and work email
- Your role and company
- Which Slack channels to monitor
- Your Gmail client/customer label (if you have one)
- Whether the default times (6am / 12pm / 5pm) work for you

That's it. Vex creates all 5 scheduled tasks automatically, personalised to you.

**Step 4 — Pre-approve your connectors**

Go to the **Scheduled** section in your Claude sidebar and hit **"Run now"** on each task once. This pre-approves your connectors so future runs are fully automated with no interruptions.

---

## How the Gmail auto-drafting works

Vex automatically drafts responses to your client and customer emails every morning before you wake up. Here's how:

1. **Scans your Gmail** for unread client emails (using your `Clients` label or all external emails)
2. **Classifies by priority** — P0 through P3
3. **Drafts a professional response** for every P0, P1, and P2 email
4. **Rates each draft** — Strong ✅ (ready to send) / Mixed ⚠️ (review first) / Needs work 🔴 (careful review needed)
5. **Lands the draft in Gmail**, threaded to the original email

> **Vex never auto-sends.** Every draft waits for your eyes before it goes anywhere.

**Pro tip:** Create a Gmail label called `Clients` (with sub-labels for each client) for maximum precision. Vex will scan every sub-label automatically and pick up new clients the moment you create their label — no changes to Vex needed.

---

## Customizing Vex

Vex is fully customizable after setup. Just open Claude Cowork and say things like:

- *"Update Vex to also monitor #product-updates"*
- *"Change my Slack brief to 7am instead of 6am"*
- *"Add a section to my EOD brief for tomorrow's prep"*
- *"Vex should also check my Asana tasks"*

Vex will update the relevant scheduled tasks immediately.

---

## Sharing Vex with your team

Once you've installed Vex, share the `vex-public.skill` file with your teammates. Each person installs it independently and sets it up for their own accounts — briefs are always private and personal, delivered only to your own Slack DMs.

---

## FAQ

**Is Vex free?**
Yes. Vex is a free skill that runs inside Claude Cowork. You'll need a Claude Cowork subscription to use it.

**Will Vex see my private messages?**
Vex runs inside your own Claude account and only accesses the connectors you authorize. Your data stays with your account — it's never shared.

**What if I don't use Granola?**
No problem. Vex skips the meeting recap brief and notes that Granola isn't connected. All other briefs work normally.

**Can I use a different task manager instead of Todoist?**
Yes — during setup, tell Vex you use Asana, Linear, Notion, or another tool and it will adapt accordingly.

**What time zone do the briefs run in?**
Your local time zone — no adjustment needed.

**Can I add more briefs or change the schedule?**
Absolutely. Just tell Claude Cowork what you want to change and it will update your scheduled tasks on the spot.

---

## Made with ❤️ by Amara Angeles

If Vex saves you time, share it with someone who needs it.

Follow [@amara_sofia_](#) on Instagram for more AI productivity tools.

---

*Vex is an independent skill built on Claude Cowork. It is not affiliated with or endorsed by Anthropic.*
