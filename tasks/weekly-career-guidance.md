# Weekly career guidance

Default schedule: Tuesday morning.
Reads: the Settings doc.
Writes: a new Claude Doc named "YYYY-MM-DD Career Guidance Brief".
LinkedIn: used only when the automation option is on, for one job: recent posts from the listed coaches.

## Prompt to install

Placeholders: `{{VERSION}}`, `{{SETTINGS_DOC_URL}}`, `{{LINKEDIN_AUTOMATION}}` (on or off). Add the full text of `shared/rules.md` after the prompt.

---

Career guidance run. Version {{VERSION}}. Settings doc: {{SETTINGS_DOC_URL}}. LinkedIn automation option: {{LINKEDIN_AUTOMATION}}.

Follow these steps exactly, and follow the rules at the end.

1. Open the Settings doc. Read About you (including the career goal), Career advice sources, Notes to Claude, History, and the LinkedIn history section.

2. For each career advice source, look for a feed first (a blog feed, a newsletter archive, or a podcast or video channel page). If there is none, use the source's public website. When the LinkedIn automation option is "on" and the source has a LinkedIn profile link in the Settings doc, also read that coach's recent posts there (about 5 LinkedIn pages in total). Open no other profile and run no LinkedIn search. If a coach has no profile link, skip LinkedIn for that coach. When the automation option is "off", never open LinkedIn.

3. Take items from the last 7 days that give real advice, at most 5 across all sources. Skip anything already in History. Never pad with older items.

4. Create a Claude Doc named "YYYY-MM-DD Career Guidance Brief" using today's real date. Use these sections:
   - **Your one action this week.** One concrete action tied to the person's career goal, drawn from the items.
   - **One section per item.** Give the title, author, link, a two-sentence summary in your own words, and a comment angle (how the person could respond with their own experience, or apply the advice to their goal). If an item is video only, write "video, no text".
   - If there are no items, create the doc and write "No new item".
   - **Import reminder.** Only if the LinkedIn history section shows a "Last import" date more than 90 days old, add one line at the end: "Your LinkedIn history was last imported on that date. Ask me to refresh it if you want." If it says "never", add nothing.

5. If someone not on the list appears in several items or is credited by two of the listed sources, add one line under Suggested additions in the Settings doc with their name, why and a link. Do not add them to the sources list.

6. Update the History section of the Settings doc with one line per item you used.

7. End with a short summary: what you saved, the doc name, anything blocked, and any new names you suggested.
