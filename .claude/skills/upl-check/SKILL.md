---
name: upl-check
description: Review site copy, an intake question, a result screen, a disclaimer, or marketing text for unauthorized-practice-of-law risk, using the team's research in notes/. Use when someone asks "is this advice?", "check this for UPL", or wants a page, question, or result reviewed before it goes to the team.
---

# UPL check

This is a closer read than the content rules in `CLAUDE.md`, and it follows those rules.
Run it on draft pages, intake questions, result text, disclaimers, and anything describing
what the tool does.

## Before starting, read the research

Read these each time, because they change:

- `notes/upl-research.md`: where the line is under Missouri law
- `notes/tool-design-guidance.md`: how comparable tools stay on the right side of it
- `notes/regulatory-landscape.md`: only if the question is about changing the rules

**Nothing in those notes has been verified by a person yet.** Every authority named below is
a lead. This check can point out risk. It cannot clear anything.

## The tests

Apply each test to every sentence, question, and answer option. The authority named with each
test is the one in the notes. Cite it from the notes, never from memory. If a concern is not
covered by the notes, say it falls outside the team's research. Do not supply the law
yourself.

1. **Should / whether.** Does the sentence answer who, what, when, where, or how, or does it
   answer should or whether? The second kind is advice. *(Indiana and Missouri court staff
   guidance)*
2. **Category or this reader.** Does it describe what is generally true of a kind of company,
   or does it evaluate the reader's company? Explaining what an ESOP requires is information.
   Evaluating whether this company can do one is advice. *(LSC AO-2017-004; Thompson;
   Mid-America)*
3. **Verdict strength.** Check against the verb ladder in the tool-design note. Nothing may
   go past "likely eligible." Also flag every phrase `CLAUDE.md` bans: "you should," "you need
   to," "we recommend," "your company qualifies," "the right structure for you."
4. **Choosing forms or structures.** Does it pick which document, structure, or path this
   reader should use, or produce a completed document for them? *(Janson; Hulse; Mid-America;
   the Upsolve terms language on "selection of forms")*
5. **Compliance or consequences.** Does it tell the reader something will comply, will be
   safe, or will not trigger a tax, ERISA, or other consequence? *(Lucas Subway)*
6. **A ranked short list.** Does it show some options and not others, or rank them? Showing all
   options is safer. *(Texas OCA guidelines)*
7. **Promises in the marketing copy.** Does anything say the tool figures things out or takes
   over for the reader? *(the LegalZoom homepage language quoted in Janson)*
8. **People in the loop.** Would anyone on the team read a visitor's answers and respond to
   them? That changes the whole analysis, so flag it as a design problem, not a wording
   problem. *(Janson)*
9. **Money.** Is there a fee, a bundled charge, or referral compensation anywhere? Being free
   removes the damages exposure, not the UPL exposure. *(§ 484.010.2; Hulse; Eisel)*
10. **Intake design.** Asking questions is fine *(Mid-America)*. Flag open free-text boxes,
    exact financials where a range would do, any storage of answers, and any missing statement
    that submissions are not confidential. *(tool-design note, data handling; Mo. Informal
    Op. 20000103)*
11. **Disclaimer placement.** Is it on every page, acknowledged before the intake, and shown
    alongside the result? Also flag any wording that treats the acknowledgment as a cure. It
    is not one. *(Eisel; Carpenter)*
12. **Tone.** Second-person, warm, persona-style writing works against the disclaimer.
    *(Utah Op. 96-12)*

## Report

For each flagged passage:

- Quote the line.
- Name the test and the authority, with the section of the note it comes from.
- Explain the problem in one plain sentence.
- Propose informational wording for the line.

Then list every authority the flags relied on, so someone can check them with
`verify-source`.

**Never** say copy is "compliant," "safe," "cleared," or "fine." If nothing was flagged, say:
*"Nothing flagged against the tests in the team's research notes. This is not a legal opinion,
and the research behind these tests has not been verified yet."*

Do not change the file unless asked. `CLAUDE.md` says to propose informational wording, not to
quietly soften copy and move on.

## Do not settle these

If the answer depends on one of these, say so and leave it to the team:

- Who operates the site (UMKC Law with faculty supervision, a partner organization, or
  standalone)
- What the intake asks and what it outputs
- Broad liability disclaimers (the Michigan and Illinois approach) versus none (North
  Carolina's safe harbor). The tool-design note says this is a question for UMKC's risk
  office.
