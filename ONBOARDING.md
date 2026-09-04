# Getting started

For Camron, Kirby, and Mandy. Fifteen minutes, and you do not need to know how to code.

## What this is

A shared copy of the website we are building. Everyone works on their own copy, then merges
changes into the main one. Nothing you do can break the live site, and nothing gets
overwritten.

## One-time setup

The setup is the only fiddly part. Once you are through it, you never touch it again.

1. Make a free account at **github.com** if you do not have one, and send Anthony your
   username so he can add you.
2. Accept the email invitation to the repository.
3. Install **Git** from git-scm.com. Accept every default. You will never type a git
   command — Claude needs it installed to do the work for you.
4. Install **Claude Code**, open it, and tell it:
   *"Clone https://github.com/Anthony-Ross-UMKC/kc-employee-ownership and set me up on the
   [your name] branch."*
5. The first time it uploads anything, a browser window will ask you to sign in to GitHub.
   Sign in with the account from step 1 — **not** any other GitHub account you may have.

If any of that fights you, stop and ask Anthony rather than clicking through. Sorting it out
takes five minutes with someone else looking; it takes an hour alone.

## Every time you work

Open Claude Code in the project folder and say what you want to work on. That is the whole
process. It reads the project rules automatically and handles the rest — getting the latest
version before you start, saving and uploading your work when you finish, and putting your
section forward for the team when it is ready.

Things you can just say:

- *"What's changed since I last worked on this?"*
- *"I want to add a section on vesting to my page."*
- *"Is this wording okay, or does it sound like legal advice?"*
- *"I'm done for today."*
- *"My section is ready for the team."*

You never need to run a command or use the GitHub website. If you would like to see your
changes visually, **GitHub Desktop** (desktop.github.com) shows them side by side — but it
is optional and nothing requires it.

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
