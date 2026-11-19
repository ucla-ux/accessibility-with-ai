# Find it, fix it, check it

UCLA UX Workshop. Three tools, one loop. **You do not need git or a terminal to start.**

> Automated tools tell you where to look. They cannot tell you whether it is a problem, or whether your fix helped anyone.

## AI principles and guardrails

1. Accuracy
2. Privacy
3. Brand and Voice
4. Accessibility
5. Usability
6. Human oversight

## Four takeaways

1. Automated tools tell you **where to look**, not whether there's a problem or how to fix it.
2. 500 flagged pages are usually **5 bugs**: group by template.
3. **AI drafts. A person decides.** Take extra care with people in images.
4. Your workflow is **one of many**.

## The three repos

Each has a **no-install** path at the top of its README. On GitHub: **Code → Download ZIP**.

| Topic | Repo | Start here |
|---|---|---|
| Lighthouse | `lighthouse-audit` | The Lighthouse tab in Chrome DevTools |
| Alt text with AI | `wp-alt-text-workflow` | `step-1-alt-prompt/` (one image), `examples/rehearsal-run/` (draft, then reviewed CSV) |
| Siteimprove and Alfa | `siteimprove` | `sample/summary-sample.md` |

- https://github.com/ucla-ux/lighthouse-audit
- https://github.com/ucla-ux/wp-alt-text-workflow
- https://github.com/ucla-ux/siteimprove

## Which option fits you?

| You have | You can |
|---|---|
| Chrome and Claude | Run Lighthouse in DevTools. Paste the samples into Claude. Review the alt-text CSV |
| A spreadsheet app | Review and edit the alt-text CSV (Modern CSV, Excel, Numbers) |
| Python 3 | Turn a Siteimprove export into a checklist table |
| Node 22+ | Run Alfa on a page |
| DDEV and an API key | Run the full alt-text workflow on a practice site |

## 1. Lighthouse: one page, four checks

Lighthouse scores **one page** on Accessibility, Performance, SEO and Best Practices. Run it from:

- a **website**: PageSpeed Insights (pagespeed.web.dev)
- **Chrome DevTools** (the steps below)
- a **browser extension**
- the **command line** (see `lighthouse-audit`)

Then use **AI** to generate a fix list.

**In Chrome DevTools, 5 steps (our main route):**

1. Open the page in a **private** Chrome window.
2. DevTools (`F12`, or `Cmd+Option+I`) → **Lighthouse** tab.
3. Choose Mobile or Desktop; tick Accessibility and Performance.
4. **Analyze page load.**
5. Read the failures **and the manual checks**. ⋮ menu → **Save as JSON**.

Tick only **Accessibility** to keep the saved file small enough to paste (a full report is 0.5 to 1 MB). Too long anyway? `lighthouse-audit` has a trim script.

**Generate the fix list.** Ask Claude: "Here is a trimmed Lighthouse report. Make a checklist of what to fix and what to test, grouped by area of work: code, design, content. One person may cover more than one area. Turn the manual checks into a keyboard and screen-reader test checklist."

**Quick look, no JSON:** https://pagespeed.web.dev. Enter a public URL and click **Analyze**. It shows the scores but has no JSON download.

A score of 100 means no automated failures. It does not mean accessible.

## 2. Alt text, the safe way

**Step 1, one image.** Upload it to Claude and paste the prompt from `step-1-alt-prompt/` in `wp-alt-text-workflow`. Edit the answer, then paste it into the Media Library.

**For a whole site, steps 2 to 4** (each has its own folder and README). Copy the repo into the site's `bin/` folder first:

2. `step-2-alt-find`: list images with no alt, as a CSV. **Review it:** delete rows, fix a wrong type.
3. `step-3-alt-generate`: Claude drafts, and may say **needs a human** (infographics, unnamed portraits). **A person reads every row.** Edit freely.
4. `step-4-alt-import`: dry run, then write. Never overwrites a person's words. Test copy first, never live.

Then check the pages, not just the Media Library.

Review checklist:
- Does it tell me something the page doesn't?
- No "image of" or "photo of"
- Under 150 characters
- Headshots: the person's name, not their looks
- Nothing invented

**People:** AI can guess at who people are and what they look like, and its guesses reflect stereotypes. Name a person only when the page does, describe only what is relevant, and have a person read every one of those rows.

Images are sent to an AI service. Check your data-use rules and consent first.

## 3. Siteimprove export to checklist

1. Siteimprove → Accessibility → Issues → filter A and AA → export CSV.
2. Convert it (the file is UTF-16 and tab-separated), then group it by page template.
3. Paste the table into Claude and ask for a checklist grouped by area of work: **code, design, content** (one person may do all three).
4. **The export is as old as the last crawl.** Re-check before you plan work.
5. Never share the raw export: it holds links with access tokens.

Alfa re-checks a page with Siteimprove's open-source rules. It sees contrast and color-only links; it cannot judge meaning.

## Skills: a prompt made reusable

A skill is a tested, named set of instructions for one task, plus the files it needs. Anyone can pick it up and get the same quality. Each step in `wp-alt-text-workflow` is a skill: a folder with a `SKILL.md`.

What goes in a skill:

```text
NAME               Short and descriptive.
WHEN TO USE        The situation that triggers it.
INPUTS             What the person must provide.
TASK               Role, context, task, why it matters, rubric.
OUTPUT FORMAT      Exactly what comes back.
RUBRIC             How to tell it's good enough to use.
SUPPORTING FILES   Style guide, examples, templates, data.
```

See a real one: `step-3-alt-generate/SKILL.md` in `wp-alt-text-workflow`.

## Learn more

- The Carpentries (Software Carpentry) lessons, for beginner-friendly Git, shell and Python: https://software-carpentry.org/lessons/
- Git is an important skill and worth the time. Want to learn? Tell your facilitator and join the Git training session (see Spring below).

## Spring

Hands-on session with a short **Git training** (Tower, plus The Carpentries' *Version Control with Git*) beforehand. See pre-work from your facilitator.
