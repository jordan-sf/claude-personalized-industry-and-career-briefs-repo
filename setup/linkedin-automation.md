# LinkedIn automation option

Setup does not ask about this automation option. Follow this page only when the person asks for it, for example after seeing it in the optional extras at the end of setup.

Say this first, in these words: "The automation option lets Claude read LinkedIn-only content in your own browser, so your briefs can point you to it. You do all the commenting and posting yourself. Claude never does."

Then show the person "What it is for", "What it is not for", "What you need", "About Claude in Chrome" and "Warnings" in plain words. Offer paste mode as the no-risk alternative: the person copies LinkedIn posts or replies into a chat and you summarize them. The README has a ready-made message for it at https://github.com/jordan-sf/claude-personalized-industry-and-career-briefs-repo#optional-extras

## What it is for

Two jobs, and no others:

1. Read recent posts from the coaches you listed (about 5 LinkedIn pages per career guidance run).
2. Read your own recent comments and posts, and list new replies and which ones need an answer (1 to 2 pages per midweek run).

Only the career guidance and midweek runs use it. The weekly sector brief never opens LinkedIn.

## What it is not for

Posting, commenting, reacting, messaging, connection requests, following, searching LinkedIn for people or posts, browsing feeds, opening anyone's profile except the coaches you listed, or collecting data about other people.

## What you need

- **Chrome and a paid Claude plan.** Claude in Chrome works only in Chrome, not in other browsers or on mobile. This repo gives no install steps. Anthropic's guide has them: https://support.claude.com/en/articles/12012173-get-started-with-claude-in-chrome
- **Check the extension is ready.** Look for the Claude in Chrome tools. If they are missing, show the guide link above and wait until the person says the extension is installed. Do not explain the installation yourself.
- **The Claude desktop app, open,** on a computer that is on and awake whenever the career guidance and midweek runs happen.
- **LinkedIn, signed in** to your own account in Chrome.
- **A LinkedIn profile link for each coach.** Ask the person to paste them. If they cannot, find them with a normal web search (never by browsing LinkedIn), show them for approval, then save them in the Settings doc.

## About Claude in Chrome

**Value.** Some content sits behind a LinkedIn login. Claude in Chrome lets Claude read it in the browser where you are already signed in, which is the only way to reach it.

**Risks.** Anthropic's safety guide covers them: https://support.claude.com/en/articles/12902428-use-claude-in-chrome-safely

- It works in your signed-in browser and sees whatever is on screen, including your logged-in accounts.
- Malicious page content can try to steer it. Anthropic says its safeguards reduce this risk but do not remove it.
- You are responsible for what it does in your browser.

**Tip.** Anthropic recommends a separate browser profile without sensitive accounts. Use a Chrome profile only for this, signed in to LinkedIn and nothing else.

**Permissions.** You control which sites it can use. Anthropic's permissions guide explains how: https://support.claude.com/en/articles/12902446-claude-in-chrome-permissions-guide

## Warnings (show these in full, in bold)

1. **LinkedIn's rules do not allow tools like this. Read them first: https://www.linkedin.com/help/linkedin/answer/a1341387**
2. **LinkedIn can warn you, limit your account or close it. That is LinkedIn's decision, and the author of this repo cannot help with it.**
3. **Claude only reads. It never posts, comments, reacts, messages, connects, follows or sends anything.**
4. **Claude in Chrome works inside your signed-in browser. Use a separate Chrome profile for this, with no sensitive accounts in it.**
5. **Claude loads only a small number of pages per scheduled run (about 5 on career guidance and 2 on the midweek update). It stops at any login wall or security check and tells you.**
6. **The briefs I write for you are useful without this option, and you can choose not to enable it if you're unsure. Paste mode adds some manual work but gives you much of the same value without any risk to your account.**

## The question to ask

Ask in these words (you can split it into short paragraphs): "Some of your professional conversation lives only on LinkedIn: posts from the coaches you follow, and replies to your own comments. The optional LinkedIn automation option lets Claude read those in your own browser so your briefs can point you to them. You do all the commenting and posting yourself. Claude never does. LinkedIn's rules do not allow tools like this, and LinkedIn can limit or close your account. Most people should leave it off. Do you want it on?"

## Confirmation

Turn the automation option on only if the person clearly says they understand the warnings, in their own words. If they hesitate, leave it off. After a yes:

1. Collect the coach profile links.
2. In the midweek update and career guidance scheduled task prompts, change "LinkedIn automation option: off" to "LinkedIn automation option: on" in the first line.
3. Require the person's computer for those two tasks.
4. Set the LinkedIn automation option line in the Settings doc to on.
