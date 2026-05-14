# Research Notes: Chapter 01 — The Slideument Problem

**Source:** TIKTOC.md chapter entry
**Notes file:** 01-the-slideument-problem_notes.md
**Corresponding chapter:** chapters/01-the-slideument-problem.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns to see the difference between a slide (a visual anchor for a speaker) and a document (a self-contained artifact), and why a deck that tries to be both fails at both.

**The feeling:** A deck that looks complete — full sentences, everything explained — but is somehow exhausting to look at during a lecture and useless to study from afterward.

**Cognitive science failure:** Redundancy principle violation. The slide contains the full verbal explanation the speaker is also delivering. The verbal channel is overloaded. The student reads instead of listens.

**Visual design failure:** Reynolds' slideument. The deck has no point of view about what it is for.

**Prompt category:** Text density reduction + notes field population.

**DESIGN.md variable:** Body text density defaults; notes field conventions.

**Bridge:** A slide can have too much text for a different reason than slideument failure — sometimes the hierarchy just isn't clear enough to show the reader what matters. That's Chapter 2.

---

## A. Conceptual foundations

### The slideument — Reynolds' coinage and what it actually names

The term "slideument" (sometimes "slide-u-ment") is Garr Reynolds' contraction of "slide" and "document," introduced on his Presentation Zen blog in the mid-2000s and elaborated in *Presentation Zen* (Reynolds, 2008, 2nd ed. 2011, 3rd ed. 2019). Reynolds' diagnostic is structural: a slideument is a deck whose author cannot decide whether they are designing visual support for a live talk or a written handout that stands alone, and so produces an artifact that tries to do both and fails at both. The slide is too dense to support live narration (the audience reads instead of listens) and too fragmented to function as a study document (the prose is incomplete because the speaker was supposed to fill the gaps).

The slideument is not a synonym for "too much text." It is a category mistake about what the artifact is *for*. A 200-word, prose-heavy slide that is honestly a handout — and is delivered as a handout, with no live narration competing — is not a slideument. A 30-word slide that mirrors the speaker's spoken words is. The diagnostic is about purpose, not word count.

Reynolds' frame inherits directly from a practical observation he attributes to communications consultants in Japan: handouts have a job, and slides have a different job, and combining them produces a worse handout and a worse slide. The economic argument: if you need both, build both. The pedagogical argument: a deck without a point of view about its use cannot serve any use well.

**Common misconception:** That a slideument is just a "wordy slide." Faculty assume reducing text fixes it. Reducing text without deciding what the deck is *for* produces a different bad deck — sparse slides that still don't function as a study artifact and still don't anchor a live talk.

**Worked example:** A title slide reading "Mitochondrial Function in Aerobic Respiration" followed by a single sub-bullet "Generates ATP through oxidative phosphorylation" is not a slideument — it is the title slide of a live deck. The same content rendered as a 90-word paragraph explaining the ATP-generation pathway *while the lecturer reads it aloud* is the slideument case: the verbal channel is doubled, and the slide is too compressed to function later as a study handout for someone who missed class.

**Source(s):**
- Reynolds, G. (2008/2011/2019). *Presentation Zen: Simple Ideas on Presentation Design and Delivery*. New Riders. https://www.presentationzen.com/
- Reynolds, G. "The 'Slideument' Is Not Working." Presentation Zen blog. https://www.presentationzen.com/presentationzen/2005/09/the_slideument_.html

### The Redundancy Principle — why on-screen text + identical narration hurts

Richard Mayer's Redundancy Principle, formulated within his Cognitive Theory of Multimedia Learning, states that learners perform worse when the same words are presented as both on-screen text and spoken narration than when they are presented as narration alone (paired with relevant visuals). The mechanism, derived from Sweller's Cognitive Load Theory and Baddeley's working memory model, is verbal-channel overload: text and speech compete for the same phonological-loop bandwidth, and the learner ends up suppressing one or the other — usually attending to the slide and ignoring the speaker.

The principle is established in Mayer's *Multimedia Learning* (2009, 2nd ed.; 3rd ed. 2020) and in the meta-analytic review by Mayer & Fiorella (2014). Importantly, the principle is *not* "no text on slides." It is "no text that duplicates narration when narration is also present." Short labels, key terms, equations, and on-screen names that the speaker references but does not read verbatim are not redundancy violations — they are scaffolding for the visual channel.

The slideument fails the Redundancy Principle as a structural matter. By design, the slideument contains the explanation the speaker also delivers, because the slide is trying to be a document. That is precisely the configuration Mayer's experiments show degrades learning.

**Common misconception:** That bullet points are inherently a redundancy violation. They are not. A bullet that names a step in a process the speaker is about to explain is signaling. A bullet that *is* the explanation the speaker is reading is redundancy.

**Worked example:** Speaker says "Oxidative phosphorylation uses the proton gradient across the inner membrane to drive ATP synthase." Slide shows a labeled diagram of the inner membrane with "ATP synthase" called out — not a redundancy violation. Slide shows the same sentence the speaker just said — redundancy violation.

**Source(s):**
- Mayer, R.E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press.
- Mayer, R.E., & Fiorella, L. (2014). Principles for reducing extraneous processing in multimedia learning: Coherence, signaling, redundancy, spatial contiguity, and temporal contiguity principles. In R.E. Mayer (Ed.), *The Cambridge Handbook of Multimedia Learning* (2nd ed., pp. 279–315). Cambridge University Press.
- Mayer, R.E., & Johnson, C.I. (2008). Revising the redundancy principle in multimedia learning. *Journal of Educational Psychology*, 100(2), 380–386. https://doi.org/10.1037/0022-0663.100.2.380

### Two artifacts, one deck — the use-case bifurcation

A useful diagnostic is to force the question: who reads this deck, when, and with what accompanying signal? Live-delivery slides exist while the speaker is in the room; the speaker carries the explanation, and the slide carries the anchor. Async/study slides exist after the lecturer is gone; the slide must carry the explanation because no speaker is available. The first deck wants minimal text and high visual dominance; the second deck wants prose density and self-contained captions. These are different products that happen to share a file format.

The slideument is the false economy of trying to ship one deck for both jobs. Faculty default to it because making two decks feels redundant. The book's move is to name the slideument as the worse outcome — not the efficient compromise — and to provide a structural fix: either choose one use case and design for it, or commit to two artifacts (using the notes field to hold what the slide cannot, or recording the lecture so the live deck can stay sparse).

**Common misconception:** That the "notes field" is for the speaker's script and nothing else. The notes field is the deck's second product. Populated fully, the live deck becomes a study artifact without redesign. Empty, it forces the slide itself to do both jobs — the slideument.

**Worked example:** Live-mode slide: large diagram of the citric acid cycle, six labels, no prose. Notes field below: 80-word explanation tying each step to the spoken narration. Async export: slide + notes panel printed together. Same source, two artifacts, neither fails.

**Source(s):**
- Reynolds, G. (2008). *Presentation Zen*, ch. 2 ("Preparation").
- Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.), chapter on the Modality Principle.

### Tufte and the analytical critique — different vocabulary, related diagnosis

Edward Tufte's *The Cognitive Style of PowerPoint* (2003, expanded 2006) is the most-cited critique of slide-based instruction. Tufte's argument is that PowerPoint's defaults — hierarchical bullet outlines, low information density per slide, decorative templates — fragment analytical reasoning by forcing complex arguments into shallow lists. He documents the case (see Domain Examples below) of the NASA Columbia engineering slide as evidence that the format itself contributed to a fatal communication failure.

Tufte's critique overlaps with Reynolds' slideument frame at the diagnosis (the medium produces a hybrid that serves no purpose well) but diverges at the prescription. Tufte recommends replacing slides with high-density technical handouts (his famous "use sentences" advice). Reynolds recommends separating the live deck and the handout into distinct artifacts. Both are defensible; the book takes the Reynolds path because it preserves the live-delivery medium and because the Brutalist system makes the two-artifact solution cheap.

**Common misconception:** That Tufte's critique means "bullets are bad." Tufte's critique is more structural: the *format* of the bullet outline encourages writers to elide logical connectives ("because," "therefore," "in contrast to") and reduces relational reasoning to spatial adjacency. A deck with no bullets can still commit the analytical sins Tufte names. A deck with bullets that names connectives explicitly does not.

**Worked example:** Tufte's preferred form is a one-page technical handout. The slideument is a deck that pretends to be that handout while also pretending to be slides. The book's preferred form is a sparse live deck plus a populated notes field that, exported, gives the reader the handout Tufte wants.

**Source(s):**
- Tufte, E.R. (2003, rev. 2006). *The Cognitive Style of PowerPoint: Pitching Out Corrupts Within*. Graphics Press. https://www.edwardtufte.com/tufte/powerpoint
- Tufte, E.R. (2003, September). "PowerPoint Is Evil." *Wired*, 11.09. https://www.wired.com/2003/09/ppt2/

---

## B. Domain examples and cases

### Case 1: The NASA Columbia accident slide (Tufte's canonical exhibit)

In the 2003 investigation of the Columbia space shuttle disaster, the Columbia Accident Investigation Board (CAIB) cited specific Boeing engineering slides as a contributing factor to the communication failure that left NASA management underweighting the foam-strike risk. The slide in question buried the critical finding — that the foam strike was outside the test database by orders of magnitude — under nested bullet hierarchies in small type. Tufte analyzed this slide in detail in *The Cognitive Style of PowerPoint* and argued the format itself obscured the engineering judgment.

The Columbia case is the most-cited real-world failure of slide design at high stakes. It functions in the chapter as the proof that "this deck doesn't feel right" can scale to "this deck killed people," and that the slideument hybrid is not stylistic preference but a documented communication failure mode.

**Source:** Columbia Accident Investigation Board. (2003). *Report Volume 1*, ch. 6, p. 191. https://www.nasa.gov/columbia/home/CAIB_Vol1.html
Also: Tufte (2003), *The Cognitive Style of PowerPoint*, pp. 8–12.

### Case 2: Edward Tufte's "Use Sentences" comparison (sparseness vs. argument)

In the *Wired* essay and the booklet, Tufte presents side-by-side examples of a bulleted slide vs. a one-paragraph written argument carrying the same content. The bulleted version omits the connectives ("therefore," "but only when," "in contrast to") that carry the analytical work. The paragraph form is denser but argumentatively stronger. Faculty can run this comparison on their own slides: write the slide's content as a paragraph. If the paragraph is stronger as an argument, the slide is doing the wrong job.

**Source:** Tufte, *Wired* (2003) and *Cognitive Style of PowerPoint* (2006 ed.).

### Failure case: Garner & Alley on bullet-format retention

Garner and Alley (2013) ran a comparison of traditional topic-header + bullets slides against assertion-headline + visual evidence slides in undergraduate engineering contexts. The bulleted format produced significantly lower retention on both immediate and delayed tests. The mechanism: bullets give the student no claim to hang the evidence on, so the evidence floats free and is not encoded into a usable schema. The study is the most often-cited empirical comparison of slide formats and supports the book's later move toward assertion-evidence (Ch 10) but is grounded in Ch 1 by demonstrating that *what a slide is for* shapes whether it teaches.

**Source:** Garner, J.K., & Alley, M. (2013). How the design of presentation slides affects audience comprehension: A case for the assertion-evidence approach. *International Journal of Engineering Education*, 29(6), 1564–1579.

---

## C. Connections and dependencies

**Prerequisites (what reader must already know):**
- That they have an AI-generated deck in front of them — the book's entry point assumption.
- That they recognize "this slide feels wrong" as a real signal worth diagnosing.
- Familiarity with the Brutalist system's notes-field convention (covered in Appendix A).

**Unlocks (what this chapter makes possible):**
- The diagnostic move "what is this deck for?" — used in every subsequent chapter.
- The notes-field-as-second-artifact frame — recurs in Chapter 9 (live vs. async).
- The Redundancy Principle vocabulary — used in Chapter 3 on text density and Chapter 10 on headlines.

**Adjacent chapter connections:**
- Chapter 2 (No Clear Hierarchy): Per TIKTOC.md bridge, "A slide can have too much text for a different reason than slideument failure — sometimes the hierarchy just isn't clear enough to show the reader what matters."
- Chapter 3 (Too Much Text): Slideument failure is type-1 of three text-density failure modes (the redundancy case). Chapter 3 generalizes the diagnosis.
- Chapter 9 (Live Deck vs. Study Artifact): The full deck-level treatment of the use-case bifurcation introduced here at the slide level.

---

## D. Current state of the field

**Settled:**
- Working memory has limited capacity; on-screen text identical to narration overloads the verbal channel — Sweller (1988), Mayer (2009, 2020). Replicated across hundreds of studies.
- Slides designed for live delivery are different products from slides used as study artifacts — Reynolds (2008), Duarte (2008).
- The bullet-outline default in slide software encourages structural decisions that obscure analytical reasoning — Tufte (2003), Kosslyn (2007).

**Contested or emerging:**
- *Whether bullets are inherently harmful or merely overused.* Tufte argues the format itself is corrosive; Kosslyn (2007) and Mayer treat bullets as one tool among many, fine when their hierarchy matches the content's hierarchy. Reynolds is closer to Tufte on aesthetics but more pragmatic on use. The book sides with the pragmatic camp.
- *Whether the slideument is solvable inside one file via populated notes fields or requires genuine two-artifact production.* Reynolds endorses notes-field solutions; Tufte argues only a separate technical document does the job. The book takes the notes-field path as default and the two-artifact path as fallback.

**Key references:**
1. Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders. — The slideument coinage and the philosophical frame for the chapter.
2. Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.). Cambridge University Press. — Redundancy Principle, full empirical backing.
3. Tufte, E.R. (2006). *The Cognitive Style of PowerPoint* (2nd ed.). Graphics Press. — The analytical critique and the Columbia case.
4. Mayer, R.E., & Johnson, C.I. (2008). Revising the redundancy principle in multimedia learning. *Journal of Educational Psychology*, 100(2), 380–386. — Refinement showing when redundancy hurts and when short on-screen labels help.
5. Columbia Accident Investigation Board. (2003). *Report Volume 1*. NASA. — The canonical real-world failure case.

**Recent developments (last 3 years):**
- AI slide tools (Gamma, Beautiful.ai, Canva Magic Design, tome.app) have made the slideument failure mode worse by default. Their generation pipelines treat the slide as a self-contained document and produce prose-heavy bullets that mirror what a speaker would say — the slideument configuration at scale. [verify] There is industry commentary (Gamma's own product blog, Beautiful.ai's documentation) but I am not aware of peer-reviewed empirical study yet on AI-slide-tool outputs measured against Mayer's principles. This is a flagged gap.
- The post-COVID normalization of hybrid teaching (live + recorded + async access to slides) has made the use-case bifurcation a daily problem rather than an edge case. The chapter should acknowledge this.

---

## E. Teaching considerations

**Where faculty get stuck:**
- *"But students need to be able to study from the slides."* This is the central faculty objection. The chapter must address it head-on rather than dismiss it. The move is to redirect: yes, students need study materials, and the slideument is the worst way to provide them. Notes field, separate handout, or recorded lecture are all better paths.
- *"I can't reduce text — the content is the content."* This conflates "the content" with "the prose currently rendering the content." The chapter must demonstrate that the prose is a *delivery choice*, not the content itself. The same content can be a diagram, a labeled image, a short prompt, or a paragraph in the notes field.
- *"My department/students expect prose slides."* Real institutional pressure. The chapter acknowledges this and offers the two-artifact compromise (sparse live deck + populated notes export) as the diplomatic path.

**Analogies and framings that work:**
- *Recipe vs. cookbook.* The recipe card on the counter while you cook is the slide. The cookbook on the shelf you study from later is the document. A laminated cookbook tied to your wrist while you cook is the slideument. (Original framing for the book.)
- *Stage directions vs. play script.* Stage directions tell the actor where to stand (slide as anchor); the play script contains the lines (document as artifact). A stage with the script projected on the back wall while the actor recites it is the slideument. (Original framing.)
- Reynolds' own: *"Slides are slides, documents are documents."* Use as the chapter's mantra but unpack the mechanism behind it.

**Exercises that build the target skill:**
- *Before/after pair (the book's standard).* Take a Brutalist-generated chapter-intro slide. Identify the redundancy. Run the prompt "Reduce this slide to a single diagram with three labels. Move the prose explanation to the notes field." Compare.
- Diagnostic questions for any slide:
  1. Is this deck designed for live delivery, async study, or both?
  2. If both: what specifically fails in each context?
  3. Is the notes field doing the work the slide shouldn't?
  4. If I removed the speaker, would the slide alone teach this content?
  5. If I removed the slide, would my narration alone teach this content?

---

## F. Library files relevant to this chapter

- `lecture-slides-deep-research.md` — **Primary cross-reference.** Sections on Cognitive Load Theory (Sweller), Mayer's 15 principles (particularly Redundancy, Modality, Coherence), and the live-vs-async distinction (the table at lines ~228–237) all feed this chapter directly. The Reynolds/Tufte distinction and the slideument coinage live here.
- `_lib_EdTech.md` (plausibly) — May contain practitioner-facing commentary on slide tools and instructional design integration. Useful for the AI-slide-tool failure-mode section.
- `_lib_How-to-Deliver-a-TED-Talk.md` (plausibly) — Carmine Gallo's treatment may include slide-density rules and the speaker-not-the-slide rule. Plausible cross-reference for the Reynolds aesthetic frame.
- `_lib_Teaching-for-Deeper-Learning.md` (plausibly) — Likely covers retrieval practice and the live/async distinction in instructional terms. Useful for the "what is the deck for" framing in Section E.
- `_lib_The-Digital-Delusion-Horvath.md` (plausibly) — May contain critique of tech-mediated instruction; relevant if the chapter wants a contemporary skeptical voice.
- `_lib_Surfaces-and-Essences.md`, `_lib_Thinking-Fast-and-Slow.md`, `_lib_Building-Thinking-Classrooms.md` — less directly relevant for Ch 1, but Kahneman's System 1/System 2 framing could surface as an analogy for "the slide does the fast work; the speaker does the slow work."

---

## G. Gaps and flags

- FLAG: I have not located peer-reviewed empirical study of AI-slide-tool outputs (Gamma, Beautiful.ai, Canva Magic Design) measured against Mayer's principles. Industry blogs and tool documentation exist; rigorous comparison studies may not yet. Author should `[verify]` any specific empirical claim here.
- FLAG: Reynolds' original "slideument" blog post date — I cited September 2005 above (https://www.presentationzen.com/presentationzen/2005/09/the_slideument_.html). Confirm the URL resolves and the date is correct before citing in the chapter.
- FLAG: The CAIB *Report Volume 1* page reference for the Boeing slide critique — I cited p. 191 from common citations; confirm against the official PDF. Tufte's analysis of the same slide is in *The Cognitive Style of PowerPoint*, 2nd ed., pages roughly 8–12 — confirm exact pagination.
- FLAG: Garner & Alley (2013) — I cited the *International Journal of Engineering Education* publication. There is also a related Garner & Alley working paper / earlier study from Alley's Penn State group (e.g., Alley & Neeley 2005); make sure the chapter cites the right one when it pulls retention numbers.
- GAP: No quantitative benchmark for "how much populated notes field is enough to make the live deck studyable." Reynolds, Mayer, Duarte all endorse the notes-field path but none specify a target density. The chapter may need to set a Brutalist convention rather than cite one.
- GAP: There is no direct empirical study (that I can name) testing the *specific* hypothesis that decks generated by AI tools fail Mayer's principles at higher rates than human-authored decks. This is the natural empirical claim of the book and is currently a flag, not a citation.
