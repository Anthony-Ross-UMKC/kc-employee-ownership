# CLAUDE.md — instructions for working in this repository

This is a team project for Urban Innovation (LAW 8925), UMKC School of Law, Fall 2026.
Team: Anthony Ross, Camron Zerr, Mandy Lawson, Kirby Garrett. Advisor: Prof. Evan Absher.

The site gives Kansas City business owners information about employee ownership as a
succession option, plus a structured intake that gives them a read on whether their company
is a plausible fit and what problems it would face.

Four people work in this repo. Follow these rules without being asked.

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

- **Never commit to `main`.** Work on your own branch. Merge to `main` through a pull
  request.
- **Pull before you start.** `git pull origin main` at the beginning of every session.
- **Stay in your own files.** Section ownership is listed in `ONBOARDING.md`. If a change
  requires editing someone else's file or a shared file (`index.html`,
  `assets/style.css`), stop and say so rather than proceeding.
- **Never delete or rewrite another person's section** to fit your own. Raise it instead.
- **Update `CHANGELOG.md` at the end of every working session.** Plain English, what changed
  and why, so teammates do not have to read commit history. This is required, not optional.

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

## Open questions that affect the build

Do not resolve these alone. Flag them if a task depends on one.

- Who operates the site (UMKC Law with faculty supervision, a partner organization, or
  standalone) — this changes the unauthorized practice analysis.
- What the intake actually asks and what it outputs.
- Whether the site supplements or replaces the course's Final Report.
- What license applies. Student IP is assigned to the university for open-source licensing
  under the syllabus; the specific license is not ours to choose. Ask Prof. Absher before
  adding a LICENSE file.
