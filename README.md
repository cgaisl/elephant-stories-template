# Graded-reader story repo — template

Template for a personal, AI-tutored graded-reader story repo (built for
Thai), read through the companion web reader at
<https://cgaisl.github.io/elephant-stories/>
([source](https://github.com/cgaisl/elephant-stories)).

Your copy holds *your* stories, *your* vocabulary ledger, and *your* learner
profile, and writes new stories on demand with a GitHub Action running on
your own Claude subscription. Nothing is shared.

## Get started

1. Click **Use this template → Create a new repository**, and make your copy
   **private** (your reading level and profile live in it).
2. Follow [`SETUP.md`](SETUP.md) — two tokens and the Claude GitHub App,
   ~10 minutes, one time.
3. Open the reader, point it at your repo, and open your first issue: tell
   the tutor your level and situation, and it sets up your learner profile
   and writes story ๑.

## What's inside

| File | Role |
|---|---|
| `CLAUDE.md` | the tutoring method — static; automation may never edit it (a CI guard reverts violations) |
| `PROFILE.md` | who you are as a learner: level, calibration, story-world cast, progression, durable preferences |
| `VOCABULARY.md` | the ledger of every word you know — the single source of truth that keeps stories ~90%+ comprehensible |
| `stories/` | your reading history, one markdown file per story |
| `.github/workflows/claude-story.yml` | turns a "new story" issue into a story and replies with teaching notes |

Requests in plain language work: "beach theme", "zero new words today",
"harder", or from-now-on preferences ("~20 new words per story from now
on"), which get recorded in your profile.
