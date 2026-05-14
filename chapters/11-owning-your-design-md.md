# Chapter 11 — Owning Your DESIGN.md

> Is the design system a tool you direct, or a set of defaults you inherited?

---

## 1. The feeling

You have been using the Brutalist system faithfully for a semester. The slides come out correct. The headlines assert. The bullets are gone. The color encodes. The figures pass the last-row test. Every diagnostic from the first ten chapters is, by visual inspection, in place.

And the slides feel generic.

A colleague who has also been using the system shows you their deck. Your deck and their deck look like the same deck. Same red. Same hierarchy. Same density. Same one-claim-per-headline rhythm. Your courses are not the same — yours is a discussion-heavy graduate seminar on intellectual history, theirs is a sophomore-level data structures lecture. The decks should not look the same. They do.

You sit with it for a while. The slides are not wrong. They are correct in the way a freshman essay can be correct — every sentence grammatical, no factual error, no clear vocabulary mistake — and still not the writing of someone who has something to say. The defaults are doing the talking. You are not.

That feeling is what this chapter is about. The diagnostic vocabulary you have built across ten chapters is the design *judgment*. The DESIGN.md is where that judgment lives persistently — or fails to live, when you let the defaults stand without examining them. The slides feel generic because the design philosophy is generic. The fix is not to change the slides. The fix is to own the file the slides are generated from.

## 2. The two diagnostic questions

Ask both, in this order, every time.

**From cognitive science:** *Do the defaults serve THIS course's pedagogy?* A 28-point body text size is a reasonable default. It is the right size for a 200-seat lecture hall with a 1080p projector at a viewing distance of 60 feet. It is too big for a seminar of twelve students around a table. It is too small for a 400-seat auditorium with a low-resolution projector. The cognitive payoff of a design system is consistency *within a context*. Inheriting defaults from a different context — even a thoughtfully constructed different context — does not produce that payoff.

**From visual design:** *Is this design system a tool I direct, or a set of defaults I inherited?* This is the question Brad Frost's *Atomic Design* ([free online, Frost 2016](https://atomicdesign.bradfrost.com/)) and the [W3C Design Tokens Community Group spec (Format Module 2025.10)](https://www.designtokens.org/tr/drafts/format/) `[verify community group status — note this is a CG document, not a W3C Standard]` both depend on but neither explicitly asks. A design system is structured to be *modified* — its whole point is that decisions live in named variables that propagate everywhere the variable is referenced. A reader who never modifies a default is not using the design system. They are using the system author's defaults.

## 3. The principle named

Plain language first: **the DESIGN.md is yours. Brutalist gives you defaults that don't fail. The default is a starting point, not a verdict.**

In framework vocabulary, this is the design-tokens-as-decisions move. A design token is a named entity that stores a single visual design value — a color, a font size, a spacing unit. The term was popularized by Salesforce's Lightning Design System team in approximately 2014 ([Salesforce SLDS documentation](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/tokens_intro.htm)), and the underlying idea — abstracting visual values into named variables — runs back through CSS custom properties, through the print-style-guide tradition (the *Chicago Manual of Style*, the AP Stylebook, *The New York Times Manual of Style*), and ultimately through the older fact that a decision made once and applied consistently is faster, cheaper, and more legible than a decision re-made on every artifact.

What is distinctive in the AI-mediated workflow — and what this chapter adds — is that the DESIGN.md is also a *prompt*. The Brutalist system reads DESIGN.md as part of the context window every time it generates a slide. Your design decisions are not just stored; they are *instructions to a model*. This is the move I am still working out the right name for. The traditional design-systems literature — Frost, Ellen Lupton in [*Thinking with Type*, 3rd ed. (Princeton Architectural Press, 2024)](https://ellenlupton.com/Thinking-with-Type), the SLDS / Material / Linear lineage — assumes a human designer or typographer applying the system. The DESIGN.md is read by both human and model and must be legible to both. No peer-reviewed treatment I can find names this dual-audience constraint as a category, which is honest to flag: the framing is original to this book, and I do not yet have an empirical case that it produces better outcomes than ad-hoc prompting. The structural argument is strong; the empirical argument is not yet.

The chapter's central claim follows from the dual-audience reading. **A DESIGN.md that is a collection of accepted defaults is a starting point. A DESIGN.md that is a collection of decisions — each traceable to a principle from cognitive science or visual design — is a design philosophy.** The reader who can explain why their body text is 28pt and not 24, why their red is brand and not danger, why their headlines are claims and not labels — that reader owns their slides. The reader who can only say "I prefer this" has not yet done the integration this chapter requires.

The book is not prescribing the Brutalist aesthetic. It is prescribing the *vocabulary* that makes any aesthetic decision defensible. Your DESIGN.md may end up looking very different from the Brutalist defaults. That is the point. The diagnostic questions are prescriptive; the answers are not.

## 4. Bad example

Here is a DESIGN.md that has been "in use" for a year, by a faculty member teaching an intellectual-history graduate seminar of twelve students. The file is a verbatim copy of the Brutalist defaults. The faculty member has never opened it.

```markdown
<!-- BAD: an unowned DESIGN.md. Every variable is the Brutalist default.
     The course is a 12-student graduate seminar on Foucault. None of the
     variables have been examined against that context. The file is a
     starting point treated as a verdict. -->

# DESIGN.md — Visual Constitution
*(Brutalist D3 default — unmodified)*

## Color system
--color-white:     #FFFFFF;   /* canvas */
--color-ink:       #121212;   /* primary text */
--color-red:       #C8102E;   /* primary accent — NEU Red */
--color-secondary: #545454;
--color-border:    #D4D4D4;
--color-ochre:     #C8860E;   /* decorative highlight */

## Typography
--font-body:       'Inter', system-ui, sans-serif;
--font-size-body:  28pt;      /* for lecture-hall projection */
--font-size-h1:    44pt;
--line-height:     1.4;

## Slide grammar
headline_must_assert: true
headline_max_words:   12
body_text_density_max: 60_chars
visual_form_default:  diagram_over_list

## Notes field
notes_required_when_live_deck: true
```

What fails, point by point.

The accent red is `#C8102E` — Northeastern University red, the brand color of the institution this Brutalist instance was originally tuned for. The faculty member teaches at a different university whose brand red is `#7B0000` and whose institutional style guide reserves any red for emergency signage. The slides are using another institution's brand color, on a campus where that color reads as a brand collision. The variable was never examined.

The body text is 28pt. This is sized for a 200-seat lecture hall — the original Brutalist context. A 12-person seminar room has a viewing distance of perhaps 12 feet, not 60. At 28pt, body text in this room is enormous; three short bullets fill the screen. The density is wrong for the context, but the variable is correct for some other context, so it does not visibly fail. It just makes every slide feel like a placard.

The visual form default is `diagram_over_list`. This is sensible for a quantitative course where most relationships are causal or comparative. The seminar in question teaches primary-source reading — Foucault, Arendt, contested archival material. The "right" visual form for a slide that quotes a 300-word passage is *the passage*, set in a readable serif, with margin annotations. A diagram-over-list default is fighting the course's pedagogy on every slide.

The headline rule is `headline_must_assert: true`. This is correct for almost every course — except possibly this one. A seminar's slide may legitimately be *"Foucault, Discipline and Punish, 1975, p. 217–220"* — a citation slide that orients a discussion rather than asserting a claim. The default rule produces forced assertions on slides that should be reference orientation. The file does not name the exception.

The file is not wrong in any single variable. It is wrong as a whole, because nobody decided anything. The defaults are reasonable for the context the system was tuned in, and they have never been re-examined for the context the file is actually being used in. This is the canonical failure mode the chapter is about — defaults masquerading as decisions.

## 5. Good example

The same faculty member, after working through this chapter, produces a DESIGN.md that reads like decisions.

```markdown
<!-- GOOD: an owned DESIGN.md. Every variable has been examined against
     the course context (12-person grad seminar on Foucault, primary-source
     reading, 75-minute sessions twice a week) and either endorsed with a
     reason or changed with a reason. The file is a design philosophy. -->

# DESIGN.md — Visual Constitution
## HIST 504: Power, Discipline, Knowledge — Spring 2026
*Last revised: 2026-04-12 (initial ownership pass after Ch 11)*

## Color system
--color-white:     #FAFAF7;   /* warm canvas — paper-like, easier on eyes
                                  for long passage reading. Departed from
                                  pure white default; primary mode of slide
                                  use is reading, not chart display. */
--color-ink:       #1a1a1a;
--color-accent:    #5B3A29;   /* deep brown — annotation accent, used for
                                  margin marks on quoted passages. Replaces
                                  Brutalist red. Institutional brand
                                  considerations and aesthetic neutrality for
                                  a course on power. Departure is deliberate. */
--color-secondary: #4F4F4F;
--color-border:    #C9C5BB;
/* No ochre. Decorative accent is not needed for a primary-source-reading
   course; one accent does the work. Removing the variable rather than
   leaving it undocumented. */

## Typography
--font-body:       'Source Serif Pro', Georgia, serif;
                  /* Serif default. The slides are 30%+ quoted passages of
                     historical prose. Serif aids reading at sustained
                     paragraph length. Sans-serif was the wrong default for
                     this course's content type. */
--font-quote:      'Source Serif Pro', Georgia, serif;
--font-meta:       'Inter', system-ui, sans-serif;
                  /* Citations, dates, page numbers in sans. The two-family
                     split signals "this is the source / this is my
                     orientation to it" without explanation. */

--font-size-body:  22pt;      /* seminar room (12 seats, 12-foot max
                                  viewing). 28pt was lecture-hall scaled
                                  and read as placards in this room. Last-
                                  row test passed at 22pt for this space. */
--font-size-h1:    32pt;
--line-height:     1.55;      /* generous leading for paragraph-length
                                  quoted passages. */

## Slide grammar
headline_style: hybrid
  # Teaching slides (about 70% of the deck): full-sentence assertion.
  # Citation slides (about 25% of the deck): "Author, Work, Year, p. N"
  #    label — these orient discussion, not assert claims.
  # Discussion-prompt slides (about 5%): question fragment ("What is
  #    a 'docile body'?") — neither assertion nor citation.
  # Three slide types, three headline grammars. The reference-slide
  # exception named in Ch 10 needed expanding for this course.

body_density_max: 250_words_for_quoted_passages
                  # Departed from Brutalist 60-char cap. Passage-reading
                  # is the course's central activity. Hard cap on
                  # author-written prose still 60 chars; quoted passages
                  # carry their own density limit (~250 words / 1 minute
                  # of reading aloud).

## Notes field
notes_field_role: discussion_prompts
                  # In a lecture deck, notes carry async-study explanation.
                  # In this seminar deck, notes carry the two or three
                  # discussion questions I plan to lead with. Different
                  # course shape, different notes-field role. Documented
                  # so the next semester's deck doesn't drift back to the
                  # default usage.

## Per-slide-type DESIGN extensions
slide.citation:
  border-left: 4px solid var(--color-accent);
  font-style: italic;
  padding-left: 32px;
                  # Citation slides are visually marked. The student
                  # recognizes the type at a glance and adjusts reading
                  # mode. Convention applied consistently across the deck.

slide.passage:
  font-family: var(--font-body);
  margin: 0 12% 0 12%;
  /* The quoted passage occupies the slide. No competing elements.
     Margin-set so the slide feels like a printed page in the seminar
     room — paper-on-paper rather than slide-as-poster. */
```

What changed: every variable has a comment explaining why it has the value it has. The comments are not aesthetic — they are *in framework vocabulary*. The body font is serif because the course content is paragraph-length quoted prose (Mayer's multimedia principle does not say "text is bad"; it says "the visual channel is underused when content can be visualized." Quoted historical prose is content that is *not* better visualized; the serif is the right default for it). The body size is 22pt because the last-row test in this room passes at 22pt — the same test from Chapter 6, applied to a different room. The accent is brown rather than red because the institutional context makes red read as a brand collision; the default would have been wrong despite being correct in the Brutalist reference instance. The notes field carries discussion prompts rather than async-study text because the course is a seminar, not a lecture — different deck shape, different notes-field role.

The headline rule is the most consequential departure. The Brutalist default `headline_must_assert: true` was correct in spirit but wrong in coverage. This deck has three slide types, and only one of them takes assertion headlines. The file names the three types explicitly and assigns each a headline grammar. The reference-slide exemption from Chapter 10 has been *expanded* — not abandoned. The chapter said "default to assertions for teaching slides, allow labels for reference slides, document the rule explicitly." This DESIGN.md does that, with the specific case the course faces.

Notice what makes the good example *good*. It is not that the variables are different from the Brutalist defaults. Most of the variables are the same or similar. It is that every variable is now a *decision* — endorsed or changed, with a reason in framework vocabulary. The faculty member can hand this file to a skeptical colleague and defend every line. The bad version had no defense because there were no decisions, just inheritance.

## 6. The prompt

Paste this into the Brutalist system. The prompt assumes you have used the system for at least one full deck — you need slides to react to.

```
Audit this DESIGN.md against the courses I teach and the institution's
brand. Report on three dimensions:

1. PALETTE. For each color variable, ask: does this color encode
   something specific in my course's content, or is it inherited from
   the Brutalist reference instance? Flag colors that have no encoding
   role for my context. Flag any color that creates a brand collision
   with my institution.

2. TYPOGRAPHY. For each typography variable, ask: is this sized for
   my lecture room, my content type, and my students' reading
   conditions? Flag font sizes that pass the last-row test in the
   Brutalist reference space (200-seat lecture hall) but not in my
   space. Flag font families that fight my content type — sans-serif
   when most slides are paragraph-length prose, for instance.

3. DENSITY AND HEADLINE GRAMMAR. For my course shape (lecture /
   seminar / studio / lab), is the default body-text-density cap
   correct? Is the default headline-must-assert rule correct, or does
   my course have legitimate reference-slide types that need a
   different headline grammar? Name the slide types explicitly.

For each flag, propose the DESIGN.md change. Include a one-sentence
rationale in framework vocabulary — cognitive science or visual
design. If you cannot justify the change in framework vocabulary,
flag it as aesthetic preference and ask me to re-examine.

Return the proposed DESIGN.md as a diff against the current file, with
inline comments preserved.
```

Two things to notice. First, the prompt names the three dimensions the chapter has been working through — palette, typography, density. It does not ask for an open-ended audit, which would produce open-ended results. Constraining the question is what makes the answer usable. Second, the prompt explicitly demands *framework vocabulary* for every proposed change. A change defended as "I like it better" gets flagged for re-examination. This is the discipline the chapter has been arguing for, embedded into the prompt itself. The reader who runs this prompt is forcing their DESIGN.md to defend itself — which is what ownership looks like in practice.

## 7. The DESIGN.md change

The DESIGN.md change *is* the chapter. There is no single variable to update. The chapter teaches the reader to own the entire file.

What this means concretely. After running the audit prompt, you will have somewhere between three and ten proposed changes. Some you will accept, some you will reject, some you will modify. For each change you accept, write a one-sentence comment in the file naming the principle that justifies it. For each default you keep, write a one-sentence comment naming the principle that endorses it. A variable without a comment is a variable you have not yet examined. The discipline is not to make the file longer; it is to make every line of it a decision.

I am tempted to give you a target number — "comment every variable" or "departures from defaults should be at least 20%" — and I am going to resist. The target is not a quota of departures. A DESIGN.md that endorses 90% of the Brutalist defaults can be fully owned, if each endorsement was the result of examination. A DESIGN.md that departs from 50% of the defaults can be fully unowned, if the departures are aesthetic preference. The test is not how many variables you changed. The test is whether each variable in the file is something you can defend.

The reflexive point is the one this chapter is built around. The Brutalist DESIGN.md you read in Appendix A is itself an opinionated file — somebody examined every variable against a particular context (probably a quantitative course taught at a particular institution by a particular author) and arrived at the defaults you inherited. The defaults are not arbitrary, but they are also not universal. The author of those defaults endorsed each one for their context. Your job, at this point in the book, is the same operation — endorse each variable for *your* context, or change it. The artifact you produce will look different from the artifact the Brutalist author produced. Both can be fully owned. Ownership is not convergence. Ownership is examination.

## 8. The diagnostic questions to keep

Run any DESIGN.md through these. If any answer is *I don't know* or *it was the default*, that variable has not yet been owned.

1. **Can I explain every variable in my DESIGN.md in one sentence?** The sentence is the decision. A variable without a one-sentence justification is still a default.
2. **Is each decision traceable to a principle from cognitive science or visual design?** "Mayer's multimedia principle" or "the last-row test" or "the slideument distinction" — the vocabulary built across the prior chapters. A justification that lives outside the framework ("I like it better") is not yet a decision.
3. **If I changed this variable, could I say why?** Not the value — the *variable*. Why does this variable exist in my DESIGN.md? What problem does it solve? A variable without a problem is dead weight in the file.
4. **Are my reference-slide conventions named separately from my teaching-slide conventions?** A course with multiple slide types (lecture + discussion-prompt + citation) needs the DESIGN.md to acknowledge them. A file that treats all slides as one type produces forced assertions on citation slides.
5. **When the system generated a slide I disliked, did I update DESIGN.md or did I tweak the slide?** The slide tweak is the per-slide fix. The DESIGN.md update is the rule. A reader who finds themselves making the same fix on slide after slide has skipped the DESIGN.md update — and is no longer using the design system.

## 9. What two people might disagree about

Two faculty members can read this chapter and arrive at honest, defensible disagreements. Naming where matters more than picking a side.

**How prescriptive a DESIGN.md should be.** The Brutalist tradition takes a relatively prescriptive position — most decisions live in DESIGN.md, slides apply them, the file is opinionated. Other design-systems traditions leave more latitude to the artifact author. Linear's design system is heavily specified; Notion's is looser; Stripe's is somewhere between. The vocabulary that lets these positions argue: *when does specification stop being load reduction and start being load production?* A 40-variable DESIGN.md that has to be re-consulted for every slide is not reducing cognitive load. A 4-variable DESIGN.md that forces re-decision on most details is not either. The right number is whatever level of specification offloads the decisions you make repeatedly and leaves room for the decisions that should be per-slide judgment. The defensible position is to start prescriptive (Brutalist defaults) and relax where you find the file is constraining without earning the constraint. The undefendable position is to leave the file uninhabited because "design feels personal."

**Whether the prompt-as-design framing is the right vocabulary.** I called the DESIGN.md a "prompt for the model" earlier in this chapter, and I want to flag that this framing is one I am working out as I write. The traditional design-systems literature (Frost, Lupton, SLDS) treats the design system as a *specification* — a normative artifact a human designer applies. The AI-mediated workflow makes the system both specification and instruction, and I do not yet have a published reference that names this dual nature in a way I find fully satisfying. Two reasonable positions: (a) the DESIGN.md is a design system that happens to be model-readable, no different in kind from a print style guide; (b) the DESIGN.md is a new artifact type whose specification grammar is distinctly shaped by the fact that a model has to apply it. I lean toward (b) and the chapter argues for it, but I cannot point to peer-reviewed work that settles the question. If you read this chapter and disagree, the disagreement is genuine.

**Whether ownership requires departure or just examination.** Some readers will conclude this chapter by changing many variables. Others will conclude it by changing very few. The chapter's position is that the test is examination, not departure — but the test is fragile. A reader who "examines" each variable and concludes "the default is fine" without much engagement can produce a file indistinguishable from the unowned bad-example case. The defensible practice is to write the one-sentence justification for each variable *out loud, in the file as a comment*. A justification you cannot write is a justification you have not made. This is the discipline that distinguishes endorsement from acceptance.

---

You started this chapter with a deck that worked and felt generic. Run the audit prompt against your DESIGN.md and the genericness will turn out to be specific — particular variables, inherited from a context that is not yours, that the audit will name. Update the ones that need updating. Endorse the ones that don't. Write the comments. Regenerate the deck.

The deck will not look dramatically different. Most of the variables stay where they are; the Brutalist defaults are not bad defaults. What changes is the file. The DESIGN.md is no longer a hand-me-down from the system's reference instance. It is yours. Every line of it is something you decided.

The book has one more piece. Eleven chapters of diagnostic vocabulary. One DESIGN.md you can defend. What you do not yet have is a way to *use* the vocabulary on a deck you have never seen before, fast, without re-reading the book. That artifact is Chapter 12.

---

**What would change my mind:** An empirical study comparing decks generated from heavily-specified DESIGN.md files against decks generated from minimally-specified DESIGN.md files, where the comparison shows that minimal specification produces equivalent or better outcomes once the author has built diagnostic vocabulary. The chapter's claim that DESIGN.md ownership scales better than per-slide tweaking is a structural argument, not an empirical finding. If a study arrives showing that expert authors do better with permissive systems than with prescriptive ones, the chapter's prescription weakens for that subset of readers.

**Still puzzling:** I do not have a clean rule for how much of a DESIGN.md should be specified versus left to the model. The chapter takes Brutalist's relatively prescriptive position because the audience is novice-in-design, and prescription scaffolds judgment until judgment exists. After a year of use, a reader probably wants to relax some prescriptions and tighten others. I cannot say in advance which ones, because the answer depends on what the reader's eye has actually internalized. The reflexive move is that the DESIGN.md itself evolves — but the trajectory of that evolution is something I am still working out.

**Tags:** design-tokens, atomic-design, Frost, design-system-ownership, prompting-as-design
