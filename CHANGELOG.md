# Changelog

## 1.0.3

The optional extras (export, paste mode, LinkedIn history import, LinkedIn automation option, update, feedback) are now explained in full in a required wrap-up that comes before the first brief runs. Before, the wrap-up came after the first-brief offer, so a long first run could skip it.

## 1.0.2

Setup asks its questions with Claude's tap-to-answer choices instead of plain text, and frames each sample brief with a label and an end line so it cannot be mistaken for real content. The briefs themselves are unchanged.

## 1.0.1

Setup now works from one link and one file. The setup message carries the exact file link, because Claude opens links that are typed into the chat and blocks links it builds itself. `setup/SETUP.md` holds everything setup needs, including the instructions each brief follows, so nothing else has to be opened. A copy-and-paste backup is in the README, and every extra has its own ready-made message. The `tasks/` and `shared/` folders and the `VERSION` file are gone, since their content lives in `setup/SETUP.md`.

## 1.0.0

First release. Three weekly briefs (sector brief, midweek update, career guidance), a guided setup, sample briefs, paste mode for LinkedIn content with no LinkedIn access, an optional LinkedIn history import, and an optional LinkedIn automation option that is off by default and limited to two read-only jobs.
