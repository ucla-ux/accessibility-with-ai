# UCLA UX Workshop 2026: facilitator run sheet

Deck: [`ux-workshop-2026-ucla.deckset.md`](./ux-workshop-2026-ucla.deckset.md). Handout: [`ux-workshop-2026-handout.md`](./ux-workshop-2026-handout.md).

**Audience:** designers, developers and writers, mixed comfort with git and the command line. The opening poll tells you the actual mix.
**Promise:** nothing to install. Chrome and a Claude account are enough. Terminal work is a demo with a browser-only twin.
**Length:** 90 minutes. If you only have 60, cut the Alfa demo and the "Other ways" slide. If Siteimprove runs long, drop the real-export demo and use the sample.

## The three repos

| Topic | Repo | Status when built (2026-11-19) |
|---|---|---|
| 1. Lighthouse | `lighthouse-audit` | Tested: live Lighthouse run and trim script on a clean clone |
| 2. Alt text with AI | `wp-alt-text-workflow` | Tested end to end on a rehearsal DDEV site, including live generation (`claude-sonnet-5-5`, 26 images, 2026-11-18; steps re-tested 2026-11-19) |
| 3. Siteimprove and Alfa | `siteimprove` | Tested: flatten, summarize, Alfa (22 failures, 17 rules, identical output) |

## Audience poll (slide 5, "Tell us about you"): write the counts here

| Question | Answers (tally) |
|---|---|
| Role: designer / developer / writer or editor / other | |
| Git and command line: never / a little / comfortable | |
| Would like to learn them: yes / maybe / no | |
| AI apps used daily or for work (pick all): see poll 4 below | |

Use it: mostly designers and writers, give the terminal demos less time. Mostly developers, give them more. Everyone who says yes or maybe goes on the sign-up list for the git training session.

### Zoom poll setup (remote or hybrid only)

In the room, a show of hands is enough: count and write the numbers above. For remote attendees, create the polls ahead of time so each one launches in one click.

1. Schedule the meeting first. Polls attach to a scheduled meeting.
2. On zoom.us, open **Meetings**, select the meeting, and scroll to **Polls/Quizzes** and choose **Add**.
3. Create seven polls. Polls 1 to 3 are single choice and match the slide. Poll 4 is multiple choice. Polls 5 to 7 are the end-of-session review, see below:

   | Poll name | Answers |
   |---|---|
   | 1 Your role | Designer / Developer / Writer or editor / Other |
   | 2 Git and command line | Never / A little / Comfortable |
   | 3 Learn git? | Yes / Maybe / No |
| 4 Which AI apps do you use daily or for work? Pick all that apply, and skip ones you have only tried. | Claude / ChatGPT / Microsoft Copilot / Google Gemini / Perplexity / GitHub Copilot or a coding assistant / Image tools (Midjourney, DALL-E) / Other / None yet |
| 5 Review: the workshop (single choice) | See below |
| 6 Review: the speaker (single choice) | See below |
| 7 Review: UCLA UX, what next (multiple choice) | See below |

4. Leave polls 1 and 2 anonymous if you like. Do not make poll 3 anonymous, so you can see who said yes or maybe. Names are not contact details: still collect emails separately for the sign-up list.
5. In the meeting, open **Polls/Quizzes**, pick a poll and **Launch Poll**. Launch one at a time, then **Share Results** and copy the counts into the table above.
6. If polling is missing from your account, fall back to a show of hands on camera, or ask for answers in the chat.

### End-of-session review polls

Launch polls 5 to 7 in the last 3 minutes, before questions close the session. Keep them anonymous so people answer honestly. Ask for names only in the sign-up list.

**Poll 5: How useful was this workshop for your work?** (single choice)

- I can use something from it this week
- I will try it, but I need more practice first
- Interesting, but not something I can use right now
- It was not what I expected

**Poll 6: How was the speaker?** (single choice, then one chat comment)

- Clear and easy to follow
- Clear, but I wanted more time on demos or activities
- Good content, but too much for 90 minutes
- Too fast or too technical for me
- Too basic for me

Then ask in the chat: **"One thing to keep, one thing to change."**

**Poll 7: What should UCLA UX offer next?** (multiple choice, pick up to 3)

- Git training with Tower (before the spring hands-on)
- Spring hands-on: run all three tools on practice material
- Accessibility reviews of our own sites, with a facilitator
- Alt text clinic: bring your media library
- Drop-in office hours: UX, AI and skills (bring your questions)
- A show-and-tell: UX and UI wins from UCLA teams
- A show-and-tell: prompts and skills your team has built
- Short recorded demos to share with my team
- Nothing more right now

Use the answers to plan the spring session. Copy the counts into the table above, and note any chat comments to add to the repo READMEs ("After the session" below).

## When to run each poll

| Poll | When | Time | Where in the deck |
|---|---|---|---|
| 1 Your role | Slide 5, "Tell us about you" | 0:05 | First question on the slide |
| 2 Git and command line | Same slide | 0:06 | Second question |
| 3 Learn git? | Same slide | 0:07 | Third question |
| 4 AI apps used daily or for work | Right after poll 3, before "Four takeaways" | 0:08 | Same slide; say it aloud |
| 5 Review: the workshop | Wrap-up, after "The four takeaways, again" | 1:20 | Before "Take home" |
| 6 Review: the speaker | Right after poll 5, then ask for the chat comment | 1:21 | Same moment |
| 7 Review: what UCLA UX should offer next | After "Spring: hands-on", before "Questions" | 1:23 | Spring slide |

Launch one poll at a time and share results briefly (10 seconds each). Polls 1 to 4 should take no more than 3 minutes together. Times are approximate: they follow the run of show below.

## Run of show

The deck goes takeaways first, then examples, then details. Each case: takeaway, example, activity or demo, details.

| Min | Section | What happens | Mode |
|---|---|---|---|
| 0:00 | **Welcome, principles, poll** | Title (1); **AI principles and guardrails (1)**; **about me (2)**: UX designer and web developer, Accessibility Officer (Physical Sciences), learning Git, Carpentries instructor, AI studies; **tell us about you (3)**: role, git and command line, want to learn: **launch Zoom polls 1 to 3, then poll 4 (AI apps)** | Talk + show of hands |
| 0:07 | **Four takeaways, three cases, agenda** | The four takeaways; our three sample cases; today's plan (7) | Talk |
| 0:14 | **Case 1: One page, Lighthouse** | Takeaway (one page, four checks, four ways to run it, AI makes the fix list); pagespeed.web.dev quick look (2); **everyone runs Lighthouse in DevTools, saves JSON, pastes it into Claude (8)**; demo report → Claude → fix list; details (18) | Activity + demo |
| 0:32 | **Case 2: A media library, alt text with AI** | Takeaway (AI drafts, a person decides); **easy step: one image, paste the prompt (try it live)**; coverage is not description; **before and after CSV**; AI guesses about people; the rule; refusal; the three automated steps; **skills: what one is and what goes in it (2)**; dry-run demo; safety (22) | Talk + demo |
| 0:54 | **Case 3: A whole site, Siteimprove and Alfa** | Takeaway (500 pages = 5 bugs); real ioes numbers; **sample → Claude → checklist (10)**; 3-minute demo on your real export; details; who catches what, with optional Alfa demo (17) | Activity + demo |
| 1:11 | **Your workflow** | How you do it; other ways; call back to the poll (7) | Talk |
| 1:18 | **Wrap-up** | The four takeaways again; take-home repos; spring plan; sign-ups; **launch review polls 5 to 7 (3)**; open questions (12) | Talk |

If you run long, shorten the Lighthouse demo first, then the Alfa demo. Never cut the before-and-after CSV walkthrough; it is the point of the alt-text section.

## Before the day (checklist)

- [ ] Repo URLs are on the **Take home** slide and the handout. Check that all three repos are pushed and the links open
- [ ] Each repo downloaded as ZIP into a clean folder and its README followed literally once
- [ ] `lighthouse-audit`: a saved Lighthouse JSON (Accessibility only) open in a text editor; Lighthouse works in your Chrome
- [ ] `siteimprove`: `sample/summary-sample.md` open; `cd alfa && npm install && npx playwright install chromium`; `node alfa-scan.mjs sample/sampler/broken.html` ends `22 failure(s)`
- [ ] `wp-alt-text-workflow`: rehearsal site at `~/Sites/alt-rehearsal` with `step-3-alt-generate/reports/alt-draft.csv` and `step-3-alt-generate/reports/alt-reviewed.csv` ready (and `tmp/before-import.sql.gz`). Rollback after the demo so you can run it again. The API key expires after 30 days; revoke it after the workshop
- [ ] Rehearsal site built (`rehearsal/README.md`) and `alt-import.php` dry-run output saved
- [ ] Claude chat open with the three prompts ready to paste
- [ ] Zoom polls created on the scheduled meeting (7 polls, see above), or a plan for a show of hands. Sign-up method for the git training list ready (form link, paper sheet or email address)
- [ ] Terminal font large, notifications off, Deckset exported to PDF as backup
- [ ] Printed or shared handout

## Fallbacks

| If this fails | Do this |
|---|---|
| Wifi | Use `sample/` and `examples/` files; they need no network. Lighthouse in Chrome and pagespeed.web.dev need the page, so keep one saved Lighthouse JSON |
| No Claude access in the room | Show your saved Claude outputs and the CSVs in `examples/rehearsal-run/`; they need no network or Claude |
| Alfa install breaks | Read `alfa/expected/broken.txt` aloud; open one rule page |
| DDEV demo breaks | Show saved dry-run output and the before and after CSVs; neither needs DDEV |
| Someone has no laptop | Pair them up; the activities work two to a screen |

## Talking points to protect

- A 100 is not accessible: ioes scored 100 on Lighthouse and 17 issue types in Siteimprove.
- 500 flagged pages are often a handful of template bugs.
- Claude's refusal (`needs_human`) is the feature.
- A person reviews every row before anything is written.
- Your workflow is one of many. Say it twice.

## After the session

- Collect emails for the git training session ([`pre-work-spring.md`](./pre-work-spring.md)).
- Post the repo links and the PDF.
- Note which questions you could not answer and add them to the repo READMEs.
