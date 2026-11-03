# Personalized Industry and Career Briefs for Claude

Every week, Claude reads up on your industry, hands you things worth saying on LinkedIn, and sums up advice from the career coaches you follow. You get three short documents in Claude. You write your own comments and posts. Claude never posts for you.

## What you get

| Brief | Arrives | What's inside | Reading time |
|---|---|---|---|
| Weekly sector brief | Sunday morning | The week's news in your topics, 5 comment targets, 2 post ideas | About 10 minutes |
| Midweek update | Wednesday morning | Up to 3 fresh items and a short nudge to finish your comments | About 3 minutes |
| Weekly career guidance | Tuesday morning | New advice from coaches you pick, plus one action to try | About 5 minutes |

You pick the days and times during setup. Look at the [sample briefs](demos/) first. The people, companies and links in them are made up.

## Who this is for

Anyone who wants to stay current in their field and join industry conversations without spending hours hunting for material. No coding needed.

## Before you start

- A Claude account that can create scheduled tasks and Claude Docs. Setup checks this for you and tells you plainly if something is missing.
- About 10 minutes.

## Set it up

Copy this message into Claude and send it:

> Please set up my weekly briefs from this GitHub repo: https://github.com/jordan-sf/claude-personalized-industry-and-career-briefs
>
> Read setup/SETUP.md in that repo and follow it. Show me the sample briefs first, ask me the setup questions in short groups, and show me a summary before you create anything.

Claude shows you the samples, asks a few short questions (each with a recommended answer), and shows you a summary. Nothing is created until you say yes.

## Where your briefs live

In Claude, as documents you can edit. Want a copy to keep? Ask Claude at any time, for example: "Export last week's brief to Word." PDF and Markdown work too.

## LinkedIn-only content

Some of your professional conversation lives only on LinkedIn: posts from the coaches you follow, and replies to your own comments. The briefs work well without it. If you want it covered, you have two choices.

### Paste mode (no automation, no risk to your account)

Copy posts or reply notifications from LinkedIn and paste them into a chat. Claude summarizes them the way the briefs do. Try this:

> Using paste mode from https://github.com/jordan-sf/claude-personalized-industry-and-career-briefs, help me with these. [paste your posts or replies here]

### LinkedIn add-on (off by default)

Setup does not ask about it. Ask Claude for it any time, and Claude explains the risks first.

**What it is for.** The add-on lets Claude read LinkedIn-only content in your own browser, so your briefs can point you to it. You do all the commenting and posting yourself. Claude never does.

It does two jobs and no others:

1. Reads recent posts from the coaches you list (used by the career guidance brief).
2. Reads your own recent comments and posts, and lists new replies and which ones are owed an answer (used by the midweek update).

**What it is not for.** Posting, commenting, reacting, messaging, connection requests, following, searching LinkedIn for people or posts, browsing feeds, or collecting data about other people.

**Read this before you turn it on.**

- LinkedIn's rules do not allow tools like this. Read [LinkedIn's rules](https://www.linkedin.com/help/linkedin/answer/a1341387) yourself. LinkedIn can limit or close your account.
- Claude only reads. It loads a small number of pages per run (about 5 for career guidance and 2 for the midweek update) and stops at any login wall or security check.
- It runs through Claude in Chrome, an extension that works inside your signed-in browser. It sees whatever is on screen, and Anthropic says malicious page content can try to steer it. Anthropic recommends a separate Chrome profile with no sensitive accounts, so use one only for this. Read Anthropic's [safety guide](https://support.claude.com/en/articles/12902428-use-claude-in-chrome-safely).
- You need Chrome and a paid Claude plan. This repo gives no install steps. Follow Anthropic's [getting started guide](https://support.claude.com/en/articles/12012173-get-started-with-claude-in-chrome).
- Your computer must be on, with the Claude desktop app and Chrome open and you signed in to LinkedIn, whenever those two briefs run.
- The weekly sector brief never opens LinkedIn.

Most people should leave it off.

## Optional: import your LinkedIn history

LinkedIn lets you download your own data. If you share a small part of it, Claude can match your usual topics, avoid repeating what you have already posted, and suggest coaches and sources you already follow. You choose what to share, and Claude keeps only a short summary. Setup mentions it at the end, and you can do it any time. [Read more](setup/linkedin-export.md).

## Privacy and safety

- Everything stays in your Claude account. This repo has no tracking and sends nothing anywhere.
- Claude never enters passwords, buys anything, accepts terms or contacts anyone for you.
- Briefs use short summaries in Claude's own words, with links to the originals.

## Change anything later

Ask Claude in plain words. For example:

- "Add a topic called restaurant technology."
- "Move my Sunday brief to Monday at 7am."
- "Turn the LinkedIn add-on on." (or off)
- "Import my LinkedIn history."
- "Pause all my briefs." or "Delete the career guidance brief."
- "Update my briefs to the newest version from the repo."

## Feedback

Questions or ideas? Open an issue in this repo. Nothing is sent to the author unless you choose to write one.

## What's in this repo

| Folder | What it holds |
|---|---|
| `setup/` | The step-by-step guide Claude follows to set you up, the LinkedIn add-on page, paste mode, and the LinkedIn history import |
| `tasks/` | The instructions for each of the three briefs |
| `shared/` | Rules every brief follows, and the template for your settings doc |
| `demos/` | Sample briefs with made-up content |

## License

MIT. Made by Jordan D. Sandford.
