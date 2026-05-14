# Research Notes: Chapter 03 — Too Much Text

**Source:** TIKTOC.md chapter entry
**Notes file:** 03-too-much-text_notes.md
**Corresponding chapter:** chapters/03-too-much-text.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns to distinguish load-bearing text from seductive text from slideument text — three different reasons a slide has too much on it, each requiring a different prompt.

**The feeling:** A slide that looks like a page. The reader starts reading and loses the thread of what the speaker is saying.

**Cognitive science failure (type 1 — redundancy):** Text repeats what the speaker is saying. Verbal channel overloaded. Slideument failure from Ch 1 at the slide level.

**Cognitive science failure (type 2 — seductive detail):** Interesting but not essential. Coherence principle violated.

**Cognitive science failure (type 3 — density):** All essential but presented at once. Working memory saturated. Segmenting principle applies.

**The test:** For each text element — which learning objective does this serve?

**The benchmark:** ~30–50 words per slide for live delivery. >75 words is a document, not a slide.

**Prompt category:** Text reduction + assertion extraction.

**DESIGN.md variable:** Maximum words per slide (a convention the reader sets).

**Bridge:** Sometimes the text is right but the visual form is wrong. That is Chapter 4.

---

## A. Conceptual foundations

### The three failure modes of "too much text" — a diagnostic taxonomy

The chapter's central move is that "too much text" is not one problem but three, each with a different mechanism and a different fix. The taxonomy is the chapter's structural contribution; faculty who recognize only "too much text" cannot prompt precisely because their diagnosis is at the wrong resolution.

*Type 1 — Redundancy.* The text on the slide duplicates what the speaker is saying. Mayer's Redundancy Principle, established in *Multimedia Learning* (2009, 2020) and the Mayer & Johnson (2008) study, predicts (and many experiments confirm) that this configuration produces worse learning than narration with relevant images alone. The mechanism is verbal-channel overload: speech and on-screen text both route through Baddeley's phonological loop, and the learner cannot process both simultaneously. The fix is not "less text"; it is "different text" — labels, anchors, headlines, terms that complement rather than duplicate narration.

*Type 2 — Seductive detail.* The text is interesting but not essential to the learning objective. The Coherence Principle (Mayer) and the seductive-details effect (Harp & Mayer, 1997, 1998; meta-analyzed by Rey, 2012) predict that such content harms retention. The mechanism is schema diversion: students form mental models around the interesting material and fail to integrate the core content. The fix is removal — not reformatting.

*Type 3 — Density.* The text is all essential, but it is presented in a single working-memory load. The Segmenting Principle (Mayer; Mayer & Pilegard, 2014) and the split-attention effect (Sweller, Tindall-Ford, Chandler, 1997) predict that essential content presented all at once is processed worse than the same content revealed in sequence or chunked into smaller units. The fix is segmentation — split the slide into two or three, or progressively reveal.

The diagnostic test for which failure mode applies: ask "what would happen if I deleted this text element?" If the speaker's narration becomes incoherent — load-bearing. If the slide is missing a flourish but the lesson is intact — seductive. If the slide still has all the necessary content but is overwhelming — density.

**Common misconception:** That word count alone diagnoses the failure. A 30-word slide can be a Type-1 redundancy violation (the 30 words are the speaker's script). A 30-word slide can be a Type-2 seductive-detail violation (the 30 words are a fascinating but irrelevant anecdote). A 100-word slide can be perfectly fine as a study-artifact deck. Word count is a downstream indicator; the diagnosis is about *function*.

**Worked example:** Slide reads "The mitochondrion generates ATP through oxidative phosphorylation, a process discovered by Peter Mitchell in 1961 and recognized with the 1978 Nobel Prize." If the speaker is delivering a lecture on cellular respiration, the Mitchell-and-Nobel detail is a Type-2 seductive-detail violation — interesting, not essential. Cut, or move to notes.

**Source(s):**
- Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.). Cambridge University Press.
- Mayer, R.E., & Johnson, C.I. (2008). Revising the redundancy principle in multimedia learning. *Journal of Educational Psychology*, 100(2), 380–386.
- Harp, S.F., & Mayer, R.E. (1998). How seductive details do their damage: A theory of cognitive interest in science learning. *Journal of Educational Psychology*, 90(3), 414–434. https://doi.org/10.1037/0022-0663.90.3.414
- Rey, G.D. (2012). A review and a meta-analysis of the seductive details effect. *Educational Research Review*, 7(3), 216–237.
- Mayer, R.E., & Pilegard, C. (2014). Principles for managing essential processing in multimedia learning: Segmenting, pre-training, and modality principles. In *The Cambridge Handbook of Multimedia Learning* (2nd ed.).

### The Coherence Principle — less is more, with evidence

Mayer's Coherence Principle states that people learn better when extraneous material is excluded rather than included. It is the most counterintuitive of his principles for faculty, who tend to assume that adding interesting context aids learning. The empirical record runs the other way: across many experiments, students who received the stripped-down lesson outperformed students who received the lesson plus extras (anecdotes, decorative images, background music, related-but-not-essential facts).

Harp and Mayer's six experiments on seductive details (1997, 1998) found that students receiving a lightning-formation lesson *with* added entertaining anecdotes and dramatic photos recalled structurally important content at roughly one-third the rate of students who received the lesson without those additions. Rey's 2012 meta-analysis confirmed small-to-medium negative effects on both retention and transfer across text-based and multimedia studies.

The effect is strongest when seductive details appear early in instruction, when students have low prior knowledge, and when intrinsic load is already high. This combination is precisely the configuration of most introductory undergraduate lecture decks. The chapter must make this argument because the faculty intuition — "I'll add a fun fact to warm up the room" — is, on the evidence, damaging.

**Common misconception:** That removing interesting content makes the lecture boring and disengages students. The research distinguishes engagement (in-the-moment interest) from learning (retention and transfer). Seductive details can increase engagement and reduce learning simultaneously. The book's position: engagement that costs comprehension is a net loss.

**Worked example:** A slide on the 2008 financial crisis with a sidebar headed "Did you know? Lehman Brothers was founded in 1850 by Bavarian immigrants." That sidebar is the seductive detail. Cut it. The students who would have found it interesting will encode it instead of the structural argument about MBS leverage.

**Source(s):**
- Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.). Cambridge University Press, chapters on Coherence.
- Harp & Mayer (1998), as above.
- Rey, G.D. (2012). A review and a meta-analysis of the seductive details effect. *Educational Research Review*, 7(3), 216–237.

### The Modality Principle and the split-attention effect

The Modality Principle states that students learn more deeply from spoken narration paired with on-screen graphics than from on-screen text paired with on-screen graphics. The mechanism is dual-channel processing: spoken words enter the verbal channel via auditory working memory, while graphics enter the visual channel — the two channels work in parallel. On-screen text + on-screen graphics forces both into the visual channel, creating a bottleneck and the split-attention effect.

The split-attention effect was demonstrated experimentally by Sweller, Chandler, and colleagues in the 1990s. Tindall-Ford, Chandler, and Sweller (1997) showed that when learners had to integrate text and diagrams that were spatially separated, performance dropped compared to integrated formats; when the text was replaced by narration, performance improved further. Kalyuga, Chandler, and Sweller (1999) extended the work, showing that the modality advantage is most pronounced for novice learners and complex material — which describes nearly every undergraduate lecture audience.

The practical implication for slides: if the speaker is present, the slide should carry the visuals and labels, and the speaker should carry the prose. The slide-as-prose configuration forfeits the dual-channel advantage and pushes the lesson into one overloaded channel.

**Common misconception:** That the Modality Principle means "always use audio narration." It means "in a multimedia learning context, prefer narration over on-screen text *when paired with visuals*." A pure-text reading task is not a Modality Principle context; a lecture with slides is.

**Worked example:** A slide showing a labeled diagram of the citric acid cycle with the speaker explaining each step in narration vs. a slide showing the same diagram with a 60-word paragraph explanation next to it that the speaker reads aloud — the first configuration uses dual channels and Modality; the second creates split-attention and Redundancy simultaneously.

**Source(s):**
- Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.), chapter on Modality.
- Tindall-Ford, S., Chandler, P., & Sweller, J. (1997). When two sensory modes are better than one. *Journal of Experimental Psychology: Applied*, 3(4), 257–287.
- Kalyuga, S., Chandler, P., & Sweller, J. (1999). Managing split-attention and redundancy in multimedia instruction. *Applied Cognitive Psychology*, 13(4), 351–371.

### Word-count benchmarks — what the practitioner literature actually says

The chapter's "30–50 words for live, >75 is a document" benchmark is consistent with the practitioner literature but worth grounding in specific sources:

- Reynolds (*Presentation Zen*) does not state a hard word-count rule but recommends "as few words as possible" and his worked examples typically run 5–15 words per slide. The "Reynolds suggests ~6 words" figure that circulates online is a folklore compression of his examples, not a quoted rule. [verify]
- Cliff Atkinson's *Beyond Bullet Points* (2007, updated editions through 2018) recommends full-sentence assertion headlines rather than fragment titles, paired with sparse evidence; his slides typically run 20–40 words including the headline.
- Kosslyn (*Clear and to the Point*, 2007) endorses a maximum of 4 bullets per slide with each bullet limited to 4 information "units" — a rough word-count cap of 30–50 words.
- The Wittich et al. (2016) CME-lecture study found a mean of approximately 26 words per slide across 105 lectures, with image fraction (not word count alone) the stronger predictor of speaker evaluation. [verify exact mean — confirm against the original paper]

The takeaway: the practitioner literature converges on roughly 30–50 words as the operating range for live-delivery slides, with the upper bound varying by use case. The chapter can defensibly cite this range without overclaiming a single source.

**Common misconception:** That word-count rules are absolute. They are heuristics calibrated to the live-lecture use case. A study-artifact deck honestly used as a study artifact can have much higher density without failing the relevant principles, because the redundancy-with-narration configuration does not arise.

**Worked example:** A 28-word slide with a clear assertion headline and a labeled diagram serves a live lecture well. The same 28 words rendered as a wall of body text without hierarchy fails for hierarchy reasons (Ch 2) even though the word count is fine.

**Source(s):**
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders.
- Atkinson, C. (2018). *Beyond Bullet Points* (4th ed.). Microsoft Press.
- Kosslyn, S.M. (2007). *Clear and to the Point: 8 Psychological Principles for Compelling PowerPoint Presentations*. Oxford University Press.
- Wittich, C.M., Mauck, K.F., Mandrekar, J.N., et al. (2016). Improving teaching effectiveness for medical CME with image-rich slides. *Western Journal of Emergency Medicine*. (Or related medical-education journal — confirm citation.)

### The notes-field move — where the cut content goes

Cutting text from the slide is not the same as discarding it. The Brutalist convention, consistent with Reynolds' two-artifact recommendation, is that essential prose lives in the slide's notes field. The speaker reads it during preparation; the live audience does not see it; the async export (slide + notes printed together) restores it for study.

This is the move that makes aggressive text reduction practically possible. The faculty member's resistance — "but students need the explanation" — is met by "the explanation is still here, in the notes field, where it serves study without competing with narration during live delivery."

**Common misconception:** That populated notes fields are extra work. They are the *same content* the slide previously held, relocated. The total writing effort is the same; the design is different.

**Worked example:** A slide previously reading (verbatim) "Oxidative phosphorylation uses the proton gradient across the inner mitochondrial membrane to drive ATP synthase, generating approximately 32 ATP per glucose molecule." Reduced live slide: labeled diagram of inner membrane + heading "ATP synthase: ~32 ATP / glucose." Original sentence: moved to notes field, expanded if useful.

**Source(s):**
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.), chapter on preparation and the "G-format."
- Brutalist DESIGN.md notes-field conventions (per the system's documentation in pantry/brutalist/).

---

## B. Domain examples and cases

### Case 1: Harp & Mayer's lightning-formation experiments

Harp and Mayer (1997, 1998) ran the now-canonical experiments on seductive details using a lesson on lightning formation. Students received either a stripped-down explanation of the physics or the same explanation augmented with entertaining anecdotes (e.g., dramatic accounts of lightning strikes) and dramatic photos. The augmented version produced engagement; the stripped version produced learning. Students in the stripped condition recalled structurally important content at approximately three times the rate of students in the augmented condition. This is the chapter's empirical anchor for the seductive-details claim. The Rey (2012) meta-analysis confirms the effect across many studies and material types.

**Source:** Harp, S.F., & Mayer, R.E. (1998). How seductive details do their damage: A theory of cognitive interest in science learning. *Journal of Educational Psychology*, 90(3), 414–434.
Rey, G.D. (2012). *Educational Research Review*, 7(3), 216–237.

### Case 2: The textbook paragraph pasted onto the slide

The most common faculty-generated failure case: a slide whose body is a paragraph (or sub-paragraph) copy-pasted from a textbook chapter. The textbook paragraph is calibrated for slow reading, re-reading, and annotation in print. The slide projects it at lecture distance with the speaker simultaneously delivering the same content. This is the Type-1 (Redundancy) failure mode in its purest form. The diagnostic question — "what would happen if I deleted this text?" — produces an immediate fix: delete the paragraph, keep the heading or terms, move the paragraph to the notes field.

This is the canonical Brutalist-system before/after case for the chapter, because the Brutalist generator's default behavior (transcribing textbook content into bullets) produces exactly this failure. The reader recognizes the output.

**Source:** No single primary citation — this is the synthesis of Reynolds, Mayer, and the lecture-slides-deep-research notes (lines 116–123).

### Failure case: The Wittich et al. CME lecture corpus

Wittich and colleagues (2016) analyzed 105 continuing medical education lectures and measured slide-level variables (word count, image fraction, animation use) against speaker evaluation scores. Image fraction — the proportion of slides with at least one educationally relevant image — was a significant positive predictor of evaluations. Mean text density was approximately 26 words per slide. Notably, raw word count alone did not significantly predict evaluations after controlling for image use. The implication: text reduction matters less than visual augmentation. Reducing text without replacing it with relevant visuals is a half-measure; replacing prose with diagrams, labeled images, or charts is the full move. This connects forward to Chapter 4 (the Wrong Visual Form).

**Source:** Wittich, C.M., et al. (2016). [verify exact citation — likely *Western Journal of Emergency Medicine*, *Mayo Clinic Proceedings*, or a CME-focused journal; double-check the venue and DOI before final use.]

---

## C. Connections and dependencies

**Prerequisites (what reader must already know):**
- Chapter 1: the live/async distinction and the redundancy diagnosis. Type-1 in this chapter is the slide-level version of the slideument failure.
- Chapter 2: hierarchy — because text reduction without hierarchy produces sparse but still navigable-poorly slides.
- The Brutalist notes-field convention.

**Unlocks (what this chapter makes possible):**
- The coherence/seductive-details vocabulary — fully developed in Chapter 7 (Seductive Details, deck-level).
- The text-cut-then-replace-with-visual move — feeds Chapter 4 (Wrong Visual Form).
- The "which learning objective does this serve?" diagnostic — recurs in every subsequent chapter as the load-bearing test.

**Adjacent chapter connections:**
- Chapter 1 (Slideument): Per TIKTOC.md, Type-1 failure in this chapter is "slideument failure at the individual slide level." The two chapters share the redundancy diagnosis; Ch 1 names it at deck level, Ch 3 at slide level.
- Chapter 2 (No Clear Hierarchy): Text density and hierarchy interact — a hierarchical slide can carry more text than a flat one before saturating working memory.
- Chapter 4 (The Wrong Visual Form): Per TIKTOC.md bridge, "Sometimes the text is right but the visual form is wrong." Cutting text is half the move; replacing it with the right form is the other half.
- Chapter 7 (Seductive Details): The Type-2 failure mode in this chapter is the slide-level instance of Chapter 7's deck-level seductive-details treatment.
- Chapter 10 (Headline That Says Nothing): Assertion extraction — the move of compressing a paragraph to a load-bearing claim — sets up the assertion-evidence rewrite.

---

## D. Current state of the field

**Settled:**
- Redundancy (identical text + narration) impairs learning — Mayer & Johnson (2008), Mayer (2020). Highly replicated.
- Seductive details impair retention and transfer — Harp & Mayer (1997, 1998), Rey (2012) meta-analysis. Robust effect.
- The split-attention effect — text and visual separated in space or modality impairs learning vs. integrated formats — Sweller, Tindall-Ford, Chandler (1997, and subsequent work).
- The Modality advantage (narration + visual > text + visual) for novice learners and complex content — Mayer (2009, 2020), Kalyuga et al. (1999).
- Image-rich slides are evaluated more highly than text-rich slides in actual lecture contexts — Wittich et al. (2016).

**Contested or emerging:**
- *Whether the seductive-details effect holds for high-prior-knowledge learners.* Some research (Magner et al., 2014) suggests the effect attenuates or reverses for learners who already have the schemas to integrate the extra material. The undergraduate audience of most lecture decks is low-prior-knowledge, where the effect is strong; the chapter can rest on this without overclaiming.
- *Whether engagement gains from interesting content offset learning losses.* Most empirical work measures learning, not the joint outcome of engagement + learning. The book's position is that learning is what we are after; engagement is instrumental, not terminal.
- *The exact word-count threshold.* Practitioner books converge on ~30–50 words for live but no rigorous empirical study (that I know of) has measured the marginal cost of each additional word. The chapter should present the range as practitioner consensus, not measured fact.

**Key references:**
1. Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.). Cambridge University Press. — Coherence, Redundancy, Modality, Segmenting Principles, all the cognitive-science backbone.
2. Harp, S.F., & Mayer, R.E. (1998). How seductive details do their damage. *Journal of Educational Psychology*, 90(3), 414–434. — Empirical anchor for seductive-details effect.
3. Rey, G.D. (2012). A review and a meta-analysis of the seductive details effect. *Educational Research Review*, 7(3), 216–237. — Meta-analytic confirmation.
4. Sweller, J., Ayres, P., & Kalyuga, S. (2011). *Cognitive Load Theory*. Springer. — Comprehensive CLT treatment including split-attention.
5. Wittich, C.M., et al. (2016). [confirm citation] — Empirical study of slide variables in real lecture corpus.

**Recent developments (last 3 years):**
- AI slide tools (Gamma, Beautiful.ai, Canva Magic Design, tome.app) systematically produce text-dense slides because their training data and prompts orient toward "complete-looking" output rather than minimal-text live-delivery output. The chapter's argument is sharpened by this: AI tools default to the Type-1 failure mode unless explicitly prompted otherwise. [verify with specific tool documentation]
- The shift to hybrid teaching (post-2020) has increased the prevalence of decks designed for both live and async use, which structurally invites the slideument hybrid. Chapter 3's diagnosis applies; Chapter 9 fully addresses the deck-level decision.
- Generative-AI image tools (DALL-E, Midjourney, Adobe Firefly, Canva AI) make replacing text with relevant visuals dramatically cheaper than five years ago. The "cut text, add visual" move that used to require finding or commissioning artwork is now a prompt. The chapter can note this as an enabler — though it stays out of tool-specific evaluation (per TIKTOC.md OQ5).

---

## E. Teaching considerations

**Where faculty get stuck:**
- *"My students need to see the definitions written out."* This is the most common defense of dense text. The fix is to redirect: yes, they need the definitions — in the notes field or in a separate study handout, not on the live slide. The diagnostic question: are you teaching live, or producing a study artifact? Different artifacts, different text densities.
- *"I'll forget what to say if I don't have the words on the slide."* Real concern. The fix is to populate the notes field as the speaker's script. The slide does not need to be the script; the notes do. The notes are visible only to the speaker.
- *"All this text IS the content — I can't just cut it."* This confuses content with rendering. The content is the *idea*; the prose is one rendering of it. A diagram, a label, a sparse headline, and a populated notes field can deliver the same idea differently.
- *"My students prefer detailed slides."* They do, because dense slides feel like comprehensive study materials. The evidence (Mayer, Harp & Mayer, Wittich et al.) is that this preference does not match learning outcomes. The book's move: acknowledge the preference, name the trade-off, and let the faculty member make the call — informed.
- *"Cutting the fun anecdote feels mean."* It is not mean; it is, on the evidence, what helps students learn the load-bearing content. Move the anecdote to the notes field, or to a "further reading" slide at the end, where it does not compete with the structural argument for attention.

**Analogies and framings that work:**
- *Stage directions vs. dialogue.* The slide is the stage direction telling the audience where to look. The narration is the dialogue. Putting the dialogue on the stage directions confuses both. (Original framing.)
- *Recipe card vs. cooking show.* The recipe card on the counter has the steps. The cooking show host explains what they are doing. A recipe card with all the host's banter written on it is harder to follow than either alone. (Original framing.)
- *Mayer's dual-channel diagram.* When the chapter introduces the Modality Principle, a small diagram showing the verbal channel (ear + phonological loop) and the visual channel (eye + visuospatial sketchpad) makes the bottleneck visible.

**Exercises that build the target skill:**
- *Before/after pair (the book's standard).* Take a Brutalist-generated content slide with a paragraph of body text. Apply the three-failure-mode diagnostic to identify which type it is. Run the appropriate prompt: for Type 1, "Reduce body to the assertion headline + 3 labels; move full text to notes field." For Type 2, "Identify and remove text not serving the stated learning objective." For Type 3, "Split this slide into 2–3 slides revealing concepts in sequence." Compare.
- Diagnostic questions for any slide:
  1. Which learning objective does each text element serve?
  2. Is any text repeating what the speaker will say aloud?
  3. Is any text interesting but not essential?
  4. Is the total word count above 50 for a live deck?
  5. If I removed each element and asked "did the lesson lose anything?" — for which elements is the answer no?

---

## F. Library files relevant to this chapter

- `lecture-slides-deep-research.md` — **Primary cross-reference.** The Coherence Principle treatment, the seductive-details section (lines 49–63), Mayer's 15 principles (lines 24–46), the slide-density evidence section (lines 215–225), the live-vs-async table — all directly feed this chapter. Several of the chapter's diagnostic moves are drawn from here.
- `_lib_EdTech.md` (plausibly) — Likely contains practitioner discussion of cognitive load and instructional design at the slide level.
- `_lib_Teaching-for-Deeper-Learning.md` (plausibly) — Likely covers the retrieval/consolidation moves that connect to "cut text, replace with retrieval prompt." Plausible cross-reference for the deeper-learning frame.
- `_lib_How-to-Deliver-a-TED-Talk.md` (plausibly) — Gallo on the TED slide aesthetic and sparseness norms.
- `_lib_The-Digital-Delusion-Horvath.md` (plausibly) — May contain critique of text-dense digital instruction; useful for the empirical-skeptic voice.
- `_lib_Thinking-Fast-and-Slow.md` (plausibly) — Kahneman's System 1/System 2: dense slides force System 2 processing on what should be a System 1 anchor.
- `_lib_Surfaces-and-Essences.md`, `_lib_Building-Thinking-Classrooms.md` — less directly relevant for Ch 3.

---

## G. Gaps and flags

- FLAG: The "Reynolds suggests ~6 words" figure that circulates in design folklore is a compression of his worked examples, not a quoted rule from *Presentation Zen*. Confirm against Reynolds directly before citing a specific number; safest to cite the range his examples demonstrate (5–15 words) or describe his recommendation qualitatively.
- FLAG: The Wittich et al. (2016) citation needs venue and DOI verification. I have given a likely journal but the exact title, year, and venue should be checked before use. The "mean ~26 words per slide" figure should be confirmed against the published paper.
- FLAG: Atkinson's *Beyond Bullet Points* is now in its 4th edition (2018). His assertion-evidence approach is closely related to Alley's; the two have collaborated. The chapter should be careful to cite the right primary source for the assertion-evidence claim (Alley & colleagues for the empirical work; Atkinson for the practitioner translation).
- FLAG: The Tindall-Ford, Chandler, Sweller (1997) split-attention paper is foundational but technical. The chapter should probably cite it in a footnote rather than the body, and use Mayer's textbook treatment for the body prose.
- FLAG: The seductive-details research has been extended by Magner, Schwonke, Aleven, Popescu, and Renkl (2014, "Triggering situational interest by decorative illustrations both fosters and hinders learning"), which suggests the effect can attenuate for some learner profiles. The chapter does not need to engage this nuance but the author should be aware.
- GAP: I do not have a clean empirical study measuring the marginal cost of each additional word on a slide. Practitioner consensus is around 30–50 words for live delivery, but the cliff (if there is one) is not located precisely in the literature. The benchmark should be presented as practitioner consensus, not measured fact.
- GAP: There is no direct empirical study (that I can name) measuring the prevalence of each of the three failure modes (Type 1/2/3) in AI-generated decks. The chapter's taxonomy is principled and useful but its claims about *what AI tools mostly produce* should be hedged or supported by spot-checks the author runs themselves.
- GAP: Connection to Chapter 7 (Seductive Details, deck-level) is strong — the chapter should explicitly note this is the slide-level instance, not the full treatment. The deck-level questions (which slides to cut entirely, how seductive details distribute across a deck) belong to Chapter 7.
