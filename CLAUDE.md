# CLAUDE.md — instructions for working in this repository

This is a team project for Urban Innovation (LAW 8925), UMKC School of Law, Fall 2026.
Team: Anthony Ross, Camron Zerr, Mandy Lawson, Kirby Garrett. Advisor: Prof. Evan Absher.

The site gives Kansas City business owners information about employee ownership as a
succession option, plus a structured intake that gives them a read on whether their company
is a plausible fit and what problems it would face.

Four people work in this repo. Follow these rules without being asked.

## Assume no prior experience

Nobody on this team except Anthony has used version control, and most are not programmers.

- Never ask them to run a command, open a terminal, or visit a website to finish a step.
- Avoid the words commit, branch, merge, repository, and pull request unless they use those
  words first. Say "saved", "your copy", "put it live", "the project", "ready for the team".
- If something technical goes wrong, fix it. Tell them what happened in one plain sentence
  and what you did about it. Do not hand them a choice they have no basis to make.
- The exceptions, where you always stop and ask: anything that could lose work, and anything
  that publishes content to the live site.

## Nobody should ever duplicate someone else's work

This is the failure this project is most exposed to. Work in progress lives on a person's
own copy, where the rest of the team cannot see it. Without deliberate effort, two people
can spend a week on the same page and not find out until their versions collide.

`TASKS.md` is the only thing standing between the team and that outcome. Treat it as shared
state, not as a document.

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

**When they finish, or stop for the day:** update the item's status and push that to `main`,
even if the content itself is not ready to go live. Half-finished is useful information;
silence is not.

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
`mandy`. This is your business to track, not theirs. Do not ask them which branch they are
on or expect them to know.

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
