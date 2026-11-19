# Spring hands-on: git training and pre-work

For attendees who want to run the tools themselves. Nothing here is needed for the November session.

## Two sessions

| Session | Length | Who | Outcome |
|---|---|---|---|
| **Git training** | 60 min | Anyone new to git | Clone a repo, see what changed, save a commit, in Tower. Then the same steps on the command line |
| **Hands-on** | 90 min | Everyone with pre-work done | Run all three tools on practice material |

## Git training

Two resources, used together:

- **Tower** ([git-tower.com](https://www.git-tower.com/)): a git app for Mac and Windows. You click instead of typing commands, so you can see what git is doing.
- **Version Control with Git**, from The Carpentries ([software-carpentry.org/lessons](https://software-carpentry.org/lessons/)): a free, beginner-friendly lesson that teaches the same ideas on the command line.

**Before the session (30 minutes)**

1. Install Tower and sign in to GitHub from it.
2. Install git if Tower asks for it. Check with `git --version` in a terminal.
3. Skim the first episodes of *Version Control with Git*: what version control is, and setting up git.

**In the session**

1. What git is for: history, undo, sharing. A repo, a commit, and a remote.
2. In Tower: clone one of the three workshop repos, open it, and read its history.
3. In Tower: change a file, see the diff, stage it, commit it.
4. The same three steps in a terminal: `git clone`, `git status`, `git log`. Open it, `pwd`, `ls`, `cd`.
5. Read an error message: three common ones and what they mean.
6. Windows and Mac differences (clipboard, `python3` vs `py`).

Keep it to those. No branching, no merging, no remotes beyond clone. Where to go next: the rest of *Version Control with Git*.

## Tool pre-work for the hands-on (30 to 45 minutes)

| Check | How | Needed for |
|---|---|---|
| Chrome | Installed | Lighthouse, Alfa |
| Claude account | Signed in | All three |
| Python 3.9+ | `python3 --version` (Windows: `py --version`) | Siteimprove scripts, Lighthouse trim, alt-text generate |
| Node 22+ | `node -v` | Lighthouse CLI, Alfa |
| Lighthouse CLI | `npm install -g lighthouse` | Topic 1 |
| Alfa | `cd siteimprove/alfa && npm install && npx playwright install chromium` | Topic 2 |
| Modern CSV or a spreadsheet app | Installed | Topic 3 review |
| **Alt text only:** DDEV and Docker or OrbStack | `ddev version` | Topic 3 full run |
| **Alt text only:** Anthropic API key | Console, then `export ANTHROPIC_API_KEY=...` | Topic 3 live generation |

Alt text needs the most setup. Attendees who skip it can still do the CSV review and see the rest demonstrated.

## Decisions to make before announcing

- Date, room, and whether remote attendees are allowed
- Who supplies API keys (personal, department, or a shared demo key you control)
- Campus approval for sending images to an AI service
- Practice material: the rehearsal site only, or a sanitized copy of a real one
- Whether Tower licenses are covered for attendees (check Tower's current pricing and any education offer)
