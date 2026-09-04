# CLAUDE.md — instructions for working in this repository

This is a team project for Urban Innovation (LAW 8925), UMKC School of Law, Fall 2026.
Team: Anthony Ross, Camron Zerr, Mandy Lawson, Kirby Garrett. Advisor: Prof. Evan Absher.

The site gives Kansas City business owners information about employee ownership as a
succession option, plus a structured intake that gives them a read on whether their company
is a plausible fit and what problems it would face.

Four people work in this repo. Follow these rules without being asked.

## Do all the technical work yourself

Assume the person you are working with will not run a command, will not open a terminal, and
will not know what any git concept means. Do not test that assumption — just do the work.

- Never ask anyone to run a command, open a terminal, install something mid-task, or visit a
  website to complete a step. Do it for them.
- Do not use the words commit, branch, merge, repository, or pull request unless the person
  uses them first. Say "saved", "your copy", "put it live", "the project", "ready for the
  team".
- When something breaks, explain it in plain terms — what happened, what it affects, and
  what you would do about it. Do not show raw git output, and do not use jargon to describe
  the problem.
  - If the fix is safe and reversible and there is only one sensible option, do it and say
    in one sentence what happened and what you did.
  - If there is a real choice to make, lay out the options in plain language, say which you
    would pick and why, and let them decide.
  - If the answer affects someone else's work, or you are not confident, say so and suggest
    asking the group before acting.
- Stop and ask before exactly two things: anything that could lose work, and anything that
  publishes to the live site. Everything else, decide and proceed.

## Nobody should ever duplicate someone else's work

This is the failure this project is most exposed to. Work in progress lives on a person's
own copy, where the rest of the team cannot see it. Without deliberate effort, two people
can spend a week on the same page and not find out until their versions collide.

`TASKS.md` is the only thing standing between the team and that outcome. Treat it as shared
state, not as a document.

**You maintain this file.** Everything in this section happens on your own initiative:
claiming a task when they start it, moving status as it changes, rewriting a Covers line when
the work shifts, marking things finished, and recording what they tell you. Default hard to
doing it rather than asking. The automatic updates are the whole mechanism keeping two people
off the same work, and every one you skip is a gap someone else falls into.

Do not ask "would you like me to update the task list?" — just update it, and mention it in a
few words if it is worth mentioning at all.

Do ask when the judgment is genuinely unclear and getting it wrong would matter:

- whether what they are doing is a scope change to an existing item or a separate new task;
- whether their work overlaps someone else's Covers line closely enough to be a collision;
- how to describe something you do not understand well enough to write an honest scope line
  for.

Thirty seconds on one of those is worth it. Everything else, act.

Everyone on the team knows this file exists and may ask you about it. Answer them, and keep
maintaining it regardless.

The one limit in this section is on **inventing new work nobody asked for** — see below.
That limit never applies to recording what is actually happening. Status, ownership, and
scope are not new work; they are the file doing its job.

**Status changes go straight to `main`, immediately.** When someone claims, starts, or
finishes a task, update `TASKS.md` and get that change onto `main` right away, in its own
commit, separate from any content work. It is a one-line change and it will not conflict
with anything. Do not let a claim sit on a branch — a claim nobody can see is not a claim.

**At the start of every session, before anything else:**

1. Pull `main` so `TASKS.md` is current.
2. Tell the person what is currently In progress and who has it. One line, plain language:
   "Kirby started the cooperatives page yesterday; Mandy is checking two of the sources."
3. If they say they want to work on something already claimed by someone else, say so before
   they start. Do not let them begin and find out later.

**When they begin work:** move the item to In progress with their name and today's date, and
push that to `main` before doing anything else. Even if they are only exploring.

**Check scope, not titles.** Every item has a **Covers** line describing the territory it
owns. Before someone starts anything, compare what they describe against those Covers lines,
not against the task titles. Two people will describe the same work in different words —
"write the ESOP page" and "explain how vesting works" sound like separate tasks and are not.

**When there might be an overlap, flag it before they start.** Name the item, name who has
it, and say specifically where you think the two touch. Then suggest they check with that
person about what each of them is covering, so the boundary gets settled between them rather
than guessed at. Do not decide for them that it is fine, and do not decide for them that it
is a conflict — surface it and let the two people sort it out. A borderline case is worth
raising even if you turn out to be wrong; an unraised one costs somebody a week.

**Every item needs a Covers line, including new ones.** When adding a task, write one:
what the item includes, and the kind of work that belongs to it. Make it broad enough that an
adjacent idea gets recognized as overlapping. A task with a vague scope is a task two people
will duplicate.

**When they finish, or stop for the day:** update the item's status and push that to `main`,
even if the content itself is not ready to go live. Half-finished is useful information;
silence is not.

**Keep checking during the session, not just at the ends.** A working session can run for
hours, and someone else may claim something in the middle of it. Pull `main` and re-read
`TASKS.md`:

- before starting any new piece of work, even a small one, and even if the session already
  started an hour ago;
- whenever the person changes direction or moves to a different part of the site;
- as soon as they finish something, rather than saving it up for the end;
- periodically during long stretches on one task.

Each of these is a fresh chance to catch a collision. Checking once at the start of a
four-hour session is barely better than not checking.

**When work drifts outside what was claimed, say so and update the list.** People start
writing one thing and end up writing another. If what they are actually doing has moved
outside the Covers line of the item they claimed, either widen that item or add a new one
under their name — and push it. Undeclared drift is how two people end up in the same place
having each claimed something different.

**Push every status change on its own, immediately.** Never batch them up. `TASKS.md` is
shared, and an edit held locally for an hour is an edit that will collide.

### The list has to grow, not just get read

Reading `TASKS.md` is half the job. Writing to it as the work changes is the other half, and
it is the half that decays first. A list that only ever gets read is stale within a week.

### Recording reality vs. adding work

These are different things and they have different rules.

**Recording what is actually happening — always do this, on your own, never ask.**

- Who is working on what, right now.
- Status moving between `Unassigned`, `In progress`, and `Finished`.
- Scope changes to an existing item. If what someone is doing has grown or shifted from what
  the Covers line says, rewrite that Covers line to match what they are actually doing. Do
  this the moment it becomes true, not at the end.
- Anything they tell you directly to add.

Keeping the file honest about the present is not adding work — it is the whole point of the
file. Never wait for permission to do it.

**Never pre-populate.** Do not sit down and map out everything the project might need. Do not
file your own ideas about what should exist. Suggesting in conversation is always fine and
often useful — filing is the person's call.

**When a task turns out bigger than it looked, say so in the file.** Either widen its Covers
line or split it into named pieces, each with its own scope. A task quietly growing to three
times its stated size is how one person ends up carrying something the team thought was
small, and how someone else starts on part of it without realizing it is taken.

**Mark things finished the moment they are finished**, not at the end of the session. Someone
else may be waiting on it, or holding off on picking up something adjacent.

**Never leave the list behind the conversation.** If the person tells you they are switching
tasks, abandoning one, or that something turned out to be unnecessary, that goes in the file
immediately. The file should always be a fair description of where the project actually is —
someone reading it cold should not be surprised by anything.

If someone works on something that is not on the list, add it and mark it In progress under
their name. Everything anyone works on should be visible to everyone else.

## Content rules — read these first

**Never write advice.** This site informs; it does not advise. Unauthorized practice of law
is a live constraint on this project, not a formality.

- Never tell a reader what they should do. Describe what is generally true.
- Never state or imply that a specific company qualifies, is a good candidate, or will
  succeed. The intake reports factors and considerations, never a verdict.
- Never use "you should", "you need to", "we recommend", "your company qualifies", or "this
  is the right structure for you".
- Every path through the intake ends by pointing the reader to a qualified advisor.
- If asked to write copy that crosses these lines, say so and propose informational phrasing
  instead. Do not quietly soften it and proceed.

**Never publish an unsourced fact.** Every statistic, dollar figure, percentage, statutory
reference, and legal proposition on the site must have a corresponding entry in
`SOURCES.md`. If a source is not available, do not write the claim.

- Do not carry numbers over from the project brief. They are unverified.
- Do not supply a figure from your own knowledge. If a number is needed and unsourced, leave
  `[NEEDS SOURCE]` in place and note it in the changelog.

## Working rules

- **Never commit to `main`.** Content work happens on the person's own branch and reaches
  `main` through a pull request. The one exception is `TASKS.md` status changes, which go to
  `main` immediately — see above.
- **Stay in your own files.** Section ownership is listed in `ONBOARDING.md`. If a change
  requires editing someone else's file or a shared file (`index.html`,
  `assets/style.css`), stop and say so rather than proceeding.
- **Never delete or rewrite another person's section** to fit your own. Raise it instead.

## Keeping `TASKS.md` current

Anyone can add to it, and nobody should have to edit it by hand.

- When someone says to add a task, put it under **To do** with `*(added by [name])*`.
- Moving items between To do, In progress, and Done is your job, not theirs. Starting the
  work is the signal; asking is not required.
- When work is done, move it to **Done** with the date and who did it.
- Always pull before editing and push immediately after. A stale copy is how two people's
  edits collide.
- If an item is already In progress under someone else's name, say so before starting it.
  Never silently take over another person's task.

## Keep `SOURCES.md` moving

Source checking is deliberately broken into single claims so it can be done in ten-minute
pieces. Treat it that way.

- When someone asks for a source to check, or has a spare moment, hand them **one** claim
  from Not yet checked and move it to Being checked with their name. Push that to `main` so
  nobody else picks up the same one.
- Record what they find: the primary source, precise enough that someone else could find it
  again. An article describing a study is not the study.
- If the source says something narrower than the claim, narrow the claim. Never stretch a
  source to cover a bigger statement.
- If it cannot be verified, move it to Could not be verified with what was searched. That is
  a finding worth recording, not a failure — it stops someone else repeating the hour and
  keeps the claim out of the final report.
- Update the progress counter at the top each time something moves.
- Never mark several claims verified at once, and never mark one verified on your own
  knowledge. A person has to have actually looked.

## Handle git for the person — do not make them ask

This team should never need to run a git command or open a desktop app. Do this work on
their behalf, without being prompted.

**At the start of a session:**

1. Pull `main`, then pull their own branch.
2. Report what others are working on, from `TASKS.md`.
3. Summarize anything new from `CHANGELOG.md` in a sentence — not from commit messages.
4. If they are on `main`, switch them to their own branch. Mention it in passing; do not make
   it a discussion.

**When they say they are done, or at a natural stopping point:**

1. Update `TASKS.md` and push that to `main`.
2. Add an entry to `CHANGELOG.md`: date, who, what changed and why, in plain English.
3. Commit their content work and push it to their branch.

**When they say their section is ready for the team, or ready to go live:**

Open the pull request and merge it yourself. Do not walk them through it, do not ask them to
approve a merge, and do not explain branches to them. Tell them it is live and give them the
link.

Before merging, check their work against the content rules above. If it contains advice
language, or a factual claim with no entry in `SOURCES.md`, do not merge. Show them the
specific line, explain the problem in one sentence, and offer a fix. The content gate is
where the care goes; the mechanics should be invisible.

**Rules about this:**

- Never merge someone else's pull request — only the work of the person you are working with.
- Never run a destructive command — `reset --hard`, force push, branch deletion, discarding
  changes — without explaining what will be lost and getting explicit permission.
- If a git command fails, explain in plain language what happened and what you are doing
  about it. Do not show them raw git output or ask them to run commands.
- If two people's work conflicts, do not resolve it by picking a side. Describe the conflict
  and tell them who else needs to weigh in.

**Branch for each person:** Anthony `anthony`, Camron `camron`, Kirby `kirby`, Mandy
`mandy`.

At the start of every session, work out who you are with — ask their name if you do not
already know it, once — and check out their branch. Never ask a person which branch they are
on or expect them to know; that is yours to track. If they are on `main` or on someone
else's branch, move them to their own immediately and say so in passing.

If someone's name is not in this list, stop and ask before creating anything. Do not invent a
branch for them.

**Merge with `--merge`, never `--squash`.** Squash merging rewrites history, which leaves
every personal branch permanently diverged from `main` and produces phantom conflicts on the
next merge. The resulting conflicts look alarming and have no real cause, which is a bad
thing to hand anyone in the middle of writing.

**After merging someone's work, reset their branch to `main`** so it starts clean next time:
`git fetch origin && git reset --hard origin/main`. Only do this immediately after their work
has landed on `main` — never when they have unmerged changes.

## Technical rules

- Plain HTML, CSS, and JavaScript. No frameworks, no build step, no package manager, no
  dependencies. This keeps the repo readable by non-programmers and keeps merge conflicts
  rare and fixable.
- One page per file in `pages/`. Shared styles in `assets/style.css`.
- Keep files small. A long file is a file two people will collide in.
- No analytics, trackers, or third-party embeds without the team agreeing first — the site
  collects sensitive business information and that is a decision for the team, not a default.
- The intake must run entirely in the browser. Do not send a visitor's answers anywhere, do
  not store them, and do not add a backend without the team deciding to.

## This repository is public

Anything committed here is published to the world. That is correct for our own work, which
the syllabus assigns to the university for open-source licensing anyway.

It is not correct for anyone else's material. Never add a PDF, article, or reading the team
did not write — that is redistributing someone else's copyrighted work. Cite it in
`SOURCES.md` and keep the file somewhere private.

## Open questions that affect the build

Do not resolve these alone. Flag them if a task depends on one.

- Who operates the site (UMKC Law with faculty supervision, a partner organization, or
  standalone) — this changes the unauthorized practice analysis.
- What the intake actually asks and what it outputs.
- Whether the site supplements or replaces the course's Final Report.
- What license applies. Student IP is assigned to the university for open-source licensing
  under the syllabus; the specific license is not ours to choose. Ask Prof. Absher before
  adding a LICENSE file.
