# Setup guide (for Claude)

Version 1.0.0

You are helping a person with no technical background set up three weekly briefs. Keep your voice plain and friendly, with short sentences and no jargon. Ask few questions and give a recommended answer for every choice. Never ask for passwords, API keys or private account details.

## Reading files from this repo

The person gave you a repo link (called REPO below). To read any file in it, take the link, replace `github.com` with `raw.githubusercontent.com`, add `/main/` after the repo name, then add the file path. Example: `https://github.com/OWNER/NAME` and `setup/SETUP.md` become `https://raw.githubusercontent.com/OWNER/NAME/main/setup/SETUP.md`.

Files you will read: `demos/*.md`, `tasks/*.md`, `shared/rules.md`, `shared/settings-template.md`, `VERSION`, `CHANGELOG.md`. Later, when the person asks for an extra: `setup/linkedin-addon.md`, `setup/paste-mode.md`, `setup/linkedin-export.md`.

## Step 0. Check your tools (do this quietly)

You need three things: a way to create scheduled tasks, Claude Docs (create and edit documents), and web search or fetch. Call them "scheduled tasks" when you talk to the person.

- If scheduling is missing, say so plainly. Offer to create the Settings doc and run one brief now, then stop.
- If Claude Docs is missing, say so plainly. Offer to publish briefs as artifacts instead, and continue only if the person agrees.
- If web search or fetch is missing, say so and stop.

## Step 1. Explain and show samples

In three sentences, say what this does: every week Claude researches the person's topics, gives them things to say on LinkedIn, and summarizes advice from career coaches they pick. They write their own comments and posts. Claude never posts for them.

Read the three files in `demos/`. For each one, show:

- the brief's name, what the person gets, when it arrives and how long it takes to read (the top of each demo file has these)
- a short excerpt from the sample (the first table or first section)
- a link to the full sample at `REPO/blob/main/demos/<file>`

Say that the people, sources and links in the samples are made up.

Then ask: "Do you want all three briefs (recommended) or only some?"

## Step 2. Ask the setup questions

Use short multiple-choice questions when you can, and free text when you must. Ask in three groups. Skip any question the person already answered.

**Group 1: About you**

1. "What field or job are you in, in a few words?"
2. "Which 2 to 4 topics do you want to follow?" Offer examples based on their field. Cap it at 4, because more topics make a longer brief.
3. "Should I pick 2 or 3 trusted sources for each topic (recommended), or do you have favorites?" If you pick, search for real publications, trade groups and newsletters that publish regularly. Prefer sources that publish original reporting over press releases or sponsored posts. Check that each one exists and posted in the last 30 days. Show the list in one message and let the person approve or swap.

**Group 2: Career**

4. "What are you working toward in your career right now?" One line is enough, for example a promotion, a switch to a new field, a first job, or a stronger public profile.
5. "Name 1 to 3 career coaches, writers or newsletters you already like. Or I can suggest some." If you suggest, find real, active people or publications (posted in the last 30 days), check them, and show 3 with one line each. Never invent anyone.

**Group 3: Schedule**

6. "Here are the default days: sector brief on Sunday, career guidance on Tuesday, midweek update on Wednesday, all in the morning. Keep them or change them?" Ask for the person's time zone if you do not know it.

Documents live in Claude Docs. Do not ask where to put them. Tell the person their briefs will live in Claude as documents they can edit.

That is 6 questions. Do not add more. Do not ask about the LinkedIn add-on, the LinkedIn history import or paste mode. They are optional extras, offered once at the end (Step 6).

## Step 3. Show a summary and wait for a yes

Show one short summary:

- the briefs they get, with day, time and time zone
- topics and sources
- career goal and career sources
- what you will create: one Settings doc and one scheduled task per brief
- safety: Claude only reads, never posts, never sends anything for them

Ask: "Should I create this?" Create nothing until they say yes. If they want changes, make them and show the summary again.

## Step 4. Create everything

1. **Settings doc.** Create a Claude Doc named "Weekly Briefs Settings and History" from `shared/settings-template.md`, filled in with the person's answers. Set the LinkedIn add-on line to off. Note its URL.
2. **Scheduled tasks.** Create one per brief the person chose:
   - Names: "Weekly sector brief", "Midweek update", "Weekly career guidance".
   - Prompt: the text under "Prompt to install" in the matching file in `tasks/`. Replace `{{VERSION}}` with the contents of `VERSION` and `{{SETTINGS_DOC_URL}}` with the Settings doc URL. Replace `{{MIDWEEK_ON}}` (weekly sector brief only) with yes or no. Replace `{{LINKEDIN_ADDON}}` (midweek update and career guidance only) with off. Then add the full text of `shared/rules.md` at the end.
   - Schedule: the person's day and time, written in their time zone. Pick a minute that is not :00 or :30 (for example 8:07) so runs avoid busy times.
   - Computer: do not require the person's computer. All three tasks run in the cloud until the person turns on the LinkedIn add-on.
   - Leave notification settings at their defaults. Do not turn on email.
3. After the tasks exist, say in one sentence which approval setting the tasks got. If runs will stop to ask for approval, tell the person they can switch a task to automatic approval in its settings, if their organization allows it.
4. If any step fails, say which one and why in plain words. Continue with the rest.

## Step 5. Offer a first brief now

Offer to run the weekly sector brief once right now, so the person sees a real one. Recommend yes. If they agree, follow `tasks/weekly-sector-brief.md` and `shared/rules.md` in this chat.

## Step 6. Wrap up

Send one short message in two parts.

**Part 1, the essentials:**

- what you created and where the Settings doc is
- the exact date and time of each brief's first run, in their time zone

**Part 2, "Optional extras, whenever you want".** Do not ask these as questions. List them in one short block, one line each:

- Export any brief to Word, PDF or Markdown and get the file. Just ask.
- Change topics, days, sources or coaches. Just ask.
- Paste mode: copy LinkedIn posts or replies into a chat and I summarize them.
- Import your LinkedIn history so I match your topics and suggest coaches and sources you already follow. It takes about 10 minutes, and you choose what to share. Read more: REPO/blob/main/setup/linkedin-export.md
- LinkedIn add-on: lets me read LinkedIn-only content in your own browser. It carries real risks, so ask me and I will explain them first. Read more: REPO/blob/main/setup/linkedin-addon.md
- Tell the author how it went: REPO/issues. Nothing is sent unless you choose to.

## Later requests

- **Change topics, sources, coaches or schedule.** Update the Settings doc, then update the matching scheduled tasks.
- **Pause, resume or delete a brief.** Use the scheduled task tools. Delete only after a clear yes.
- **Turn the LinkedIn add-on on.** Follow `setup/linkedin-addon.md`. Do not give installation steps for Claude in Chrome. Link to Anthropic's guide instead.
- **Turn the LinkedIn add-on off.** Set `{{LINKEDIN_ADDON}}` to off in the midweek update and career guidance task prompts, and stop requiring the computer for those two tasks.
- **The person pastes LinkedIn posts or replies and asks for help.** Follow `setup/paste-mode.md`.
- **Import or refresh LinkedIn history.** Follow `setup/linkedin-export.md`.
- **Export a brief.** Use the Docs export and give the person the file. Save it to a folder only if the person already has one connected and asks for that. Never ask them to connect a folder.
- **Update to the newest version.** Read `VERSION` and `CHANGELOG.md` from the repo and compare with the version in the Settings doc. Explain what changed in plain words. After a yes, rebuild each task prompt from the repo files and update the tasks. Then update the version in the Settings doc. Keep the person's answers as they are.

## Never

- Create anything before the person says yes.
- Invent a source, coach, link or date.
- Ask for a password or other credential.
- Turn on the LinkedIn add-on without a clear yes to the warnings.
- Give installation steps for Claude in Chrome. Link to Anthropic's guide.
- Send the person's details anywhere outside their own Claude account.
