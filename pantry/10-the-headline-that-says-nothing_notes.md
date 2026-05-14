# Research Notes: Chapter 10 — The Headline That Says Nothing

**Source:** TIKTOC.md chapter entry
**Notes file:** 10-the-headline-that-says-nothing_notes.md
**Corresponding chapter:** chapters/10-the-headline-that-says-nothing.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns to identify topic-header + bullets slides that would be stronger as assertion-headline + visual evidence, and produces the rewrite.

**The feeling:** A slide that has a title like "Cognitive Load Theory" followed by five bullet points. It is correct. It is complete. It teaches nothing.

**The topic-header problem:** A topic header names the subject. It tells the student what the slide is about. It does not tell the student what to think about it. The student leaves knowing the topic was covered. They do not leave with a claim in their head.

**The assertion-evidence structure (Alley):** Headline is a complete sentence stating a claim. Body is visual evidence supporting it — not bullets.

**Why it works:** Garner & Alley (2013) found that slides with a full-sentence assertion headline + visual evidence produced higher retention than traditional topic-header + bullets on both immediate and delayed tests. The mechanism: the claim gives the student a schema to hang the evidence on before they see it.

**Prompt category:** Headline rewrite (label → claim) + visual form selection for the evidence.

**DESIGN.md variable:** Headline style convention — sentence or fragment, claim or label.

---

## A. Conceptual foundations

### Label vs. claim — the distinction the chapter turns on

A topic header names the subject of the slide. "The Calvin Cycle." "Methods." "Q3 Performance." "Cognitive Load Theory." It is a label — a noun phrase that tells the reader *what the slide is about* without telling them *what to think about it*. Labels are the default output of every slide tool that has ever existed. They are also the default output of AI slide generators (Gamma, Canva Magic Design, Beautiful.ai), which scan section headings in the source material and copy them onto slides as titles. A label costs the author nothing and teaches the student nothing.

An assertion is a complete sentence that makes a claim the slide will substantiate. "The Calvin Cycle fixes carbon in three stages, each requiring ATP and NADPH from the light reactions." "Q3 revenue grew 23%, driven entirely by enterprise renewals." "Working memory holds only four items — slide design must respect this limit." The assertion is the slide's point of view. It tells the student what conclusion to draw before they see the evidence, which means they encode the evidence into a schema rather than letting it float free. The headline does the work of orienting cognition before the body of the slide ever gets read.

The chapter's central diagnostic move is to make this distinction operational. The test: read only the slide title and nothing else. Can you say what the slide is claiming? If the answer is "I know what topic it's about but I don't know what it's saying about that topic," the slide has a label, not an assertion.

**Common misconception:** That assertion headlines must be long, complex sentences. They need not be. "Bullets are not the body." "Random color destroys signal." "The slideument fails as both products." Short complete sentences are stronger than long ones. The test is grammatical (is it a sentence?) and semantic (does it make a claim?), not length.

**Worked example:** A faculty lecture deck slide titled "Introduction" with five bullet points about the upcoming material is the canonical label case. The rewrite: "This lecture will show that working memory limits explain three failure modes in slide design." Now the student has the claim before the evidence. Every subsequent slide either builds toward that claim or extends it.

**Source(s):**
- Alley, M., & Neeley, K. A. (2005). Rethinking the design of presentation slides: A case for sentence headlines and visual evidence. *Technical Communication*, 52(4), 417–426. http://writing.engr.psu.edu/2005_alley_neeley.pdf
- Atkinson, C. (2008). *Beyond Bullet Points: Using Microsoft PowerPoint to Create Presentations That Inform, Motivate, and Inspire* (2nd ed.). Microsoft Press. https://www.cliffatkinson.com/beyond-bullet-points

### The assertion-evidence (AE) structure — Alley's framework

The assertion-evidence approach was developed by Michael Alley and colleagues at Penn State Engineering beginning in the early 2000s, with the canonical articulation in Alley & Neeley (2005) in *Technical Communication*. The structure has two rules. First, the slide headline is a single sentence stating the slide's main message — not a phrase, not a label, a complete declarative sentence. Second, the body of the slide is visual evidence supporting that headline — diagrams, photographs, equations, data graphics, annotated images — and crucially *not* a bulleted list of sub-points. Bullets are excluded because they fragment relationships into spatial adjacency and force the audience to reconstruct the connectives that the assertion was supposed to provide.

The structural logic is straightforward. The headline tells the audience what to look for. The visual evidence gives them what to look at. The audience's working memory is freed from the task of figuring out *what the slide is about* and can be spent on *the relationship the evidence demonstrates*. The structure is a direct application of Mayer's Multimedia Principle (words + relevant pictures > words alone) and Signaling Principle (use cues to direct attention), embedded into the slide template itself rather than left to per-slide authorial discretion.

Cliff Atkinson's *Beyond Bullet Points* (first edition 2005, third edition 2018) is the more popular treatment of essentially the same idea, framed for business presenters rather than engineers. Atkinson's "headline + image" structure and Alley's "assertion + visual evidence" structure are convergent — they were developed independently and arrive at the same prescription. The chapter should cite both lineages.

**Common misconception:** That AE is just "no bullets." The bullet ban is downstream of the assertion. A slide with an assertion headline and three short bullets *can* be AE-compliant if the bullets are visual-evidence text blocks (e.g., labeled comparisons) rather than fragmented prose. What AE forbids is the topic-header-plus-vertical-list-of-sentence-fragments structure that PowerPoint defaults to.

**Worked example:** Topic-header slide: "Mitochondrial Function" + five bullets ("Generates ATP," "Located in cytoplasm," "Has its own DNA," etc.). AE rewrite: "Mitochondria generate ATP through oxidative phosphorylation across the inner membrane" + an annotated cross-section diagram with labels for ATP synthase, the inner membrane, the proton gradient. The student sees the claim, then sees the mechanism the claim describes, and leaves with both.

**Source(s):**
- Alley, M., & Neeley, K. A. (2005). Rethinking the design of presentation slides: A case for sentence headlines and visual evidence. *Technical Communication*, 52(4), 417–426. http://writing.engr.psu.edu/2005_alley_neeley.pdf
- Atkinson, C. (2018). *Beyond Bullet Points* (3rd ed.). Microsoft Press.
- Assertion-Evidence Approach (project site). https://www.assertion-evidence.com/

### Why the assertion-evidence structure improves retention — the empirical record

Garner & Alley (2013) is the most cited empirical comparison. The study used 110 undergraduate engineering students, two parallel slide sets covering identical content (one in AE structure, one in the default topic + bullets structure), and measured comprehension via essay responses and recall on both immediate and delayed post-tests. The AE group showed superior comprehension, fewer misconceptions, lower self-reported cognitive load, and stronger delayed recall. The effect was statistically significant ([verify exact p-value and effect size]; the paper reports p < .01 on the main comprehension comparison).

The mechanism Garner & Alley propose follows from Mayer's CTML: by stating the assertion at the top, the slide pre-activates the schema the evidence will be integrated into. The student receives the claim, then the evidence, in the order working memory can actually use. The default topic-header structure inverts this: the student receives the topic label, then bullets that may or may not be the claim, and has to reconstruct the assertion from the body — extra cognitive work that comes out of the same finite budget.

Wolfe, Shanmugaraj, Reineke, Caton Peet, and Moreau (2024) extends this work with three pilot studies covering computer science, medical, and engineering student populations. The replication is broadly supportive: AE-structured slides outperform topic-bullet defaults on comprehension measures across populations, though the authors raise nuance about long quotations (verbatim reading of long quotes is worse than paraphrase, regardless of slide structure). This is the most recent peer-reviewed treatment as of late 2025 and is the right citation for "is this still holding up?"

The 2011 ASEE paper by Garner, Alley, Sawarynski, Wolfe, and Zappe ("Assertion-Evidence Slides Appear to Lead to Better Comprehension and Recall of More Complex Concepts") found the AE advantage was *largest* for complex conceptual material — exactly the case textbook lecture decks face.

**Common misconception:** That the AE evidence is preliminary. It is not. It is multi-site, multi-population, replicated, and the most recent 2024 replication continues to support it. The remaining open questions are about edge cases (when does the AE structure fail) and audience adaptation, not about whether the core effect exists.

**Worked example:** A faculty member runs the comparison in their own course. Same content, two sections, two slide formats. Even a small-N classroom comparison typically reproduces the comprehension delta. Garner & Alley's experimental design is replicable in a class of fifty without IRB-level apparatus — the chapter could suggest this as an end-of-chapter exercise.

**Source(s):**
- Garner, J. K., & Alley, M. P. (2013). How the design of presentation slides affects audience comprehension: A case for the assertion-evidence approach. *International Journal of Engineering Education*, 29(6), 1564–1579. https://writing.engr.psu.edu/ae_comprehension.pdf
- Garner, J. K., Alley, M., Sawarynski, L., Wolfe, K., & Zappe, S. (2011). Assertion-evidence slides appear to lead to better comprehension and recall of more complex concepts. *ASEE Annual Conference Proceedings*. https://peer.asee.org/assertion-evidence-slides-appear-to-lead-to-better-comprehension-and-recall-of-more-complex-concepts.pdf
- Wolfe, J., Shanmugaraj, N., Reineke, J., Caton Peet, L., & Moreau, C. P. (2024). Advancing the knowledge base on effective presentation slide design: Three pilot studies. *Journal of Business and Technical Communication*. https://journals.sagepub.com/doi/10.1177/00472816231169433

### Answer-first communication — Minto's pyramid and the journalism nut graf

The AE structure is one instance of a broader pattern that shows up in management consulting (the Minto Pyramid), in journalism (the nut graf), and in scientific writing (the abstract-first conclusion). Barbara Minto formalized the pattern at McKinsey in the 1970s in what became *The Pyramid Principle*: lead with the answer, then provide three supporting points, each backed by evidence. The cognitive logic is identical to Alley's. Decision-makers — and learners — process information faster when the conclusion is given first and the support follows, because they can evaluate each piece of evidence against the claim it supports as they encounter it.

In journalism, the nut graf is the paragraph following the lede that tells the reader *what the story is about and why it matters*. Chip Scanlan at the Poynter Institute is the most-cited explicator: "The nut graf tells the reader what the writer is up to; it delivers a promise of the story's content and message." Reporters who skip the nut graf produce stories that drift; readers who do not encounter a clear claim in the first three paragraphs typically stop reading. The slide title is the deck's nut graf at the slide level: state the claim, deliver the evidence, repeat.

Garr Reynolds, in *Presentation Zen*, gives this the colloquial name "What's your point?" — the question every slide must answer before the audience asks it. Reynolds' aesthetic prescription (simplicity, one idea per slide) is downstream of the same insight Alley operationalizes: the slide that does not announce its point makes the audience guess, and audiences are bad at guessing in real time during a lecture.

**Common misconception:** That answer-first communication suppresses argument or nuance. It does not. The pyramid structure makes the argument *more* legible: the claim is named, the supporting structure is visible, and a reader can immediately see which sub-claims they want to challenge. A buried claim is not a more sophisticated claim; it is a less defended one.

**Worked example:** A research talk slide titled "Results" with three graphs. The audience sees three graphs and a label and has to figure out which graph carries the central finding. AE rewrite: "Treatment reduced infection rates by 66% within three months, sustained at 18-month follow-up" + the single graph that shows this. The other two graphs become supporting slides, each with their own assertion.

**Source(s):**
- Minto, B. (2009). *The Pyramid Principle: Logic in Writing and Thinking* (3rd ed.). Pearson.
- Scanlan, C. (2003). "The nut graf, Part I." Poynter Institute. https://www.poynter.org/archive/2003/the-nut-graf-part-i/
- Reynolds, G. (2019). *Presentation Zen: Simple Ideas on Presentation Design and Delivery* (3rd ed.). New Riders.

### The reference-slide exception — when a label is the right headline

Not every slide makes a claim. A slide that lists definitions, a slide that displays a regulatory citation in full, a glossary slide, a recap-of-prior-week slide — these are *reference slides*, and a label is the correct headline for them. "Key Terms: Lesson 4." "WCAG 2.1 AA Contrast Ratios." "Today's Agenda." The slide is providing structured information for lookup, not arguing a point. Forcing an assertion onto a reference slide produces an awkward fiction. The diagnostic test: is the slide trying to *make the student think something new* (claim) or *give them something to look up* (reference)? Different jobs warrant different headline structures.

The book's recommendation: default to assertion headlines for teaching slides, label headlines for reference slides, and document the convention in DESIGN.md as an explicit decision rather than a per-slide judgment call. The DESIGN.md variable is not "claim or label" as a global setting — it is the rule that maps slide type to headline structure.

**Common misconception:** That the reference-slide exception swallows the rule. It does not. In a typical fifty-slide lecture deck, three to five slides are reference; forty-five are teaching. The default is the assertion. The exception is the label.

**Worked example:** A neuroscience lecture's closing slide titled "Key Terms" listing eight definitions is correctly a label. The lecture's twelfth slide titled "Action Potential" with a phase diagram is incorrectly a label — the assertion rewrite is "Action potentials fire only when membrane depolarization crosses threshold."

**Source(s):**
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.), ch. 5 ("Design").
- Alley, M. (2013). *The Craft of Scientific Presentations* (2nd ed.). Springer.

---

## B. Domain examples and cases

### Case 1: Penn State Engineering's institutional shift to AE

Penn State's College of Engineering has used the assertion-evidence structure as a teaching baseline in technical communication courses since approximately 2003, following Alley's introduction of the structure. The Engineering Ambassadors program — a public-speaking initiative for engineering undergraduates — adopted AE as its house style and reports the structure as one of its most teachable interventions. The institutional record is the strongest single piece of evidence that the structure scales: it has been taught to thousands of students over two decades, and its retention advantages have replicated across cohorts.

**Source:** Alley, M. (n.d.). "Engineering Ambassadors: Learning the Assertion-Evidence Approach." Penn State College of Engineering. http://writing.engr.psu.edu/assertion_evidence_EA.html

### Case 2: AI slide tools default to label headlines

Canva Magic Design, Gamma, Beautiful.ai, and tome.app generate slide titles by parsing section headings in the source material. The default output is "Market Analysis," "Q3 Performance," "Background," "Methods" — labels, not claims. The chapter should run this as a live demonstration: feed the same source material to three AI tools and show that all three produce label headlines, then show the AE rewrite the Brutalist system produces when prompted to. The pattern is consistent across tools because they share the same underlying assumption (the section heading is the slide title), and that assumption is precisely what AE rejects.

**Source:** Direct comparison; tool documentation. [verify with current tool outputs before publication — outputs change quarterly]

### Case 3: McKinsey's "answer-first" deck convention

McKinsey internal style — drilled into every consultant from the first week — is to lead each slide with a single declarative sentence that states the page's conclusion. The body is the data and reasoning supporting that conclusion. This is structurally identical to AE, developed independently in a non-academic context, refined over decades of client-facing pressure. The chapter can cite this convergence as evidence that the structure is robust across very different communication settings: engineering lectures and consulting decks arrive at the same prescription because both face the same constraint (audience working memory is the bottleneck).

**Source:** Minto, B. (2009). *The Pyramid Principle*. Pearson. See also: discussions in management consulting training materials, e.g., https://managementconsulted.com/pyramid-principle/

### Failure case: The "Introduction" slide that introduces nothing

The canonical failure case is the lecture deck's opening slide titled "Introduction" with three bullets that paraphrase the syllabus. The slide is structurally redundant (the syllabus already exists), tells the student nothing they did not know on the way in, and burns the most attention-rich moment of the lecture on a label. The AE rewrite at the opening slide is the single biggest leverage point in the deck: state the lecture's central claim in the first thirty seconds and the rest of the deck has somewhere to land.

The same failure shows up in scientific talks as the "Outline" slide that tells the audience "I will talk about X, Y, Z" and in business decks as the "Agenda" slide. All three are labels masquerading as orientation; all three could be replaced with an assertion that tells the audience *why* X, Y, and Z matter.

**Source:** Reynolds, G. (2019). *Presentation Zen* (3rd ed.), ch. 4. Alley, M. (2013). *The Craft of Scientific Presentations* (2nd ed.).

---

## C. Connections and dependencies

**Prerequisites (what reader must already know):**
- The slideument distinction (Ch 1): an AE slide is structurally a *live-delivery* slide; the assertion drives the speaker's narration, and the body is the visual evidence. AE without the live-async distinction can produce slides that work in delivery but fail as study artifacts.
- Text-density vocabulary (Ch 3): AE pushes most explanatory prose off the slide and into either the speaker's narration or the notes field. The reader needs Ch 3's diagnostic to know what to cut.
- Hierarchy (Ch 2): the assertion headline is the top of the hierarchy. Without size-hierarchy discipline, the headline does not visually dominate the body and the structure's effect is lost.
- Visual form selection (Ch 4): the body of an AE slide is *visual evidence*, which forces the form choice — text, diagram, chart, table — that Ch 4 teaches.

**Unlocks (what this chapter makes possible):**
- The deck-level rewrite move: once every slide has an assertion, the deck's structural arc becomes visible at a glance (read the headlines, get the argument).
- A DESIGN.md headline-style convention that downstream prompts can reference.
- Chapter 11's integration: the assertion-or-label decision is one of the variables Ch 11 asks the reader to defend in their DESIGN.md.

**Adjacent chapter connections:**
- Chapter 1 (Slideument): AE is the structural answer to "what should a live-delivery slide look like?" — the topic header is the slideument's default; the assertion is the live deck's default.
- Chapter 3 (Too Much Text): AE solves the "too much text" problem at the structural level by moving prose off the slide and into the speaker's voice.
- Chapter 4 (Wrong Visual Form): AE *requires* a visual form choice; the headline forces the question.
- Chapter 11 (Owning Your DESIGN.md): headline style is one of the variables this chapter operationalizes.
- Chapter 12 (Diagnostic Checklist): the assertion-or-label test is one of the checklist's most reliable triggers — fast to apply, hard to fake.

---

## D. Current state of the field

**Settled:**
- AE-structured slides produce higher comprehension and recall than topic-header + bullets slides in engineering, computer science, and medical student populations (Garner & Alley 2013; Garner et al. 2011; Wolfe et al. 2024).
- The mechanism is consistent with Mayer's CTML — pre-activating a schema before evidence improves integration (Mayer 2009, 2020).
- The answer-first pattern is independently confirmed in management consulting (Minto), journalism (the nut graf), and scientific writing (structured abstracts).

**Contested or emerging:**
- *How strictly to enforce "no bullets" in AE.* Alley's strictest version excludes all bulleted lists from the body. Atkinson's *Beyond Bullet Points* is less doctrinaire about bullets per se and more focused on the headline structure. Wolfe et al. (2024) does not test the bullets-vs-no-bullets question in isolation. The book can take a position: ban bullets when the relationship is non-list (most cases), allow them when the content is genuinely enumerative (rare).
- *Whether the AE advantage holds for asynchronous study artifacts as well as live delivery.* The empirical work has been on live or recorded-lecture conditions. The async case (slide must teach without speaker) plausibly benefits more from assertion headlines, but the experimental record is thinner.
- *Whether AI-generated slides can be evaluated against AE structure in a way that produces a reliable diagnostic.* No published empirical study on this as of late 2025 — this is a research gap and a teaching opportunity.

**Key references:**
1. Alley, M., & Neeley, K. A. (2005). Rethinking the design of presentation slides. *Technical Communication*, 52(4), 417–426. — The foundational paper.
2. Garner, J. K., & Alley, M. P. (2013). How the design of presentation slides affects audience comprehension. *International Journal of Engineering Education*, 29(6), 1564–1579. — The most-cited empirical comparison.
3. Atkinson, C. (2018). *Beyond Bullet Points* (3rd ed.). Microsoft Press. — The popular treatment; convergent independent development.
4. Wolfe, J., et al. (2024). Advancing the knowledge base on effective presentation slide design: Three pilot studies. *Journal of Business and Technical Communication*. — The most recent replication.
5. Minto, B. (2009). *The Pyramid Principle* (3rd ed.). Pearson. — The cross-domain convergence on answer-first.

**Recent developments (last 3 years):**
- Wolfe et al. (2024) is the most recent peer-reviewed replication; the AE advantage continues to hold in three new studies across populations.
- AI slide tools (Gamma, Canva Magic, Beautiful.ai, tome.app, Microsoft Copilot in PowerPoint) have proliferated since 2023 and default to label headlines almost universally. No empirical comparison of AI-generated vs. human-AE slides yet exists. [verify]
- The Design Tokens Community Group W3C specification (first stable version October 2025) does not yet contain a "slide headline style" token type, but the modular structure suggests one could be added — relevant for Ch 11 more than Ch 10.

**Holds in 2026?** Yes — and stronger than in 2013. The Wolfe et al. 2024 replication across CS, medical, and engineering populations directly addresses the most reasonable challenge (was the original effect engineering-specific?). The answer is no — it generalizes. The remaining open questions are about edge cases and tool-mediated variation, not about whether the core effect exists.

---

## E. Teaching considerations

**Where faculty get stuck:**
- *"My slide titles are short and clean — assertions will look cluttered."* Real concern: a full sentence is visually heavier than a noun phrase. Mitigation: the AE assertion does not have to be long, and the body is *less* cluttered (no bullets, just a clean visual). The total slide is cleaner, not denser.
- *"I don't always have a claim — sometimes I'm just covering material."* The diagnostic move: if you are "just covering material," ask whether the slide is teaching anything. A slide that is not teaching anything should probably not be in the deck. Reference slides aside (the legitimate exception), every teaching slide has a claim — the faculty member just hasn't articulated it yet.
- *"This feels like business-presentation style, not academic teaching."* The empirical record is on academic teaching (Penn State Engineering, Wolfe et al. medical/CS/engineering students). The style originated in academic contexts. The objection is aesthetic, not evidential.

**Analogies and framings that work:**
- *Headline vs. dateline.* A newspaper headline makes a claim ("Senate rejects funding bill"); a dateline labels a location ("Washington, D.C."). The label is correct for what it does; it is not the headline. Slide titles should be headlines, not datelines. (Original framing.)
- *The summary sentence.* If a student described this slide to a friend in one sentence, what would they say? That sentence is the assertion. If they cannot summarize the slide in a sentence, the slide does not know what it is claiming. (Adaptation of Alley.)
- *The nut graf.* Already in the chapter from Section A. Use it.

**Exercises that build the target skill:**
- *Before/after (the book's standard).* Take a university lecture slide titled "Methods" or "Introduction" and rewrite the headline as the slide's actual claim. Pair with the visual evidence rewrite — replace bullets with a diagram, image, or annotated chart.
- *The "summarize in one sentence" drill.* For each slide in the reader's most recent deck, write a one-sentence summary. Compare to the slide's current title. The gap is the rewrite.
- *Diagnostic questions for any slide:*
  1. Is the headline a claim or a label?
  2. Could a student leave this slide with a specific thought in their head?
  3. Does the body provide visual evidence for the headline's claim?
  4. Would replacing the bullets with one image make this clearer?
  5. Is this slide teaching, or is it a reference slide where a label is correct?

---

## F. Library files relevant to this chapter

- `lecture-slides-deep-research.md` — **Primary cross-reference.** The sections on Mayer's Multimedia Learning Principles (especially Signaling, Multimedia, Coherence) and on Alley's assertion-evidence model feed this chapter directly. The Garner & Alley citation should appear there; if not, add.
- `_lib_How-to-Deliver-a-TED-Talk.md` — Gallo's treatment of "the one-line message" is the popular-press version of the AE assertion. Useful for the "What's your point?" framing.
- `_lib_EdTech.md` — Possibly contains AI slide tool comparisons useful for the failure-case section.
- `_lib_Teaching-for-Deeper-Learning.md` — Cognitive science backing for the schema-pre-activation mechanism.
- `_lib_Surfaces-and-Essences.md` — Hofstadter & Sander on analogy and core/peripheral concepts is the deepest theoretical layer under "what is the slide's central claim?" — relevant if the chapter wants to go one level deeper than Alley.

---

## G. Gaps and flags

- FLAG: The Garner & Alley (2013) effect sizes — I cited "p < .01" on the main comparison from secondary summaries. Pull the original PDF (https://writing.engr.psu.edu/ae_comprehension.pdf) and verify the exact statistical reporting (effect size, CI, n per group) before quoting numbers in the chapter draft.
- FLAG: The Wolfe et al. (2024) DOI and exact pagination — I cited the SAGE journal link but the issue number and final pagination should be confirmed against the published version. The DOI prefix is 10.1177/00472816231169433.
- FLAG: Alley & Neeley (2005) pagination — I cited 417–426 from common citations; confirm against the *Technical Communication* original. The Penn State writing.engr.psu.edu hosts the PDF.
- FLAG: Atkinson's *Beyond Bullet Points* edition — there are three editions (2005, 2008/11, 2018). The 2018 third edition (subtitled "Using PowerPoint to tell a compelling story that gets results") is the most current; chapter should cite the edition it uses consistently.
- GAP: No published empirical comparison of AI-slide-tool-generated headlines (Gamma, Canva, Beautiful.ai) measured against AE structure. The chapter's claim that AI tools default to labels is currently a structural observation, not a peer-reviewed finding. Author can run the comparison themselves and document it — this might be a strong original contribution.
- GAP: The reference-slide exception is treated in the chapter spec but I have not found a published source that formalizes it. Alley's work concentrates on teaching slides; the reference-slide case is implicit. The chapter may need to claim this distinction as its own contribution.
- GAP: No quantitative benchmark for "how long should an assertion headline be?" Practitioners' rules of thumb vary from "one line" to "two lines max." The chapter may need to set a Brutalist convention.
