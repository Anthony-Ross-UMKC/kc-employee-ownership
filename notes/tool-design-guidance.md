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

---

# Corrections and additions from a second pass

## The sharpest statement of the line — and it is uncomfortable

**LSC Advisory Opinion AO-2017-004**
([lsc.gov](https://www.lsc.gov/about-lsc/laws-regulations-and-guidance/advisory-opinions/ao-2017-004)):

> "explaining the process for obtaining a child custody order is legal information. By
> contrast, **an evaluation of a parent's legal basis for a claim** for custody of a specific
> child is legal advice."

Applied here: explaining what an ESOP requires is information. **Evaluating whether this
company can do one is advice.** That is close to a description of what a candidacy screener
does, so the distinction has to be real rather than cosmetic — output that describes
categories a company might fall into, not an evaluation of the company in front of it.

Use this as the internal switch on every output: *does this require legal analysis applied to
this user's facts?* If yes, it belongs on a path with a licensed lawyer, not in the
questionnaire.

## A click-wrap gate cannot cure UPL

The click-through recommendation above stands, but **only for the problem it solves.**

- *Eisel v. Midwest BankCentre*, 230 S.W.3d 335 (Mo. banc 2007): "the activities prohibited by
  section 484.020 are **not subject to waiver, consent or lack of objection by the victim**."
- *Carpenter v. Countrywide*, 250 S.W.3d 697 (Mo. banc 2008): treble damages "do[] not require
  a finding of a culpable mental state."

**Consent solves relationship formation and user expectation. Only conduct design solves UPL.**
Two problems, two solutions; do not let the gate create false comfort.

## Michigan RI-301 — the four factors that kept a program clear

[Mich. State Bar Op. RI-301](https://www.michbar.org/opinions/ethics/numbered_opinions/RI-301)
found no attorney-client relationship, and no disqualification from later representing the
adverse party, where a self-help clinic was:

1. conducted **in a group setting**;
2. with **no individual consultation** in which confidential information was divulged;
3. collecting **only eligibility information** at intake; and
4. backed by a **signed written disavowal**.

Translated to software: broadcast-identical content, no confidential intake channel,
eligibility-only fields, click-accepted disavowal. This is the clearest target to build to.

## Disclaimers are judged by user expectation, not emphasis

[Utah Ethics Op. 96-12](https://www.utahbar.org/wp-content/uploads/2022/12/1996-12.pdf):
disclaimers are "effective where the individual receiving the information has **no expectation
that an attorney/client relationship is created**."

So control tone, personalization, second-person address, and anything resembling a human
persona — not just the boilerplate. A warm conversational interface undermines its own
disclaimer.

## Two refusal manuals worth hard-coding

**Texas Office of Court Administration**, *Legal Information vs. Legal Advice*
([PDF](https://www.txcourts.gov/media/1220087/legalinformationvslegaladviceguidelines.pdf)) —
a twelve-item "may not" list ("Recommend whether to file…", "Predict the outcome of a case"),
the heuristic that "**telling a member of the public what to do rather than how to do it** may
be giving legal advice," and a warning that showing only *some* options "may indirectly
influence a decision."

**That last point matters for design: show all options, never a ranked subset.** A ranked
recommendation engine is closer to advice than an exhaustive option list.

**Judicial Council of California**, *May I Help You?*
([PDF](https://courts.ca.gov/sites/default/files/courts/default/2024-10/mayihelpyou.pdf)) —
"'Can I?' or 'How do I?' … Telling someone how to do something is almost always appropriate,"
whereas "whenever you hear the word '**should**,' the court user may be asking for advice that
you cannot provide."

If any language model generates output here, these two lists are the refusal taxonomy to give
it.

## Structure the disclaimer as a stage, not a sentence

**New York courts' A2J best-practices guide**
([PDF](https://www.nycourts.gov/LegacyPDFS/ip/nya2j/pdfs/BestPractices_courtsystemdocument_assemblyprograms.pdf),
p. 15):

> "It is important to include a screen early in the program with a disclaimer that the program
> does not provide legal advice. This screen should require the user to respond with an
> **affirmative acknowledgment** and should include a pop-up or learn more on the difference
> between legal advice and legal information."

And: "**If information is essential for the litigant to read do not put it in a 'Learn More'
box. Most litigants do not read them.**" On screening (p. 16): "it is best to exclude them
early on… think about where to send excluded litigants when they exit the program."

A2J Author ships this as structure: a new interview's default steps are "(0) Access to
Justice, (1) **Do You Qualify?**, (2) **Do You Agree?**, (3) Your Information."

## Data retention, with real numbers

- Michigan Legal Help deletes answers after **60 days** (protection orders) or **180 days**
  (everything else), with an "Exit and delete my answers" button. Its triage tool "does not
  collect your name or contact information."
- Illinois Legal Aid Online deletes at **90 days** / **180 days** depending on platform.
- LawHelp Interactive does not autosave at all for guest users.

## Two Missouri-specific cautions

**[Missouri Informal Opinion 20000103](https://mo-legal-ethics.org/informal-opinion/20000103/)**
— the nearest Missouri authority on web intake, and it is a warning: "By providing the
opportunity to contact Attorney by e-mail through Attorney's website, Attorney exposes
Attorney's firm to certain risks. One of the primary risks is that an attorney-client
relationship will be established." It also flags **imputed conflicts** that could disqualify a
participating firm from unrelated adverse matters.

**An unfiltered free-text box is the highest-risk element on the page.** Structured choices
are safer than open input.

**Missouri Rule 4-6.5** (short-term limited legal services, relaxed conflicts) applies **only**
"under the auspices of a program sponsored by a nonprofit organization or court." If the team
ever wants that shelter, sponsorship structure is a compliance feature, not branding.

**Kansas bar ethics opinions are not published online at all**, so the Kansas side cannot be
researched the same way.

---

# Output framing — what real screeners actually say

## Start here: UMKC has already built one of these

The **Missouri Public Expungement Tool** — a guided interview that assesses eligibility under
§ 610.140 RSMo and generates a petition — was built by **UMKC School of Law's Clear My Record
project** and is now housed at the **Center for Law, Entrepreneurship and Innovation**
([lei.center](https://www.lei.center/projects/missouri-expungement-tools)).

This is the closest possible precedent: a public tool that evaluates a person's situation
against Missouri law, operated by this law school. Whoever built it already made every call
this project is about to make. **Talk to them before designing anything.**

**It is currently broken** — `expungementmo.civilaw.tech` returns a MySQL connection error.
Worth knowing as a lesson about who maintains these after the students graduate.

How it framed things (from an archived copy, since the live site is down):

- **Two-stage read.** Step names ran "Preliminary Review → Case Information → Lookup Your
  Offense → Categorize Offenses → … → **Final Eligibility Assessment** → Start Petition."
- **Never claims the outcome.** "This self-help tool is designed to help you generate the
  necessary paperwork… This tool does not file the documents for you… After filing the
  Petition for Expungement, it may take up to six months for **a judge** to make a decision."
- **Disclaimer in the footer of every step**, not just the intro: "The information provided by
  this tool is based on publicly available statutes and is intended for informational purposes
  only. It is not a substitute for professional legal advice… it is your responsibility to
  review the documents and ensure they meet your specific legal needs before filing."
- **Separate site-level disclaimer** disclaiming both the relationship and the accuracy:
  "using this website does not establish an attorney-client relationship… laws are constantly
  changing, and we cannot guarantee that the information provided is fully accurate or
  applicable to your case."

## The verb ladder

Attested across real tools, weakest to strongest:

1. "you **may be able to**" — Clean Slate PA headline
2. "**predict whether they might be** eligible" — Rasa Legal, describing its software
3. "you **may be eligible for** these benefits" — USAGov Benefit Finder results
4. "**Likely eligible** / More information needed / Not eligible" — USAGov per-item labels
5. "**confirm your eligibility**" — Rasa, but *only* after a licensed lawyer reviews
6. "**true eligibility**" / "**exact** premium" — reserved for the deciding agency

Nothing this project builds gets past rung 4.

## Name the confidence level — it beats a disclaimer paragraph

**Healthcare.gov** labels the same field "**Estimated Rate**" or "**Guaranteed Rate**"
depending on confidence, and stamps "**Prices here are estimates**" as a section heading, not
fine print. "Important: The premiums and tax credit you've seen here are just estimates based
on limited information."

**USAGov** splits the vocabulary by who is speaking: the tool produces "**your potential
benefits**"; the agency has "**true eligibility**." Its instruction is "Visit each agency to
find true eligibility and to apply."

Naming what kind of answer this is does more work than any paragraph of hedging.

## Disclaim the act, not just the content

**Upsolve's** terms are the UPL-safest sentence found, because they negate the definition
directly rather than characterizing the output:

> "**At no time do we review your answers for legal sufficiency, draw legal conclusions,
> provide legal advice, opinions or recommendations about your legal rights, remedies,
> defenses, options, selection of forms, or strategies, or apply the law to the facts of your
> particular situation.**"

Note "selection of forms" — directly relevant if this project publishes a form set.

Caveat: it did not save Upsolve at the Second Circuit, though *Upsolve v. James* concerned
live nonlawyer advice rather than software. The court held UPL statutes regulating
individualized advice are **content-neutral** speech regulations under intermediate scrutiny,
vacated the injunction, and remanded — leaving the First Amendment question unresolved.

## Disclaim the inputs too

More credible than a generic "not legal advice," and all attested:

- Clean Slate PA: "It relies on public data that [may] be imperfect, and **the screener can
  make mistakes**."
- The UMKC tool: "based on publicly available statutes."
- Rasa names the specific missing fields that block a confident read — probation end dates,
  close dates, legal financial obligations.

## Placement — almost everyone gets this wrong

Only two of the tools surveyed force acknowledgment **at the point of output** rather than
burying it in a terms page:

- **Clean Slate PA** puts a required consent checkbox inside the intake form, above Submit.
- **Illinois Legal Aid Online**'s triage ends with two required checkboxes, one of which is
  "**I know that just because I fill out this online form, no legal organization has taken my
  case.**"

The UMKC tool's footer-on-every-step is second best. Michigan Legal Help has **no inline
disclaimer** on its substantive pages at all — the hedging is done entirely by verb choice.

## Two models for handing off the hard part

- **Code for America's Clear My Record deliberately never told the user their eligibility.**
  The tool routed to a county public defender, who answered in about four weeks: "In about 4
  weeks, you'll hear from each county. They'll tell you what you qualify for." CfA later
  pivoted away from consumer screening entirely toward automatic record clearance.
- **Rasa Legal** splits it: software "predicts," a licensed lawyer "confirms" for a fee. Rasa
  carries no not-legal-advice disclaimer because it *is* a law firm and sells the confirmation.

Both are ways of not being the one who decides.

## Saving answers

- **USAGov saves nothing and says so before you start:** "We do not share, save, or submit
  your information."
- Clean Slate PA emails results and adds the user to a mailing list.
- Illinois Legal Aid, Michigan Legal Help and Upsolve all persist answers behind a login.

Storing nothing is both the safest privacy posture and the one that keeps humans out of the
loop by construction.
