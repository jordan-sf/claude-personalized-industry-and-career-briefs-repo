# Weekly sector brief

Default schedule: Sunday morning.
Reads: the Settings doc.
Writes: a new Claude Doc named "YYYY-MM-DD Weekly Brief".
LinkedIn: never used. This brief runs in the cloud and does not need the person's computer.

## Prompt to install

Placeholders: `{{VERSION}}`, `{{SETTINGS_DOC_URL}}`, `{{MIDWEEK_ON}}` (yes or no). Add the full text of `shared/rules.md` after the prompt.

---

Weekly brief run. Version {{VERSION}}. Settings doc: {{SETTINGS_DOC_URL}}. Midweek update turned on: {{MIDWEEK_ON}}.

Follow these steps exactly, and follow the rules at the end. Never open LinkedIn in this run.

1. Open the Settings doc. Read About you, Topics and sources, Notes to Claude, History, and the LinkedIn history summary (if there is one).

2. Collect news. For each topic, read each listed source. Look for a feed first (RSS or Atom), because it gives exact links, titles and dates. If a source has no feed, use its website. Take items published in the last 7 days, at most 2 per source and 3 per topic. Skip anything already in History. Open an article only to confirm its date, author and facts. If a topic has nothing new, write "No new item" for that topic.

3. Create a Claude Doc named "YYYY-MM-DD Weekly Brief" using today's real date. Make the title line "Weekly Brief: " followed by today's weekday abbreviation, month abbreviation, day and year (for example "Weekly Brief: Sun, Jun 7 2026"). Use these sections, in this order:
   - **Your week.** A checklist: "Read this brief (about 10 minutes)"; "Pick 2 comment targets and write your own comments"; "Read the midweek update" (only when the midweek update is turned on); "Optional: write one or two posts using a post idea".
   - **This week at a glance.** Up to 3 bullets on the main themes.
   - **News.** One table of all items, with the four columns from the rules.
   - **Comment targets.** Up to 5 news items most worth joining. Prefer ones where the person's field gives them something real to add. For each one give the item (linked) and its age, why it is worth joining, a one-sentence angle the person could take, and one question they could ask. Sort by topic, A to Z, then newest first. Under the heading write: "You write your own comment. Tip: add one specific detail from your own work or experience and ask an actual, real question."
   - **Post ideas.** 2 ideas for the person's own LinkedIn posts, tied to this week's items, "About you" and their career goal. Each has a hook line, 3 bullet points and a closing question.
   - **Midweek update.** Only when the midweek update is turned on. One line: "Filled in by the midweek scheduled run."
   - **Sources.** Links to every page you used.

4. Update the History section of the Settings doc with one line per item you used.

5. End with a short summary: counts per topic, anything that was blocked, and anything that needs the person's attention.
