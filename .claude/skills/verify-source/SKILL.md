---
name: verify-source
description: Check one factual claim against its primary source and record the result in SOURCES.md. Use when someone says "give me a source to check", asks to verify a figure, statistic, statute, or case, or wants to use a fact on the site that has no SOURCES.md entry yet.
---

# Verify one source

This skill carries out the `SOURCES.md` rules in `CLAUDE.md`. Where the two differ,
`CLAUDE.md` wins. Use plain language throughout: the person you are helping may never have
done source checking before.

**Your job is to find the source and set it up so checking is quick. Deciding it is verified is
the person's job.** `CLAUDE.md` says a person has to have actually looked. What you retrieve
does not count as a person looking.

## 1. Pick one claim

- If they named a claim, use that one. If it is not already in `SOURCES.md`, add it under
  **Not yet checked** with where it came from.
- If they asked for "a source to check," give them the first unclaimed row under **Not yet
  checked**.
- Move it to **Being checked** with their name and today's date, and update the progress
  counter. Get that change live right away, as `CLAUDE.md` describes, so nobody else picks up
  the same claim.

Work on one claim at a time. Never several.

## 2. Find the primary source

A primary source is the thing itself. An article that describes it does not count.

| Kind of claim | Primary source |
|---|---|
| Federal statute | The U.S. Code section (uscode.house.gov or law.cornell.edu) |
| Missouri statute | revisor.mo.gov |
| Court decision | The opinion. Use CourtListener if it is connected, otherwise courtlistener.com. |
| Federal regulation or rulemaking agenda | eCFR, the Federal Register, or the Unified Agenda at reginfo.gov |
| Figure from a study or survey | The study itself, plus its year and sample |
| Organization's own figure (NCEO, MOCEO) | That organization's page or report where the figure appears |

When you find a secondary source, follow it back. For example, the brief cites NCEO, and NCEO
cites a specific study. Record the chain, because it shows where to look next even if you
never reach the end.

Do not fill a gap from your own knowledge. If you cannot find the source, that is a finding.

## 3. Show the person what you found

Give them:

- **The source:** title, publisher or court, date, and a link or full citation, precise
  enough that someone else could find it again.
- **The passage:** a short excerpt of the exact sentence or table row that supports the
  claim, and where in the source it appears.
- **How well it matches.** Say which of these applies:
  - It matches the claim.
  - It is narrower. Propose narrowed wording for the claim.
  - It is older than the claim implies. Give the date.
  - It says something different.
  - Only a secondary source was found.

Then ask them to open the link and read the passage themselves. **Do not move the claim to
Verified until they say they have.**

## 4. Record the outcome

**Verified** (only after they confirm they read it): move the row to **Verified** with the
source, their name, and the date. If the claim was narrowed, record the narrowed wording, not
the original.

**Could not be verified:** move it to **Could not be verified** with what was searched, their
name, and the date. Tell them this counts as progress: it saves the next person an hour and
keeps the claim out of the final report.

**Not finished:** leave it under **Being checked** and write down the chain found so far, so
the next session can pick up where this one stopped.

Update the progress counter every time a claim moves.

## Never

- Mark a claim verified from your own knowledge, or from a source nobody has opened.
- Treat an article, press release, or blog post as the source of the figure it reports.
- Stretch a source to cover a broader claim than it supports.
- Mark more than one claim at a time.
- Put someone else's PDF or article in the project. Cite it and leave the file elsewhere.
