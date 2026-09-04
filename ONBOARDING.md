# Getting started

For Camron, Kirby, and Mandy. Fifteen minutes, and you do not need to know how to code.

## What this is

A shared copy of the website we are building. Everyone works on their own copy, then merges
changes into the main one. Nothing you do can break the live site, and nothing gets
overwritten.

## One-time setup

1. Make a free account at **github.com** if you do not have one, and send Anthony your
   username so he can add you.
2. Accept the email invitation to the repository.
3. Install **GitHub Desktop** (desktop.github.com) — this is the version without the command
   line. Sign in, then File → Clone Repository → pick this one.
4. Install **Claude Code** and point it at the folder GitHub Desktop created.

## Every time you work

1. In GitHub Desktop, click **Fetch origin**, then **Pull** if there is anything to pull.
2. Make sure you are on **your own branch**, not `main`. The branch selector is at the top.
3. Do your work. Claude Code reads `CLAUDE.md` in this folder automatically and follows the
   project rules.
4. In GitHub Desktop, write a one-line summary and click **Commit**, then **Push origin**.
5. Click **Create Pull Request** when a section is ready for the team.

## Section ownership

To keep everyone out of each other's way, each of us owns specific files. Confirm these
before starting — they are a proposal, not settled.

| Person  | Branch    | Files                                    |
| ------- | --------- | ---------------------------------------- |
| Anthony | `anthony` | `pages/intake.html`, `assets/intake.js`  |
| Camron  | `camron`  | `pages/esop.html`                        |
| Kirby   | `kirby`   | `pages/eot-and-co-ops.html`              |
| Mandy   | `mandy`   | `pages/resources.html`                   |

`index.html` and `assets/style.css` are shared. Say something in the team chat before
editing either, so two people are not in them at once.

## Two rules that matter more than the rest

**Nothing on this site tells a reader what to do.** We inform; we do not advise.
Unauthorized practice of law is a real constraint on this project. If something you write
starts sounding like advice to a specific business, flag it.

**Every fact needs a source.** Every number, dollar figure, and legal statement has to have
an entry in `SOURCES.md`. Do not reuse the figures from the project brief — they have not
been verified. If you cannot source it, leave `[NEEDS SOURCE]` and note it in the changelog.

## If something goes wrong

Do not try to fix it by deleting things. Push what you have to your own branch and tell
Anthony. Nothing is ever lost — that is the point of the repository.
