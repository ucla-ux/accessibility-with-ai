theme: Next, 1
autoscale: true
slidenumbers: true
language: en-US
time-budget: 90
footer: Finding and fixing accessibility problems with AI · UCLA UX Workshop
build-lists: false

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Find it, **fix it**, check it

## Lighthouse, alt text with AI, and Siteimprove with Alfa

UCLA UX Workshop

^ 90 minutes. Mostly talk and demo, with two short browser-only activities (Lighthouse in Chrome, and pasting a saved report into Claude), about 18 minutes in all. Before the room fills: open the three repos in tabs, have Chrome ready on a page from your own site, have a saved Lighthouse JSON open in a text editor, have one Claude chat open, and have the alt-rehearsal site and the before and after CSVs ready for the alt-text demo. Everything attendees do today needs only Chrome and a Claude account.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# AI principles & **guardrails**

1. **Accuracy**
2. **Privacy**
3. **Brand and Voice**
4. **Accessibility**
5. **Usability**
6. **Human oversight**

^ Frame the whole workshop with these six before any tool. Each one comes back: accuracy and human oversight in the alt-text review, privacy in what we send to an API (images and Siteimprove links with tokens), accessibility is the subject itself, and brand and voice and usability are what a skill (later) encodes so the result is consistent. Keep it to one minute; do not read the list aloud.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# About **me**

- **UX designer and web developer, IoES**
- **Accessibility officer**, Division of Physical Sciences
- **Learning Git**: an important skill worth the time. Want to learn?
- **Certified Carpentries instructor**: teaching foundational coding skills to beginners
- Goal: websites that **work for everyone**, load fast and look good

^ Keep this to about a minute for both slides. The point: I am still learning Git myself, and it is worth the time (this sets up the poll's "want to learn" question), so nothing today assumes you already know git or a terminal. The Carpentries link is in the handout (software-carpentry.org/lessons).

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# What I **studied**

- **AI Essentials**, UCLA Extension (funded by a BruinTech scholarship)
- A **year-long experiment** with various AI tools, including **Claude Code**
- **Better UX with AI** workshop (just attended)

^ Be honest that this is a year of trying things: what you see today is what worked. Move on to the poll: now it is your turn.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Tell us about **you**

1. Your role: **designer, developer, writer or editor, other**
2. Git and the command line: **never, a little, comfortable**
3. Would you like to **learn** them: **yes, maybe, no**

^ A show of hands, 3 minutes. No wrong answers, and nothing today requires git or a terminal. Count the hands and write the numbers on the run sheet. Use them like this: mostly designers and writers, spend less time on the terminal demos and more on the takeaways; mostly developers, spend more time on the demos. Note how many said "yes" to learning: that is your sign-up list for the git training session before the spring hands-on. Mention that a mix is expected and good: designers, developers and writers each own different fixes, and one person often does all three.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Four takeaways

1. Automated tools tell you **where to look**, not whether there's a problem or how to fix it
2. 500 flagged pages are usually **5 bugs**: group by template
3. **AI drafts. A person decides.** Take extra care with people in images
4. Your workflow is **one of many**

^ Say these now, in one breath, and promise to come back to each. If people remember only this slide, the workshop worked. The rest of the hour is the evidence: one example each, then how to do it yourself.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Our three sample cases

| Case | The question | Tool | You will see |
|---|---|---|---|
| **1. One page** | What does this page fail? | Lighthouse | ioes.ucla.edu scores 100; our test site scores 94 |
| **2. A media library** | How do we fix missing alt text safely? | Audit, Claude, then WP-CLI | One image by hand, then a real run: 26 images, draft and reviewed CSV |
| **3. A whole site** | Where is the work across 1,767 flags? | Siteimprove export, then Alfa | Real ioes numbers, grouped by template |

^ Each case ends the same way: find it, explain it, fix it, check it with the same tool. Repos: lighthouse-audit,  wp-alt-text-workflow, siteimprove. The IoES numbers are from the site's own Siteimprove exports, crawled 11/17 and 11/18/2026. The test site is a disposable WordPress copy, never a live site.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Today

1. **Lighthouse**: one page **(18 min)**
2. **Alt text with AI**: a media library, with skills **(22 min)**
3. **Siteimprove and Alfa**: a whole site **(17 min)**
4. **Your workflow** is one of many options **(7 min)**
5. **Take-home**, spring and questions **(12 min)**

^ Say this early: you do not need git, a terminal, or any install today. The terminal parts are demos, and each has a browser-only equivalent. Each case starts with its takeaway, then an example, then how it works, so you can stop reading whenever you have what you need.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# [fit] Case 1
# [fit] One page: Lighthouse

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Takeaways

- Lighthouse audits a single page, reports scores, identifies issues, and recommends improvements.
- Run it from 
  - website 
  - Chrome DevTools
  - browser extension
  - command line
- Save JSON report and use AI to generate a fix list

^ The takeaway first, then the proof. Repo: lighthouse-audit; its README has Pick your path at the top. Website: PageSpeed Insights (pagespeed.web.dev). The website (what the activity uses) shows the report but has no JSON download; DevTools, the extension and the command line all save JSON. All four run the same Lighthouse engine. For the website, paste the failing audits into Claude instead. One page at a time, so a whole site needs a different tool (Case 3). The demo after the activity is where "a 100 is a starting line" lands: the ioes sample scores 100, and a person still has manual checks to do.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Quick look:

## https://pagespeed.web.dev

1. Open the site above
2. Enter the URL of a page from your own site
3. Click Analyze, then switch Mobile and Desktop
4. Find the four scores. 
5. It has **no JSON download**: use DevTools to save one

^ Put the address on screen and leave it there. PageSpeed Insights runs Lighthouse for you, so there is nothing to install, and no private window needed. The page has to be public: a staging site behind a login or VPN will fail. Common snags: pasting a URL without https://, a page that redirects, and scores that differ a little between runs. Accessibility results are in the Accessibility section; the manual checks are listed under "Additional items to manually check". This is the look-only option: about 2 minutes, then move on to the DevTools activity. Fallback if wifi fails: show a Lighthouse report you saved earlier.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Activity: Chrome DevTools to fix list **(8 min)**

1. Open a page. DevTools → **Lighthouse**
2. **Mobile**, tick **Accessibility**, then **Analyze page load**
3. ⋮ menu → **Save as JSON**. Find one failing audit and one **manual check**
4. copy JSON and **paste it into Claude** after the prompt

^ This is the main show and tell. Everyone runs Lighthouse in DevTools and saves the JSON, so they see what the file is. Then they paste it into Claude after the prompt. Keep only Accessibility ticked: with all categories a saved report is 0.5 to 1 MB, but Accessibility alone is roughly 175 KB in a test on the rehearsal site, which pastes. Use the prompt on the next slide. Common snags: extensions skewing results (use a private window), the Lighthouse tab hidden under the >> menu, the saved JSON opening in a browser instead of a text editor, and a paste that is too long (untick everything but Accessibility and rerun). Ask three people for their lowest audit, then show the result on screen.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Demo: from report to fix list

1. In **Chrome DevTools**, tick either **Accessibility** and **Performance** to keep the file small
2. Run Lighthouse and **Copy as JSON**
3. Paste prompt and JSON into ChatGPT, Claude or other AI app
4. Get a fix list
5. Human review

^ Live demo in Chrome DevTools, on your own test site or a page you are happy to show. Untick Best Practices and SEO before Analyze: only the categories you tick are in the saved file. Save as JSON, open it in a text editor, copy it, and paste it into Claude after the prompt. Do not demo a live campus site you do not own. Size check before the day: in a test on the rehearsal site, the saved file with Accessibility and Performance ticked came to roughly 430 KB, and Accessibility alone roughly 175 KB. If the paste is slow or Claude says it is too long, untick Performance. Then ask for the manual-test checklist too, because a score of 100 still needs a person. The prompt to paste is the Accessibility one in the lighthouse-audit README under AI Prompts (fill in the page and device); the lighthouse-fix-list skill runs the same steps in Claude Code. Fallback if wifi fails: show a saved Claude answer.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Performance prompt

```text
Help a small UCLA web team fix a WordPress site for an academic department,
with news posts, events, faculty profiles and photo-heavy pages. Below is a
trimmed Lighthouse performance report.

1. In two sentences: how the page is doing, and the one thing hurting it most.
2. Fixes, high impact and low effort first. For each: what is wrong (plain
   language), the evidence (audit name and number), the fix and where it lives
   (theme CSS or JS, image sizes, tag manager, plugins, caching, hosting), and
   a "done when" check (an audit or metric that should improve).
3. What this report cannot tell us, and what to measure next.

Use only what is in the report. If something is missing or unclear, say so
instead of guessing.

<paste JSON here>
```
---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Accessibility prompt

```text
Help a UCLA web team make a page more accessible. Below is a trimmed Lighthouse
accessibility report. Lighthouse finds only some problems, so a good score does
not prove the page is accessible.

Make two lists, each grouped by code, design, content. These are kinds of work,
not job titles: one person may do several. Write "none" for an empty area.

1. Fix list, most people blocked first. For each failing audit: what is wrong
   (plain language), where (selector or element), the fix, and a one-line
   "done when" test.
2. Test list: the report's manual checks as a short keyboard and screen-reader
   checklist, each item in the area that would do it.

If the score is 100 or nothing failed, say so and give only the test list.
Use only what is in the report. If you are unsure, say so.

<paste JSON here>
```
---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Details: reading a report

| Part | Question it answers |
|---|---|
| Score | Roughly how many checks passed? |
| Failing audits | What exactly, on which element? |
| Not applicable / passed | What was checked at all? |
| **Manual checks** | What did it *not* test? |

Same URL, same device setting, same version, or a comparison is meaningless.

^ The manual-check list is the most valuable part for designers: it is a ready-made test plan. Free, open source, built into Chrome; audits one page; also runs from the command line and in CI. Transition: Lighthouse sees one page. A site has thousands.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# [fit] Case 2
# [fit] A media library: alt text with AI

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Takeaway: **AI drafts. A person decides.**

- Claude is allowed to say **no** and hand an image to a person
- A person reads **every row** before anything is written
- People in images need **extra care**

^ The takeaway first. Repo: wp-alt-text-workflow. The CSV is the review gate. Nothing is written until a person has read it.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Easy step: one image, **no install**

1. Upload the image to Claude
2. Paste the prompt. Fill in the three brackets
3. Read it, edit it, paste it into the Media Library

```text
Write alt text for the attached image.
Where it appears: [page]   Who it is for: [audience]
Names I can give you: [names, or "none"]
Under 150 characters. No "image of". Never describe
people's looks or guess gender, race, age or disability.
Chart or map: summarize, then say a person must write more.
```

^ Short version of the prompt in step-1-alt-prompt/README.md; the full one is there to copy. Try it live: ask the room for an image, or use one of yours. This is the whole workflow for a handful of images. Check it before pasting: names right, nobody's appearance described, nothing invented. Then say: for hundreds of images that gets slow, so here is the same idea as three steps. The same review rule applies to both.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Coverage is not description

- A theme filled missing alt with the **post title**
- Audits reported ~**100%** alt coverage
- On one page, 11 of 25 images repeated the headline already shown beside them
- Removing the fallback made the score worse and the site better

^ The one-slide story from the ioes case study. Checkers ask "is alt present?" People ask "did it tell me anything?"

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# What the review looks like

**Draft** → **a person reads every row** → **after review**

- 26 images, 5 left for a person
- Claude flagged charts and a long alt itself
- A person caught the one it missed: a **data map** it had described as a photo

On GitHub: `examples/rehearsal-run/`

^ No attendee task here. Show the two CSVs side by side (alt-draft.csv and alt-reviewed.csv from examples/rehearsal-run/). Walk the five edits: row 86 (a data map routed as a photo; a short alt cannot say what the colors mean), row 68 (156 characters, trimmed), row 10 (a placeholder replaced with the person's name), row 35 (grammar), row 53 (a graphic rewritten as a plain transcription). Ask the room whether a name in a headshot alt is enough. Tell them the two CSVs are on GitHub if they want to read them later, in any spreadsheet app.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# AI **guesses** about people

AI can guess at who people are and what they look like, and its guesses reflect stereotypes.

So alt text should:

- **Name a person only when the page does**
- **Describe only what is relevant**
- **Always get a human read**

^ This is the most important slide in the alt-text section. Pause here. The rule is not "AI is bad at this"; it is that a guess about gender, race, age or disability does harm even when it sounds neutral. The names come from the page, never from the face.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# The rule Claude follows

> **PEOPLE.** Never describe a person's physical appearance: no hair, facial features, skin, makeup, body, age, clothing, or expression.
>
> - If the context tells you who the person is, use their name.
> - Otherwise identify them by role or activity and describe the setting and what is happening.
> - A bare portrait with no setting and no name: **set needs_human to true.**
>
> Never infer gender, race, ethnicity, disability, religion or nationality from how someone looks. Never identify anyone from their face.

^ This is the real text from step-3-alt-generate/alt-generate.py, shortened. The last line was added after the first rehearsal run. Full text and the bias tips are in step-3-alt-generate/README.md under People and bias. Be honest about the limit: a prompt is an instruction, not a filter, so the human review is the safeguard. In the rehearsal run, Claude named two people from their pages and described only the setting. A rerun of the same 26 images with the new line showed no regression, but those images were already handled well: the line has not been tested on harder cases such as an unnamed portrait or a conference crowd. Say so if asked.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Details: Claude is allowed to say **no**

| Image | What Claude does |
|---|---|
| Photo | Describes it, using the page it appears on |
| Headshot | Uses the person's name; never describes appearance |
| Logo | "Org logo" |
| **Infographic** | Summarizes and sets `needs_human=1` |

^ In the real project, 92 of 1,007 images were referred to a person. That refusal is the feature.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Details: automate it for a site

```text
Step 1  prompt      one image, no install
Step 2  find        images with no alt -> missing-alt.csv + .json
          review    a person edits the CSV: delete rows, fix route
Step 3  generate    AI writes a draft, or refuses -> alt-draft.csv
          review    a person reads every alt -> alt-reviewed.csv
Step 4  import      dry run first, then write
```

^ Repo: wp-alt-text-workflow. Folders are named step-1-alt-prompt through step-4-alt-import, each with a script, a README and a skill so Claude Code can run it. Two human gates, both in a CSV editor. Optional extra in step 4, alt-fix-pages.php, fixes pages that were saved with empty alt. Each step saves its reports in a reports/ folder next to its script.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Per site: copy the scripts in

```bash
cd ~/Sites/<site>
mkdir -p bin
cp -R ~/Git/wp-alt-text-workflow bin/wp-alt-text-workflow
echo 'bin/wp-alt-text-workflow/' >> .gitignore

ddev wp eval-file bin/wp-alt-text-workflow/step-2-alt-find/alt-find.php
```

- Scripts live in the site's `bin/`, **out of its git** (`.gitignore`)
- Each step saves its reports in its own `reports/` folder
- No DDEV? Drop `ddev` and use `wp`

^ Do this once per site, on a test copy. The copy keeps the scripts next to the site so the paths are short, and the .gitignore line stops them and their reports (which name your pages and images) from being committed to the site's repo. Then the whole of step 2 is one command. Steps 3 and 4 use the same bin path.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Skills

**A skill is a prompt made reusable.**

A tested, named set of instructions for one task, plus the files it needs. Anyone can pick it up and get the same quality.

^ Each step in the alt-text repo is a skill: a folder with a SKILL.md (alt-find, alt-generate, alt-import, alt-prompt). Claude Code finds it, runs the script, and follows the same rules every time. Tested means you ran it on real input and checked the output, not just wrote it down.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# What goes in a skill

```text
NAME
Short and descriptive.

WHEN TO USE
The situation that triggers it.

INPUTS
What the person must provide.

TASK
Role, context, task, why it matters, rubric.

OUTPUT FORMAT
Exactly what comes back.

RUBRIC
How to tell it's good enough to use.

SUPPORTING FILES
Style guide, examples, templates, data.
```

^ Open step-3-alt-generate/SKILL.md next to this as a real example. Its supporting file is the people rule inside the script. The rubric is the review checklist: names right, under 150 characters, nothing invented.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Demo: dry run, then write

```bash
S=bin/wp-alt-text-workflow
CSV=$S/step-3-alt-generate/reports/alt-reviewed.csv
ddev wp eval-file $S/step-4-alt-import/alt-import.php $CSV          # plan
ddev wp eval-file $S/step-4-alt-import/alt-import.php $CSV execute  # write
```

- Never overwrites alt a person wrote
- Skips `needs_human` rows
- Saves a rollback list

^ Show the rehearsal site, not a real one. Before: Media > Library in list view, mostly red "missing" in the Alt text column (the rehearsal mu-plugin). The repo is already copied into the site's bin/ folder. Run the dry run (21 ready, 5 left for a human), then execute, flush the cache, reload: 21 rows now show text, 5 stay red. Then show the rollback, using the saved rollback list, and rerun the dry run to prove it is back to 21 ready. Rule: test copy first, snapshot before the pages step, never the live site. Live generation was verified 2026-11-18 with claude-sonnet-5-5 on 26 images; keep that output as your fallback.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Safety rules

- Test copy first. Dry run is the default
- A person reviews every row before it is written
- Never overwrite a person's words
- **People: a human reads every one**, because AI guesses reflect stereotypes
- Images go to an AI service: **check your data rules**

^ Pause for questions on privacy and consent. Do not send images of people who have not agreed.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# [fit] Case 3
# [fit] A whole site: Siteimprove and Alfa

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Takeaway: 500 pages is usually **5 bugs**

- Same template, same defect, hundreds of pages
- Group by **template**, and the list is short and assignable
- The export is **a photograph**: it may already be out of date

^ The takeaway first. Repo: siteimprove. Attendees without Siteimprove access still do the activity with the sample.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# What 1,767 flags look like

| Issue | Template | Pages |
|---|---|---|
| Content missing after heading | `/publication/` | 671 |
| Link missing a text alternative | `/person/` | 437 |
| Headings are not structured | `/project/` | 222 |
| Color contrast | `/event/` | 28 |

^ Real numbers from seven issue exports of the ioes site, crawled 11/17 and 11/18/2026: 1,767 flags, each a page and issue pair, grouped by template. One template, one defect, hundreds of pages. Say the stale-crawl point in one sentence: on the ioes project, five of fourteen re-testable rule types were already fixed when re-tested, which is why you re-check before planning work.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Activity: sample to checklist **(10 min)**

1. Open `sample/summary-sample.md` (link on the handout)
2. Paste it into Claude with the prompt from the README
3. Ask: **Which three items remove the most flagged pages?**
4. Mark each item **code, design or content**

No Siteimprove account needed. Work in pairs.

^ The sample is made-up data from a fictional institute. Fallback prompt if people lose the README: "Turn this table into a to-do list grouped by code, design and content." Compare answers around the room: people will disagree about which area an item belongs to, and that is the point. Remind them one person often does all three, so these are kinds of work, not job titles. Anyone without Claude can label the printed table by hand.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Demo: your own export, in 3 minutes

1. Export one issue at a time from Siteimprove
2. Convert and group it by template (two commands)
3. Paste the short table into Claude
4. Read the checklist: **code, design, content**

^ Use your real ioes summary (tmp/run1 or the short summary), not the raw file. Never open the raw export on screen: its Page Report column holds links with access tokens. Commands: python3 scripts/flatten_siteimprove.py <folder> flat.csv, then python3 scripts/summarize_issues.py flat.csv --min-pages 3 --examples 2. Skim the example URLs first for anything you would not show publicly. Tip to say: working one issue at a time keeps the list finishable. Fallback if anything misbehaves: sample/summary-sample.md.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Details: what Siteimprove gives you

- Crawls the **whole site** on a schedule and lists issues by rule and page
- You export it as a file, a snapshot of the **last crawl**
- Re-check a page **now** with Alfa, without waiting for the next crawl

^ Skip the file-format details (UTF-16, nested rows); they are in the README.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Who catches **what**

| Sample page, 19 planted defects | Caught |
|---|---|
| Markup re-test | 9 |
| **Alfa** | 15 |
| **Lighthouse** | 10 (+2 notes) |
| No tool at all | 2 |

**Alfa** is Siteimprove's open-source rule engine. You run it yourself on one page you choose.

^ Source: measured 2026-11-10 on the fictional fixture page. Different tools, different gaps. Two defects need a person. Optional 3-minute Alfa demo: node alfa-scan.mjs sample/sampler/broken.html shows 22 failures across 17 rules; fixed.html shows none. That is also how you re-check a page without waiting for the next Siteimprove crawl. No-terminal equivalent: read alfa/expected/broken.txt. Do not go into Alfa versus Playwright here; it is in the siteimprove README for spring.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# [fit] Your workflow
# [fit] is one option

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# How I do it

- **Terminal** and **git** for repeatability
- **DDEV** for a safe copy of the site
- **Claude Code** to adapt scripts to my site
- **Spreadsheet or Modern CSV** for the review step

^ Be explicit: this is what works for you, not the standard. Show your actual terminal for two minutes, no more. Mention the setup in one breath: DDEV for a disposable copy, Python and the Anthropic API for generation, a spreadsheet for review. The README starts with an Assumptions list so people can see which parts are yours and which are required. Call back to the opening poll: name how many people said they were comfortable with a terminal, and how many wanted to learn.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Other ways to get there

| If you prefer | Do this |
|---|---|
| Browser only | Lighthouse in DevTools, paste exports into Claude |
| Spreadsheets | Review the CSV in Excel or Numbers |
| Chat with a developer | Hand them the grouped checklist |
| No-code | Edit alt text by hand in the Media Library, a few images at a time |
| Terminal | The three repos, step by step |

^ Every row ends in the same place: a person decided. The tool choice is yours.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# The four takeaways, again

1. Automated tools tell you **where to look**, not whether there's a problem or how to fix it
2. 500 flagged pages are usually **5 bugs**: group by template
3. **AI drafts. A person decides.** Take extra care with people in images
4. Your workflow is **one of many**

^ Close the loop with the same four lines from the start. Ask which one surprised people.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Take home

| Repo | Start here |
|---|---|
| **github.com/ucla-ux/lighthouse-audit** | Samples, then DevTools |
| **github.com/ucla-ux/wp-alt-text-workflow** | The prompt, then the before and after CSVs |
| **github.com/ucla-ux/siteimprove** | `sample/summary-sample.md`, then Alfa |

Each README has a **no-install path**. Download as ZIP; no git needed.

^ Hand out the one-page sheet. All three repo URLs are in.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Spring: hands-on

- **Before:** a short git training session (Tower and Software Carpentry)
- **Then:** build it yourself on a practice site
- **Bring:** laptop, Node, Python, and (for alt text) DDEV

^ Gauge interest by show of hands, and compare with the opening poll. Collect emails for the git training session from everyone who said yes or maybe to learning.

---

[.background-color: #005587]
[.text: #FFFFFF, Helvetica]
[.text-strong: #FFFFFF, Helvetica Bold]
[.text-emphasis: #FFFFFF, Helvetica Oblique]
[.header: #FFD100, Helvetica Bold]
[.link: #FFD100, Helvetica]
[.list: #FFFFFF, bullet-color(#FFD100)]
[.quote: #FFFFFF, Helvetica]
[.table-separator: #FFFFFF]
[.footer-style: #FFFFFF, Helvetica]
[.slidenumber-style: #FFFFFF, Helvetica]

# Questions

Find it. **Fix it.** Check it with the same tool.

^ Leave this up. Take the last minutes for open discussion; ask what page or template they would try first.
