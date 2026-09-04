# CLAUDE.md — instructions for working in this repository

Team project for Urban Innovation (LAW 8925), UMKC School of Law, Fall 2026.
Anthony Ross, Camron Zerr, Mandy Lawson, Kirby Garrett. Advisor: Prof. Evan Absher.

The site gives Kansas City business owners information about employee ownership as a
succession option, plus a structured intake that gives them a read on whether their company
is a plausible fit and what problems it would face.

Follow these rules without being asked.

## Working with people here

Assume the person will not run a command, will not open a terminal, and will not know what
any git concept means. Do not test that assumption — just do the work.

- Never ask anyone to run a command, open a terminal, install something mid-task, or visit a
  website to complete a step. Do it for them.
- Do not use the words commit, branch, merge, repository, or pull request unless they use
  those words first. Say "saved", "your copy", "put it live", "the project", "ready for the
  team".
- Stop and ask before exactly two things: anything that could lose work, and anything that
  publishes to the live site. Everything else, decide and proceed.

**When something breaks**, explain it in plain terms — what happened, what it affects, what
you would do. Never show raw git output.

- Safe, reversible, one sensible option: do it, then say in one sentence what happened.
- A real choice to make: lay out the options plainly, say which you would pick and why, let
  them decide.
- Affects someone else's work, or you are not confident: say so and suggest asking the group
  before acting.

## `TASKS.md` — the anti-duplication mechanism

Work in progress lives on a person's own branch where nobody else can see it. `TASKS.md` is
the only thing preventing two people spending a week on the same page. Treat it as shared
state.

**You maintain it, on your own initiative.** Claiming a task when they start, moving status,
rewriting a Covers line when work shifts, marking things finished, recording what they tell
you. Never ask "would you like me to update the task list?" — update it, and mention it in a
few words if worth mentioning.

**Do ask** when getting it wrong would matter: whether something is a scope change or a
separate task; whether work overlaps someone else's Covers line closely enough to collide;
how to describe work you do not understand well enough to scope honestly.

**Status changes go straight to `main`, immediately**, in their own commit, separate from
content work. A claim sitting on a branch is a claim nobody can see. Never batch them.

### Every session

1. Pull `main` so `TASKS.md` is current.
2. Tell them what is In progress and who has it, in one plain line.
3. If they want something already claimed, say so before they start.

**Keep re-checking during the session** — before any new piece of work even an hour in,
whenever they change direction, as soon as they finish something, and periodically during
long stretches. Someone may claim something mid-session.

### Claiming and scope

**When they begin work:** move the item to In progress with their name and today's date, and
push to `main` before doing anything else. Even if they are only exploring. If what they are
doing is not on the list, add it and mark it In progress under their name.

**Check scope, not titles.** Every item has a **Covers** line describing the territory it
owns. Compare what they describe against those, not against titles — "write the ESOP page"
and "explain how vesting works" sound like separate tasks and are not.

**When there might be an overlap, flag it before they start.** Name the item, name who has
it, say specifically where the two touch. Suggest they check with that person about what each
is covering, so the boundary gets settled between them. Do not decide either way yourself. A
borderline case is worth raising even if you turn out to be wrong; an unraised one costs
somebody a week.

**Every item needs a Covers line**, broad enough that an adjacent idea gets recognized as
overlapping. A vague scope is a task two people will duplicate.

**When work drifts outside what was claimed**, widen that item's Covers line or add a new one
under their name, and push. Undeclared drift is how two people end up in the same place
having each claimed something different.

**When a task turns out bigger than it looked**, widen its Covers line or split it into named
pieces with their own scopes.

**If an item is In progress under someone else's name**, say so before starting it. Never
silently take over another person's task.

### Recording vs. adding

**Always record, never ask first:** who is working on what, status moving between
`Unassigned` / `In progress` / `Finished`, scope changes to existing items, and anything they
tell you to add. This is not adding work — it is the file doing its job.

**Mark things finished the moment they are finished.** Someone may be waiting on it.

**Never leave the list behind the conversation.** Switching tasks, abandoning one, something
turning out unnecessary — that goes in the file immediately. Someone reading it cold should
not be surprised by anything.

**Never pre-populate.** Do not map out everything the project might need or file your own
ideas about what should exist. Suggesting in conversation is fine; filing is the person's
call. New items go under **Unassigned** with `*(added by [name])*`.

## Content rules

**Never write advice.** This site informs; it does not advise. Unauthorized practice of law
is a live constraint on this project, not a formality.

- Never tell a reader what they should do. Describe what is generally true.
- Never state or imply that a specific company qualifies, is a good candidate, or will
  succeed. The intake reports factors and considerations, never a verdict.
- Never use "you should", "you need to", "we recommend", "your company qualifies", or "this
  is the right structure for you".
- Every path through the intake ends by pointing the reader to a qualified advisor.
- If asked to write copy that crosses these lines, say so and propose informational phrasing.
  Do not quietly soften it and proceed.

**Never publish an unsourced fact.** Every statistic, dollar figure, percentage, statutory
reference, and legal proposition must have an entry in `SOURCES.md`. No entry, no claim.

- Do not carry numbers over from the project brief. They are unverified.
- Do not supply a figure from your own knowledge. Leave `[NEEDS SOURCE]` and say so.

## `SOURCES.md`

Source checking is broken into single claims so it can be done in ten-minute pieces.

- When someone asks for a source to check, hand them **one** claim from Not yet checked, move
  it to Being checked with their name, and push to `main` so nobody duplicates it.
- Record the primary source precisely enough that someone else could find it again. An
  article describing a study is not the study.
- If the source says something narrower than the claim, narrow the claim. Never stretch a
  source to cover a bigger statement.
- If it cannot be verified, move it to Could not be verified with what was searched. That is
  a finding, not a failure — it stops someone repeating the hour and keeps the claim out of
  the final report.
- Update the progress counter each time something moves.
- Never mark several claims verified at once, and never mark one verified from your own
  knowledge. A person has to have actually looked.

## Git — do it all for them

**Branches:** Anthony `anthony`, Camron `camron`, Kirby `kirby`, Mandy `mandy`.

At the start of every session, work out who you are with — ask their name once if you do not
know it — and check out their branch. Never ask which branch they are on; that is yours to
track. If they are on `main` or someone else's branch, move them and say so in passing. **If
a name is not in this list, stop and ask. Do not invent a branch.**

**Session start:** pull `main`, pull their branch, then say from `TASKS.md` what others are
working on and what finished since they last worked.

**When they stop:** update `TASKS.md` and push to `main`, then commit their work to their
branch. Commit messages are the only prose record — write them plainly.

**When they say a section is ready:** open the pull request and merge it yourself. Do not
walk them through it or ask them to approve a merge. Tell them it is live and give the link.

Before merging, check the work against the content rules above. If it contains advice
language or a factual claim with no `SOURCES.md` entry, do not merge — show the specific
line, explain the problem in one sentence, offer a fix. The content gate is where the care
goes; the mechanics should be invisible.

**Rules:**

- Never commit to `main`. The only exception is `TASKS.md` status changes.
- Stay in the person's own files. `index.html` and `assets/style.css` are shared — stop and
  say so rather than editing them unannounced. Never delete or rewrite another person's
  section.
- Never merge someone else's pull request — only the work of the person you are with.
- Never run a destructive command (`reset --hard`, force push, branch deletion, discarding
  changes) without explaining what will be lost and getting explicit permission.
- If two people's work conflicts, do not resolve it by picking a side. Describe the conflict
  and say who needs to weigh in.
- **Merge with `--merge`, never `--squash`.** Squashing rewrites history, leaving every
  personal branch permanently diverged from `main` and producing phantom conflicts that look
  alarming and have no real cause.
- **After someone's work lands on `main`, reset their branch to it**
  (`git fetch origin && git reset --hard origin/main`) so it starts clean. Only immediately
  after their work has landed — never when they have unmerged changes.

## Technical rules

- Plain HTML, CSS, and JavaScript. No frameworks, no build step, no package manager, no
  dependencies — this keeps the repo readable by non-programmers and merge conflicts rare.
- One page per file in `pages/`. Shared styles in `assets/style.css`. Keep files small; a
  long file is a file two people will collide in.
- The site has no fixed structure yet — what pages exist is the team's decision. When someone
  writes something new, create the page and add a link to it on the homepage. `index.html` is
  shared, so say so when you edit it.
- No analytics, trackers, or third-party embeds without the team agreeing first.
- The intake runs entirely in the browser. Do not send a visitor's answers anywhere, do not
  store them, and do not add a backend without the team deciding to.

## This repository is public

Everything committed here is published. That is correct for our own work, which the syllabus
assigns to the university for open-source licensing anyway.

It is not correct for anyone else's material. Never add a PDF, article, or reading the team
did not write — that is redistributing copyrighted work. Cite it in `SOURCES.md` and keep the
file elsewhere.

## Open questions — do not resolve these alone

Flag them if a task depends on one.

- Who operates the site (UMKC Law with faculty supervision, a partner organization, or
  standalone) — this changes the unauthorized practice analysis.
- What the intake asks and what it outputs.
- What license applies. Student IP is assigned to the university for open-source licensing;
  the choice is not ours. Ask Prof. Absher before adding a LICENSE file.
