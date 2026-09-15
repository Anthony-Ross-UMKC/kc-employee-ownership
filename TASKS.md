# Team task list

This is how we know who is doing what. It is the only place work in progress is visible to
everyone else — while you are writing, your changes stay private to your copy until you say
your section is ready.

**Anyone can add anything.** This is not a list of assignments. If you think something should
exist, put it here — that is how the rest of us find out you think so.

You do not maintain it by hand. Tell Claude what you are picking up or what you think we
should do, and it records it. It also keeps an eye on this file throughout your session, so
if someone else claims something while you are working, you hear about it then rather than a
week later.

Ask *"what's everyone working on?"* any time.

**Every item has a "Covers" line** saying what territory it owns, so work that *sounds*
different but *is* the same gets caught before two people spend a week on it. Read the Covers
lines, not the titles.

Status is `Unassigned`, `In progress`, or `Finished`.

---

## In progress

### Sean Power, Polsinelli — call done, follow-ups open
`In progress` · Anthony
**Covers:** the call with Polsinelli's ESOP practice group and everything that came out of it.
Held Friday September 11. Notes are in `notes/polsinelli-call-notes.md`. Still to
collect: the due diligence checklist and ESOP 101 deck he offered to send. Still open: thank-you email,
collecting the due diligence checklist and ESOP 101 deck he offered, and asking Absher what he
and Sean discussed about cash at closing.

### Where the unauthorized practice line is
`In progress` · Anthony, September 9 — citations checked against source text; needs review by a person
**Covers:** how far the intake can go before it becomes legal advice, and what that means for
the wording of every result. Missouri authority — Mo. Rev. Stat. 484.010 and 484.020, Janson
v. LegalZoom (W.D. Mo.) — plus how comparable public legal-information tools are structured.
Anything about UPL, disclaimers, or advice-versus-information belongs here. Findings are in
`notes/upl-research.md` (the legal analysis), `notes/tool-design-guidance.md` (what comparable
tools actually do), and `notes/regulatory-landscape.md` (whether the rules could be changed).
**The citations in `notes/upl-research.md` were checked against the source text on September
15.** Quotes and holdings match. The one error found, the *McKeage* fee figures, has been
corrected. A person still needs to review the citations before anything is published or
presented. Not yet checked: most pinpoint pages, the *Janson* settlement dates, Rules 13 and
5.30, and every citation in the other two files.

---

## Unassigned

*Nothing yet — add what you think we should be doing.*

---

## Finished

### What makes a company a good ESOP candidate
**Covers:** the criteria that decide whether a company is a plausible ESOP candidate: financial
(profitability, EBITDA, debt capacity, covered payroll), organizational (a finance function, an HR
function, management depth), owner objectives (fair price and legacy versus maximum cash, willingness
to carry a seller note), and structural choices (1042 or not, seller or bank financing, partial or
full sale). Also covers disqualifiers, the compliance and carry-cost thresholds that rule small
companies out, where companies most often fall short on preparation, and what existing screening and
intake tools already ask. Also covers how ESOPs fail and which warning signs are visible before a deal,
the case critics make against ESOPs, what lenders and trustees require, deal data for the $5–20M
range, and the tax, ERISA, and SBA rules that bear on fit (§ 1042, § 409(p), contribution and
deduction limits, SBA 7(a) loans to ESOPs). This is the foundation for the tool being built for Prof.
Absher's fund, and it applies to both the owner-facing and practitioner-facing sides.
*Anthony, September 15. Memo: `notes/esop-candidate-research.md`. A second round of research the same
day (research papers, critics, failure cases, lenders and the $5–20M market, primary legal sources)
found errors in six legal points in that memo: Herman, Cunningham v. Cornell, § 1042, § 409(p), the
payroll limit, and SBA's citizenship rule. The memo in `notes/` has not been corrected yet, so don't
rely on those points.*

### Source-checking and advice-review instructions for Claude
**Covers:** the two checks Claude runs when someone asks for a source to check
(`verify-source`) or asks whether wording reads as legal advice (`upl-check`). They live in
`.claude/skills/`. Any change to how either check works belongs here.
*Anthony, September 12.*

### Set up the project so all four of us can work on it at once
**Covers:** the repository, working rules, onboarding guide, and shared task and source
tracking.
*Anthony, September 4.*
