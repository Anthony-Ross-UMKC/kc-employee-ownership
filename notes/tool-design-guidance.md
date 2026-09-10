# Design guidance — how comparable tools stay on the right side

Research findings, September 9, 2026. **Not independently verified by the team.**

This is the operational companion to `upl-research.md`. That file says where the line is; this
one says what other people actually do about it.

---

## The one-sentence test

Indiana's court self-help guidance is the sharpest operational rule found, and it transfers
directly to writing questions and output
([in.gov](https://www.in.gov/courts/selfservice/unrepresented/help/)):

> "Staff can answer questions that call for factual information — these are generally
> questions that start with 'who,' 'what,' 'when,' 'where,' or 'how.' They cannot answer
> questions that call for an opinion about what you should do — these are generally questions
> that start with 'should,' or 'whether.'"

Apply it to every sentence of output. *How does an ESOP get financed* is answerable. *Should
you do one* is not.

Missouri's own version, from the courts' Court Staff Assistance page
([courts.mo.gov](https://www.courts.mo.gov/page.jsp?id=3833)) — staff MAY "explain and answer
questions about how the court works" and "provide you with the number of the local lawyer
referral service"; staff MAY NOT "tell you whether or not you should bring your case to
court," "tell you what words to use," or "give you an opinion about what will happen in your
case."

## What the employee-ownership sector itself does

**It does not use disclaimers.** NCEO, Project Equity, and ESOP Partners were checked for
legal-advice disclaimers and none were found — the terms-of-use pages 404.

They avoid the problem structurally: they stay wholly inside **business feasibility** framing
and never characterize legal consequences. NCEO's
[ESOP Pre-Feasibility Toolkit](https://www.nceo.org/resource-toolkits/esop-pre-feasibility-toolkit)
is the closest domain analogue — organized around "Screening Questions" (big enough?
profitable enough? is top price your priority?) and stating plainly that it "does not replace
the need for an ESOP feasibility study, which may be an important next step."

That is probably more transferable than any disclaimer language. A tool that talks about
money, headcount and margins is on different ground from one that talks about what the law
requires.

## The de facto standard disclaimer formula

Three statewide navigators use near-identical wording. The shared core:

1. **Information is not advice**, with advice defined as *applying law to specific
   circumstances*.
2. **You are not authorized to rely on this.**
3. **No attorney-client relationship is created.**

[Michigan Legal Help](https://michiganlegalhelp.org/terms-of-use): "Legal information is not
the same as legal advice. Legal advice is the application of law to a person's specific
circumstances." … "You should not and are not authorized to rely on Michigan Legal Help
Content as a source of legal advice."

[Illinois Legal Aid Online](https://www.illinoislegalaid.org/terms-of-use) extends the
disclaimer expressly to the *interactive* features, including automated documents — worth
copying, since that is the part most at risk.

**[LawHelp Interactive](https://support.lawhelpinteractive.org/hc/en-us/articles/221936688-Can-you-please-summarize-the-legal-terms-in-plain-English-)
is the best model**, because it enumerates what the tool *cannot* do rather than only what it
is not:

> "Because this website is not a lawyer, it cannot: Give you advice, opinions, or
> recommendations about your rights or your case • Apply the law to the facts of your case •
> Make conclusions about your case • Tell you if your answers are legally sufficient • Tell
> you about possible defenses, choices, or outcomes…"

It also warns: "Other people involved in your case may be able to use the legal system to
access the information you provide at this site."

## Where to put the disclaimers

Virginia Legal Ethics Opinion 1869 ([PDF](https://vsb.org/common/Uploaded%20files/LEOs/1869.pdf)),
approved by the Supreme Court of Virginia on November 2, 2016, is the best authority found on
questionnaire design. It recommends:

> "the use of a 'click-through' (aka 'click-wrap') disclaimer, which requires the prospective
> client to assent to the terms of the disclaimer **before being permitted to submit the
> information**."

And warns the person "to not disclose confidential or sensitive information," stating "that no
attorney-client relationship is being formed when a prospective client submits information and
that the firm has no duty to maintain as confidential any information submitted."

**Three layers, following the sites surveyed:** a persistent footer on every page; a click-wrap
gate before the questionnaire opens; and a disclaimer block rendered **inline with the result,
above the read** — not only in a linked terms page.

## Watch the marketing copy as hard as the disclaimers

*Janson* quoted LegalZoom's own homepage — "Just answer a few simple online questions and
LegalZoom takes over" — and concluded the portal sold "more than merely a good (i.e., a kit
for self help) but also a service."

Never write "we'll figure out the right structure for you" or anything in that family.
Describe the tool as an educational screening questionnaire producing general information.

## Keep humans out of the loop

*Janson* turned partly on non-lawyer employees reviewing each customer file. The court saw no
difference between that and "a lawyer in Missouri asking a client a series of questions and
then preparing a legal document based on the answers."

**Fully automated, deterministic output from published criteria is materially safer than a
person reading submissions and tailoring responses.** If anyone on the team ever reads a
visitor's answers and writes back, the analysis changes completely.

## Output framing

Never "you are eligible," "you should," "your company qualifies." Instead: "companies with
this profile are often considered plausible candidates," "these are the issues a company like
this typically faces," "you may want to discuss X with counsel."

Compare [Benefits.gov](https://www.benefits.gov/benefit-finder), which is careful throughout:
"a customized list of **potential** government benefits you **may be eligible for**."

The output must read as a **general description of a category**, not a conclusion about *this*
company. That is exactly the *Thompson* line, and it is Missouri law.

## Referral routing

Route to institutions, never to individuals, and never rank them. Missouri's own model is
"provide you with the number of the local lawyer referral service" — a number, not a
recommendation. The Missouri judiciary's site disclaimer expressly adds that it "does not
recommend or endorse any attorney."

Destinations worth listing: the Missouri Bar LawyerSearch,
[Missouri Free Legal Answers](https://missouri.freelegalanswers.org), legal aid, and domain
bodies including NCEO and [MOCEO](https://moceo.org/).

**ABA Free Legal Answers is a referral destination, not a design model.** It works because
volunteer attorneys form a limited-scope attorney-client relationship under Model Rule 6.5:
"When a client submits a question and receives an answer from a volunteer attorney, **an
attorney-client relationship is formed**." Its terms are a template for *forming* a
relationship, not avoiding one.

## Data handling

- State plainly that submissions are **not confidential and not privileged.** KU Legal
  Services for Students uses all caps: "PLEASE DO NOT SEND… ANY CONFIDENTIAL INFORMATION
  REGARDING YOUR SITUATION UNTIL SUCH TIME AS [we have] EXPLICITLY AGREED TO ADVISE AND/OR TO
  REPRESENT YOU." ([KU](https://legalservices.ku.edu/index.php/disclaimer))
- **Minimize collection.** Ask for ranges and bands, not exact financials. UGA's Business Law
  Clinic intake asks for the problem in "1–2 sentences is usually plenty."
- **Consider storing nothing.** A stateless calculator has the smallest surface, and it also
  keeps humans out of the loop by construction.

## Rule 13 does not apply, in either direction

Missouri Supreme Court Rule 13 (Legal Assistance by Law Students) was retrieved in full. It is
keyed entirely to an identified client or indigent person, a case or tribunal matter, and
written consent filed in the record. A public website answering anonymous business owners has
none of those.

**Rule 13 gives the team nothing here — and it is also not a restriction being violated.** The
analysis falls back entirely on §§ 484.010/.020 and *Thompson*. Kansas Supreme Court Rule 715
has the same structure and the same result.

## One judgment call for the team

Michigan and Illinois use **broad liability disclaimers and indemnification**. North Carolina's
safe harbor **forbids** them — § 84-2.2 disqualifies a provider that disclaims warranties or
limits damages.

That is a genuine jurisdictional split in philosophy. Since anything the team builds may be
university-associated, run this past whoever handles UMKC's institutional risk before choosing
a side.
