# Research Notes: Chapter 11 — Owning Your DESIGN.md

**Source:** TIKTOC.md chapter entry
**Notes file:** 11-owning-your-design-md_notes.md
**Corresponding chapter:** chapters/11-owning-your-design-md.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader integrates ten chapters of diagnostic vocabulary into a DESIGN.md they can explain, defend, and update — one that reflects their own design philosophy, not the Brutalist default.

**The feeling:** Looking at a DESIGN.md after ten chapters and seeing it differently. Variables that were arbitrary are now decisions. Defaults that were accepted are now either endorsed or changed.

**The integration:** Each prior chapter gave the reader a vocabulary and a variable. This chapter asks: what is YOUR answer to each of these questions, and why?

**The DESIGN.md as design philosophy:** A DESIGN.md that is a collection of defaults is a starting point. A DESIGN.md that is a collection of decisions — each traceable to a principle from one of the two frameworks — is a design philosophy.

**The reader's DESIGN.md may look different from yours:** That is the point. The book is not teaching the Brutalist aesthetic. It is teaching the vocabulary that makes any aesthetic decision defensible.

**Final prompt:** Write your own DESIGN.md rationale document — one paragraph per major decision, stating the principle behind it in vocabulary from both frameworks.

---

## A. Conceptual foundations

### Design tokens — what a DESIGN.md variable actually is

A design token is a named entity that stores a single visual design value: a color, a font size, a spacing unit, a contrast ratio, a layout breakpoint. The term was popularized by Salesforce's Lightning Design System team in the mid-2010s but the underlying idea — abstracting visual values into named variables — predates the term by decades in software engineering. The W3C Design Tokens Community Group reached its first stable specification in October 2025, formalizing a vendor-neutral JSON format for sharing tokens across tools and platforms. The specification matters here because it confirms that "design tokens" is now an industry standard term with a precise definition, not a marketing coinage.

The pedagogical move in this chapter is to treat DESIGN.md as a token file written in prose rather than JSON. Each variable in DESIGN.md — body font size, body font color, accent color role, headline weight, slide grid unit, density target — is a design token. The prose form is appropriate for the Brutalist system because the system reads the file as natural language and applies the tokens through prompts; the principle is identical to a Style Dictionary JSON file that compiles to CSS custom properties. The reader does not need to know JSON. They do need to understand that the variable they are updating is a token in the technical sense: a single value, named, reused everywhere that value is needed, changed in exactly one place.

The cognitive payoff of this framing is that variable changes propagate. When the reader updates "body font size: 28pt" in DESIGN.md, every slide that uses body text gets the new value. The reader is no longer making fifty per-slide tweaks; they are updating one token. This is the difference between editing a deck and owning a design system.

**Common misconception:** That tokens are technical infrastructure separate from design decisions. They are not. Each token *is* a design decision, made once, applied consistently. The DESIGN.md is the document of those decisions. A token without a rationale is a default in disguise.

**Worked example:** A faculty member dislikes the accent ochre color when it appears next to body text. The wrong fix is to find the slides where ochre appears next to body text and change the color on each. The right fix is to update DESIGN.md: "accent color is reserved for emphasis on numeric claims; never paired with body prose." That single rule, expressed as a token-level constraint, replaces dozens of per-slide judgments.

**Source(s):**
- Design Tokens Community Group. (2025). Design Tokens Format Module 2025.10. https://www.designtokens.org/tr/drafts/format/
- Salesforce. Styling with Design Tokens and Styling Hooks (Lightning Aura Components Developer Guide). https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/tokens_intro.htm
- Style Dictionary. Design Tokens Community Group. https://styledictionary.com/info/dtcg/

### Atomic design — Brad Frost and the hierarchy of design system thinking

Brad Frost's *Atomic Design* (2016, freely available online at atomicdesign.bradfrost.com) is the most widely cited contemporary framework for organizing a design system. Frost borrows from chemistry: atoms (basic building blocks — a button, a label, a color value), molecules (combinations of atoms — a search input with a label and submit button), organisms (combinations of molecules — a header with logo, navigation, and search), templates (page-level structures), and pages (specific instances filled with real content).

The framework's relevance to DESIGN.md is structural. A slide deck is the "page" level. A slide template is the "template" level. A repeating slide element — a citation block, a section divider — is an "organism." The slide's components — the headline element, the body element, the figure caption — are "molecules." The tokens — color values, font sizes, spacing units — are "atoms." DESIGN.md, in atomic-design terms, lives at the atoms-and-molecules level: it specifies the building blocks and the rules for combining them. The slides themselves are pages, generated at runtime by the Brutalist system from the atomic specifications.

The deeper pedagogical point in Frost is that *consistency at the atomic level enables variation at the page level*. A design system that locks down atoms and molecules can produce thousands of different slides while maintaining a coherent visual language. A design system that tries to lock down the page level produces brittle templates that fight every new slide. The reader's DESIGN.md should be opinionated about atoms (specific color values, specific font sizes) and permissive about pages (slides can vary widely as long as they use the specified atoms).

**Common misconception:** That atomic design is about literal hierarchy — that every design element must fit one of the five levels exactly. Frost is explicit that the levels are heuristic, not rigid. The point is the cognitive move (small reusable parts compose into larger structures), not the chemistry analogy itself. The chapter should adopt the move and not over-extend the metaphor.

**Worked example:** A DESIGN.md that specifies "primary red: #C81E1E" (atom), "headline = primary red on white, 36pt sans-serif" (molecule), "section divider = single full-bleed headline on primary red background" (organism). Every section divider in every deck is generated from this one specification. Change the atom (the red value) and every section divider updates in lockstep.

**Source(s):**
- Frost, B. (2016). *Atomic Design*. https://atomicdesign.bradfrost.com/
- Frost, B. *Atomic Design*, Table of Contents. https://atomicdesign.bradfrost.com/table-of-contents/

### Style guide as artifact — the older tradition

Style guides predate the internet by centuries. Newspaper style guides (*Chicago Manual of Style*, the AP Stylebook, *The New York Times Manual of Style and Usage*) codify the rules a newspaper applies to every story — punctuation, capitalization, treatment of names, handling of contested terms. The function is identical to a design token file: capture a decision once, apply it consistently across thousands of artifacts. The cognitive load reduction is the same: the writer no longer thinks about whether to capitalize "internet" on each story; the decision was made once, in the style guide, and the writer applies it without re-deciding.

Ellen Lupton's *Thinking with Type* (3rd ed., 2024) is the modern bridge between print style-guide tradition and contemporary design system thinking. Lupton's three sections — letter, text, grid — map directly onto the layers a slide DESIGN.md must specify: typography choices (letter), text-block conventions (text), layout structure (grid). Lupton's pedagogical move is also the chapter's: rules are tools, not constraints. Learning the rules makes it possible to break them deliberately rather than accidentally.

The slide-design specific style-guide lineage runs through Reynolds (*Presentation Zen*, 2008), Duarte (*slide:ology*, 2008), and Kosslyn (*Clear and to the Point*, 2007). Each of these is a style guide for slides — a set of decisions made once and applied consistently. The Brutalist DESIGN.md is structurally the same artifact, formalized for an AI-mediated workflow.

**Common misconception:** That a style guide is a constraint on creativity. It is the opposite — a style guide frees the author from re-deciding settled questions and reserves attention for the questions that actually need judgment on each new artifact.

**Worked example:** *The New York Times* style guide specifies that book titles are italicized in body text and quoted in headlines. A reporter writing a story about a book never has to decide which convention to use; they apply the rule. A slide DESIGN.md that specifies "tables of numeric data use the figures-tabular font feature; tables of text use proportional figures" eliminates the same re-decision on every data table.

**Source(s):**
- Lupton, E. (2024). *Thinking with Type: A Critical Guide for Designers, Writers, Editors, & Students* (3rd ed.). Princeton Architectural Press. https://ellenlupton.com/Thinking-with-Type
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders.
- Duarte, N. (2008). *slide:ology: The Art and Science of Creating Great Presentations*. O'Reilly.
- Kosslyn, S. M. (2007). *Clear and to the Point: 8 Psychological Principles for Compelling PowerPoint Presentations*. Oxford University Press.

### Prompting as design — the new layer this chapter adds

What is distinctive to the AI-mediated workflow — and to this chapter — is that the DESIGN.md is also a *prompt*. The Brutalist system reads DESIGN.md as part of the context window every time it generates a slide. The reader's design decisions are not just stored; they are *instructions to a model*. This changes what a DESIGN.md must contain. A traditional style guide can say "use 24-point body text"; the human typographer interprets that correctly. A DESIGN.md must say "body text: 24pt; body text color: #1a1a1a; body text line-height: 1.4; body text never appears in accent color (red or ochre)" — the model needs the rule and the constraint, not just the value.

The pedagogical implication: the reader's job, after this book, is no longer to hand-tweak slides. It is to update the DESIGN.md variable so that the next generation of slides is correct without intervention. A faculty member who finds themselves manually fixing the same problem on slide after slide has skipped the DESIGN.md update. The fix that scales is the rule, not the per-slide intervention.

This is also where the Brutalist system departs from the traditional design-system literature. Frost's *Atomic Design* assumes a human designer applying the system. Lupton assumes a human typographer reading the style guide. The DESIGN.md is read by both human and model, and must be legible to both. The chapter's move is to make this dual-audience constraint explicit and turn it into a discipline: every DESIGN.md rule must be specific enough that a model can apply it without ambiguity, and the rationale must be clear enough that a human reader can defend it.

**Common misconception:** That DESIGN.md is "just prompts." It is not — it is design decisions, expressed in a form a model can apply. The "just prompts" framing produces ad-hoc rules without rationale; the "design system" framing produces a coherent artifact with defensible decisions.

**Worked example:** A reader notices that the system keeps generating slide headlines as labels rather than assertions (Ch 10 failure). The wrong fix is to add "use assertion headlines" to each slide prompt. The right fix is to update DESIGN.md: "headline style: complete sentence, declarative, stating the slide's main claim; reference slides (glossary, agenda) may use noun-phrase labels — name them explicitly." The next hundred slides apply this without intervention.

**Source(s):**
- Frost, B. (2016). *Atomic Design*. https://atomicdesign.bradfrost.com/
- Design Tokens Community Group. (2025). Format Module 2025.10. https://www.designtokens.org/tr/drafts/format/
- Brutalist DESIGN.md (in pantry/brutalist/DESIGN.md) — the reference implementation.

### Defending departure from defaults — the principled-disagreement move

The last conceptual layer the chapter adds is the *defense*. A DESIGN.md that matches the Brutalist defaults is not yet owned — the reader has merely accepted a starting point. A DESIGN.md that departs from defaults is owned only if the departure can be justified in the diagnostic vocabulary of the prior chapters. "I changed body text from 24pt to 22pt because my projection environment uses higher-resolution displays and the last-row test still passes at 22pt" is a principled departure. "I changed body text to 22pt because I like it better" is not.

The discipline here is not that the reader must accept the Brutalist defaults; it is that any change must be expressible in the framework's vocabulary. This is the meta-move the chapter teaches: the book has built a vocabulary, and ownership is demonstrated by using that vocabulary to defend specific decisions. The reader who can say "my headline weight is 700 because I want the assertion to dominate the body diagram, and 600 was reading as part of the same hierarchy level" has internalized the framework. The reader who can only say "I prefer 700" has not.

**Common misconception:** That the Brutalist defaults are the right answers and any departure is a mistake. The book is explicit that the defaults are starting points. The mistake is undefended departure, not departure itself.

**Worked example:** Two faculty members produce different DESIGN.mds. The first uses 28pt body text, no accent color, and assertion headlines. The second uses 22pt body text, ochre accent for definition-of-term moments, and label headlines for a reference-heavy course. Both are correct *if* both can defend their choices in the framework's vocabulary. The chapter teaches the defense, not the answer.

**Source(s):**
- Brutalist DESIGN.md (pantry/brutalist/DESIGN.md). — the reference defaults.
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.). — the aesthetic of restraint, one example of a defensible position.
- Tufte, E. R. (2006). *The Cognitive Style of PowerPoint* (2nd ed.). Graphics Press. — a different defensible position.

---

## B. Domain examples and cases

### Case 1: Salesforce Lightning Design System and the "decisions made once" payoff

Salesforce introduced the Lightning Design System (SLDS) and design tokens in approximately 2014. The internal payoff was concrete: across thousands of components built by hundreds of teams, brand consistency was maintained by changing token values in a single source file. When Salesforce shifted to a new visual identity (SLDS 2, Spring 2025), the migration ran through token updates rather than per-component edits. The case demonstrates the economic argument for design tokens at scale: the up-front cost of building a token system is repaid every time the design shifts.

The DESIGN.md analog is the same. A faculty member who maintains a course's slides over five semesters and decides in semester three that the body text needs to be larger updates one token. The slides for semesters three through five regenerate with the new token. The slides for semesters one and two — if the source markdown is preserved — can regenerate as well.

**Source:** Salesforce. Styling with Design Tokens. https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/tokens_intro.htm

### Case 2: Material Design tokens — the public-facing scale case

Google's Material Design has used design tokens since approximately 2014 and made them publicly available as a reference. The case is interesting because Material Design is consumed by external developers at scale; the token format has to be precise enough for non-Google engineers to apply without ambiguity. This forced precision is the same discipline a DESIGN.md must impose: specifications must be unambiguous enough for a model to apply, not just enough for a human collaborator to interpret.

**Source:** Material Design. Design Tokens. https://m3.material.io/foundations/design-tokens/overview (or current canonical Material 3 docs).

### Case 3: Linear, Vercel, Stripe — modern design-system blog culture

The 2020s saw a wave of well-documented design systems from software companies — Linear, Vercel, Stripe, Notion — each publishing their token specifications and design principles publicly. The case-study value for the chapter is that these systems each made distinct, defensible decisions. Linear's typography is dense and information-rich; Stripe's is generous and air-filled; Vercel's is geometric and high-contrast. Same design-system structure, three different aesthetics, each defensible in framework vocabulary. This is the reader's lesson: ownership is not about converging on the Brutalist look. It is about owning the choices.

**Source:** Linear, Stripe, Vercel design system documentation (publicly available; URLs vary, [verify current canonical sources before citing]).

### Failure case: The unowned DESIGN.md — defaults masquerading as decisions

The canonical failure case is the faculty member who runs the Brutalist system unmodified for a year, then complains that their slides "all look the same as everyone else's." They have not lost ownership of their slides; they never had it. A DESIGN.md the reader has never opened and never modified is not theirs — it is the system's defaults applied without examination. The chapter's diagnostic move is to make this audible: can the reader explain why each variable has the value it has? If the answer is "I don't know, it was the default," that variable is not yet owned.

This is not pejorative. Defaults exist because they are reasonable starting points. The chapter's argument is that owning the file requires the reader to either *endorse* each default (with a reason) or *change* it (with a reason). Endorsement is owning. Acceptance without examination is not.

**Source:** Original framing. The Brutalist book's central pedagogical move.

---

## C. Connections and dependencies

**Prerequisites (what reader must already know):**
- The full diagnostic vocabulary built across Ch 1–10. This chapter does not introduce new vocabulary; it integrates the existing vocabulary into the DESIGN.md as defensible decisions.
- The Brutalist DESIGN.md structure and where to edit it (covered in Appendix A).
- Recognition that AI slide tools read DESIGN.md as part of the prompt context — the design-system layer is not optional infrastructure; it is the interface to the model.

**Unlocks (what this chapter makes possible):**
- The reader can update DESIGN.md to fix a class of slide problems rather than the individual slide.
- The reader can defend their DESIGN.md to a skeptic in framework vocabulary, completing the book's promise.
- The reader can read another person's DESIGN.md and predict what their slides will look like — and disagree with specific choices, in framework vocabulary, rather than aesthetically.
- Chapter 12's diagnostic checklist becomes operational — the checklist tests the slide; the DESIGN.md sets the rules the slide should be tested against.

**Adjacent chapter connections:**
- Chapters 1–10 (all): each chapter gives the reader a variable. This chapter is the integration where the variables become an owned file.
- Chapter 12 (Diagnostic Checklist): the checklist asks whether the slide meets the standards the reader's DESIGN.md sets. A DESIGN.md without ownership produces a checklist without teeth.
- The Brutalist series: this is the meta-chapter that surfaces what the Brutalist methodology *is* — system files as authoritative specifications, not configuration.

---

## D. Current state of the field

**Settled:**
- Design tokens are a now-standard pattern for software design systems (Salesforce, Google Material, the W3C Design Tokens Community Group spec at 2025.10 stable).
- The atomic design framework (Frost) is widely adopted in the industry and is treated as foundational in design-system curricula.
- Style guides as artifacts predate the design-system formalism by a century (newspaper style guides, the *Chicago Manual*).
- Specification clarity matters more for AI-mediated workflows than for human-only ones — the model cannot interpret the way a human collaborator can.

**Contested or emerging:**
- *Whether prompts and design tokens are the same thing or distinct.* The chapter's position is that DESIGN.md tokens are a subset of the prompt — design decisions that the model applies automatically. The broader prompt-engineering literature is still emerging; this chapter contributes a teaching frame.
- *How prescriptive a DESIGN.md should be vs. how much it should leave to per-slide judgment.* Brutalist takes a relatively prescriptive position (most decisions in DESIGN.md, slides apply them); other systems leave more latitude. The chapter should name this as a choice, not a settled answer.
- *Whether AI-mediated design systems will converge or diversify aesthetically.* Industry early signs suggest convergence (everything starts looking like Vercel's design language). The book's argument is that ownership of DESIGN.md is the antidote to convergence.

**Key references:**
1. Frost, B. (2016). *Atomic Design*. https://atomicdesign.bradfrost.com/ — The foundational framework.
2. Design Tokens Community Group. (2025). Format Module 2025.10. https://www.designtokens.org/tr/drafts/format/ — The first stable industry standard.
3. Lupton, E. (2024). *Thinking with Type* (3rd ed.). Princeton Architectural Press. — The typography-as-system bridge.
4. Salesforce SLDS documentation. https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/tokens_intro.htm — The first major public design-system token implementation.
5. Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders. — The slide-specific design-philosophy lineage.

**Recent developments (last 3 years):**
- The W3C Design Tokens Community Group reached its first stable specification in October 2025, ending nearly a decade of competing vendor formats.
- Public design systems have proliferated; nearly every major tech company now publishes a design system with token specifications.
- AI-mediated design tooling (Figma AI, Anthropic-style design assistants, the Brutalist system itself) has made DESIGN.md-style specifications part of the working artifact for non-designers. The faculty audience this book targets is precisely the population for whom this is newly accessible.
- Brad Frost has continued to publish on atomic design and has launched online courses building on the book. The 2016 book is still the canonical text.

---

## E. Teaching considerations

**Where faculty get stuck:**
- *"I'm not a designer — I shouldn't have opinions about typography."* The chapter's pushback: every faculty member already has design opinions (they have rejected ten AI-generated decks); they have lacked the vocabulary to express them. The DESIGN.md is the artifact that captures the opinion in language the system can apply.
- *"This feels like over-engineering. I just want my slides to look fine."* Real concern. Mitigation: the DESIGN.md is a one-time cost amortized across years of slide production. The faculty member who spends two hours owning their DESIGN.md saves twenty hours of per-slide tweaking over a semester.
- *"What if my DESIGN.md is wrong?"* The chapter's move: any DESIGN.md is better than no DESIGN.md, and the file is meant to evolve. A first draft will reveal mistakes when the slides expose them; the DESIGN.md gets updated, the slides regenerate, the loop tightens. The error is not having a wrong DESIGN.md; it is treating the defaults as untouchable.

**Analogies and framings that work:**
- *The recipe vs. the menu.* The recipe (DESIGN.md) specifies the ingredients and the method. The menu (the deck) is what gets served. Update the recipe and every future meal changes. (Original framing.)
- *The newspaper style guide.* Already cited above. A working analogy because faculty have encountered style guides as authors.
- *The classroom syllabus.* The DESIGN.md is to a deck as the syllabus is to a course — the spec that makes the artifact possible. (Original framing.)
- *The constitution and the laws.* The DESIGN.md is the constitution; individual slide prompts are the laws. Laws must be consistent with the constitution; the constitution gets amended deliberately, not casually. (Original framing, perhaps too political — flag for review.)

**Exercises that build the target skill:**
- *Read your DESIGN.md aloud, line by line. For each variable, say why it has that value. Where you cannot, mark the line for examination.*
- *Find one Brutalist default you want to change. Write the change. Then write the one-sentence defense in framework vocabulary.*
- *Read another person's DESIGN.md (provide a sample). Identify three decisions you would make differently and articulate the disagreement in framework vocabulary, not aesthetic preference.*
- *Diagnostic questions for any DESIGN.md:*
  1. Can I explain every variable in my DESIGN.md in one sentence?
  2. Is each decision traceable to a principle from cognitive science or visual design?
  3. If I changed this variable, could I say why in framework vocabulary — not "I like it better"?
  4. Are my reference-slide conventions named separately from my teaching-slide conventions?
  5. When the system generated a slide I dislike, did I update DESIGN.md or did I tweak the slide?

---

## F. Library files relevant to this chapter

- `lecture-slides-deep-research.md` — Cross-reference for the cognitive science vocabulary the DESIGN.md decisions must trace to. Every variable in DESIGN.md needs a principled justification, and the principles live in this file.
- `pantry/brutalist/DESIGN.md` — **The reference implementation.** Read in full. The chapter's worked example is the reader producing their own DESIGN.md by accepting or departing from this one.
- `pantry/brutalist/CLAUDE.md`, `pantry/brutalist/PROJECT.md` — Adjacent system files; show how DESIGN.md sits within the larger Brutalist file structure.
- `_lib_EdTech.md` — May contain design-system commentary relevant to the prompting-as-design framing.
- `_lib_Surfaces-and-Essences.md` — Hofstadter on category-level vs. instance-level thinking is the deep cognitive layer under "token vs. instance." Useful if the chapter wants to gesture at why this distinction works.
- `_lib_Teaching-for-Deeper-Learning.md` — The integration-as-pedagogy move (Ch 11 integrates Ch 1–10) parallels the deeper-learning literature on consolidation. Useful for Section E framing.
- `D3a.md` — May contain notes on the D3/HTML production pipeline that ties DESIGN.md tokens to actual rendered slides. Confirm.

---

## G. Gaps and flags

- FLAG: Brad Frost's *Atomic Design* is available at atomicdesign.bradfrost.com — confirmed via search. The book is free online; print/ebook also available. URL: https://atomicdesign.bradfrost.com/. Confirm before citing in the chapter.
- FLAG: The W3C Design Tokens Community Group spec — first stable version dated October 28, 2025. URL: https://www.designtokens.org/tr/drafts/format/ (note: the spec is a community-group document, not a W3C Standard). Confirm the version-as-cited remains current at publication time.
- FLAG: Salesforce SLDS — there are now two versions (SLDS 1 and SLDS 2 introduced Spring '25). The chapter should cite SLDS as a historical example of design tokens at industrial scale and not anchor to a specific version that may shift.
- FLAG: Ellen Lupton *Thinking with Type* edition — the 3rd edition was published 2024. Earlier editions (2004, 2010) are also in wide circulation. Cite the edition the chapter uses consistently.
- GAP: There is no published peer-reviewed empirical study (that I can identify) on whether AI-mediated design systems with DESIGN.md-style specifications produce better outcomes than ad-hoc prompting. The chapter's claim that DESIGN.md ownership scales better than per-slide tweaking is currently a structural argument, not an empirical finding.
- GAP: No quantitative benchmark for "how much of a DESIGN.md should be specified vs. left to the model." The chapter must take a position (Brutalist defaults are heavily specified) without empirical backing for the specific level of specification.
- GAP: Frost's *Atomic Design* does not directly address AI-mediated workflows — the book predates the LLM era. The chapter is extending the framework into a context Frost did not write for; the extension is the chapter's contribution but is not citationally supported in Frost.
- GAP: The "prompting as design" framing is original to this chapter. There is no widely cited published treatment that names the move. The chapter can either claim the framing as its own contribution or find adjacent treatments in the prompt-engineering literature ([verify recent prompt-engineering reviews 2024–2026]).
