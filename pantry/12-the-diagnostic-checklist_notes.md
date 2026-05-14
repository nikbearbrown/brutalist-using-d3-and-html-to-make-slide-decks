# Research Notes: Chapter 12 — The Diagnostic Checklist

**Source:** TIKTOC.md chapter entry
**Notes file:** 12-the-diagnostic-checklist_notes.md
**Corresponding chapter:** chapters/12-the-diagnostic-checklist.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** A single reference page — every diagnostic question from every chapter, organized by failure mode — that the reader can use on any slide, in any system, forever.

**What it is not:** A chapter. No new content. No new principles. No before/after pair. No prompt. This is a reference artifact, not a lesson.

**What it is:** The proof that the vocabulary was built. A reader who can work through this checklist on a slide they have never seen before has the eye. That was the goal of the book.

**Format:** One page. Two columns. Eleven failure modes as headers. Three to five diagnostic questions under each. Plain language — no framework jargon. Designed to be printed, pinned, and used.

**Status:** Per TIKTOC.md Open Question 4 (resolved 2026-05-13): Ch 12 is a standalone reference artifact, not a teaching chapter. Research scope here covers what makes checklists work as cognitive artifacts; the actual diagnostic questions are aggregated from Ch 1–11 chapter drafts (when written) rather than invented here.

---

## A. Conceptual foundations

### Why checklists work — the cognitive-load argument

The case for checklists as cognitive artifacts is grounded in two strands of research. The first is the working-memory limit established by Sweller's Cognitive Load Theory and Miller's prior work on chunking: human working memory holds roughly four chunks at once (updated from Miller's seven plus or minus two). The second is the observation, formalized by Hales and Pronovost (2006) in *Journal of Critical Care*, that experts in high-stakes domains do not fail because they lack knowledge — they fail because the right knowledge is not retrievable at the right moment under stress, fatigue, or time pressure. A checklist offloads retrieval from working memory to a stable external artifact, freeing the operator's attention for the parts of the task that genuinely require judgment.

Atul Gawande's *The Checklist Manifesto* (2009) is the popular treatment that brought this argument to a broad audience. Gawande's framing is that the complexity of modern professional work has outstripped the capacity of unaided memory — surgeons can no longer hold every relevant step in their head during a procedure, and pilots could not from the 1930s onward. The checklist is the artifact that compensates for the working-memory bottleneck. It is not a substitute for expertise; it is the scaffolding that lets expertise actually deploy.

The slide-design analog is direct. A faculty member building a deck under time pressure — between classes, on a Sunday night, at the end of a long semester — cannot reliably retrieve every diagnostic question they have learned across eleven chapters. The checklist makes the questions retrievable on demand, without depending on working memory. The cognitive offloading is the entire point.

**Common misconception:** That checklists are for novices and experts grow out of needing them. The empirical evidence — aviation, surgery, ICU — is the opposite. Experts benefit *more* from checklists than novices because experts face higher complexity and operate closer to working-memory saturation. Gawande's surgeons were not failing because they were new surgeons; they were failing because the operation was complex enough that even good surgeons missed steps without a checklist.

**Worked example:** A faculty member who has internalized the slideument diagnostic still produces slideuments when rushed. The checklist's "Is this deck for live delivery or async study?" question, asked before generation, prevents the failure that the internalized knowledge would prevent if there were time and attention to deploy it.

**Source(s):**
- Gawande, A. (2009). *The Checklist Manifesto: How to Get Things Right*. Metropolitan Books.
- Hales, B. M., & Pronovost, P. J. (2006). The checklist — a tool for error management and performance improvement. *Journal of Critical Care*, 21(3), 231–235. https://doi.org/10.1016/j.jcrc.2006.06.002

### Read-do vs. do-confirm — two checklist architectures

There are two distinct ways to use a checklist, named in the aviation literature and codified in Gawande's treatment. A *read-do* checklist is executed step by step as the operator reads each item: read step one, do step one, read step two, do step two. A recipe is a read-do checklist. A pre-flight checklist run by a single pilot before engine start is often read-do. A *do-confirm* checklist is run after a task is complete: the operator does the task from memory or routine, then runs the checklist to confirm nothing was missed. A surgeon's pre-incision checklist is typically do-confirm — the team has done their preparation, then they pause to verify.

The architectural choice depends on the task. Read-do is appropriate when the steps must occur in a specific order and the operator cannot reliably remember the sequence. Do-confirm is appropriate when the operator can perform the task fluently but might omit a step under cognitive load. The slide-design checklist is, by design, a *do-confirm* artifact. The faculty member builds the deck. Then they run the checklist to confirm. Reading the checklist before each slide would be slower than building intuition; running the checklist after the deck exists catches the failures the intuition missed.

This distinction matters for the chapter's design. The eleven failure modes are checked against an existing deck, not used as a recipe for building one. The questions are framed in the diagnostic mood ("Is the headline a claim or a label?") rather than the imperative ("Write a claim headline"). The grammatical form is the architectural choice.

**Common misconception:** That all checklists are the same. They are not — the read-do/do-confirm distinction is the most important architectural decision in checklist design and the one most frequently mishandled. A checklist that should be do-confirm rendered as read-do becomes paperwork; a checklist that should be read-do rendered as do-confirm misses the failure mode it was meant to prevent.

**Worked example:** A faculty member who runs the Ch 12 checklist *before* generating the deck is using it as read-do — and will probably find it slow and unhelpful, because the diagnostic questions presuppose the existence of a slide to diagnose. The same faculty member who generates the deck first and then runs the checklist is using it correctly as do-confirm. The chapter's brief framing instructions should make this explicit.

**Source(s):**
- Gawande, A. (2009). *The Checklist Manifesto*. Metropolitan Books. (See discussion of Boeing checklist evolution and read-do/do-confirm distinction throughout.)
- Boorman, D. (Boeing). On checklist philosophy, cited in *The Checklist Manifesto* and in https://code7700.com/checklist_philosophy.htm

### What makes a checklist effective — Gawande's criteria

Drawing on Daniel Boorman's checklist-design work at Boeing, Gawande names criteria that distinguish effective checklists from paperwork. Items must be *killer items* — the steps where failure is plausible and consequential, not every conceivable step. The checklist must fit on one page (longer checklists are not followed). The language must be plain — jargon causes users to skip items. The checklist must be *tested in the field* — what works on paper often fails in use, and revision in actual conditions is essential. The checklist should specify *who does what* when relevant, and *when* in the workflow it is run.

The slide-design checklist meets these criteria. Eleven failure modes, three to five questions each, total roughly forty-five questions — borderline at the upper limit of one-page feasibility. The questions are in plain language (the TIKTOC.md draft questions use no framework jargon — "Where does my eye go first?" rather than "What is the Gestalt grouping of attention?"). The workflow placement is do-confirm after deck generation. The remaining criterion — field testing — is where the chapter is weakest, because the checklist has not yet been used by readers other than the author. This is a known gap.

The "killer items" criterion is the one most easily violated by an author who knows the material too well. The temptation is to ask every diagnostic question that came up in the book. The discipline is to keep only the questions that catch failures the reader actually makes, not the failures the reader could conceivably make. The chapter's curation pass — which questions survive from the chapter drafts — is the work of distinguishing killer items from comprehensive coverage.

**Common misconception:** That a longer checklist is more thorough and therefore better. Gawande's evidence is the opposite. Checklists that exceed one page are not followed; the user skips items, defeating the purpose. The discipline of cutting is more important than the discipline of including.

**Worked example:** The TIKTOC.md draft has approximately 40 questions across 11 sections. This is close to but not over the one-page threshold; some sections will likely need to be trimmed in production. The cut decisions should be made on the basis of which questions catch failures, not which questions feel important.

**Source(s):**
- Gawande, A. (2009). *The Checklist Manifesto*, ch. 6 ("The Checklist Factory"). Metropolitan Books.
- Boorman, D. (n.d.). Boeing checklist philosophy. Discussed in Gawande (2009) and at https://code7700.com/checklist_philosophy.htm

### The teaching paradox — checklists work best when internalized

There is a counterintuitive empirical pattern in the checklist literature. Checklists produce the largest benefit when first introduced, then continue to produce a benefit, but the user's relationship to them changes: with use, the checklist becomes a redundancy check rather than a memory aid. The expert who has run the WHO surgical safety checklist for two years still runs it — but most items are now habit, and the checklist catches the rare day where habit is interrupted.

For the slide-design reader, this is the right ending for the book. The first few times the reader works through the Ch 12 checklist, they are using it to retrieve vocabulary the chapters built. After enough decks, the checklist becomes a redundancy check — the reader has internalized the eye, and the checklist catches the days the eye is tired. The book's promise is that this internalization happens. The checklist is both the proof and the safety net.

**Common misconception:** That a checklist that becomes "habit" is no longer needed. The Hales and Pronovost line of work directly addresses this: experts who stop using the checklist when they feel confident reintroduce the failures the checklist prevents. The reduction in catheter-related bloodstream infections in the Michigan ICUs (Pronovost et al. 2006) was sustained because the checklist was sustained; populations that stopped using it returned to baseline rates.

**Worked example:** The TED-talk speaker who has given the same talk fifty times still does the pre-talk run-through (mic check, water placement, slide advance test). The run-through is the checklist; experience does not retire it.

**Source(s):**
- Pronovost, P., Needham, D., Berenholtz, S., et al. (2006). An intervention to decrease catheter-related bloodstream infections in the ICU. *New England Journal of Medicine*, 355(26), 2725–2732. https://www.nejm.org/doi/full/10.1056/NEJMoa061115
- Haynes, A. B., Weiser, T. G., Berry, W. R., et al. (2009). A surgical safety checklist to reduce morbidity and mortality in a global population. *New England Journal of Medicine*, 360(5), 491–499. https://www.nejm.org/doi/full/10.1056/NEJMsa0810119

---

## B. Domain examples and cases

### Case 1: The B-17 origin — the first modern pre-flight checklist

On October 30, 1935, the prototype Boeing Model 299 (later the B-17 bomber) crashed during a demonstration flight at Wright Field, killing two of the five crew. The cause was simple: the pilots forgot to release a control lock before takeoff. The aircraft was not too difficult for trained pilots; it was too complex to fly without external scaffolding for memory. Boeing's response was the pre-flight checklist — a short, ordered list of items printed on a single card. With the checklist, the B-17 went on to fly 1.8 million miles without an accident attributable to pilot oversight, and the Army Air Corps ordered nearly 13,000 of them. The case is the most cited origin story in the checklist literature and the structural template for every subsequent professional checklist.

The B-17 case carries a specific lesson for the slide-design checklist: the failure mode the checklist prevents is not ignorance, it is *omission under pressure*. The reader of this book is not failing because they do not know the diagnostic vocabulary. They are failing because, at 11 p.m. on a Sunday building Monday's lecture, the vocabulary is hard to retrieve. The checklist makes retrieval reliable.

**Source:** Gawande (2009), ch. 2 ("The Checklist"). Aviation Geek Club, https://theaviationgeekclub.com/did-you-know-the-pre-flight-checklist-was-first-introduced-by-boeing-following-the-1935-crash-of-the-prototype-b-17-then-known-as-the-model-299/

### Case 2: The WHO Surgical Safety Checklist — the canonical clinical evidence

The Haynes et al. (2009) study published in the *New England Journal of Medicine* is the most-cited evidence that checklists improve outcomes in clinical settings. The WHO Surgical Safety Checklist — a 19-item, single-page checklist run at three points in a surgical procedure (sign-in, time-out, sign-out) — was implemented in eight hospitals across Tanzania, India, Jordan, the Philippines, New Zealand, the United Kingdom, Canada, and the United States. After implementation, in-hospital mortality dropped from 1.5% to 0.8% (a 47% reduction) and inpatient complications dropped from 11% to 7% (a 36% reduction). The effect held across high-income and low-income settings.

This is the strongest single piece of evidence that checklists can reduce error rates in skilled-professional contexts. It is also the case the chapter should be careful about — the evidence is clinical, and the inference to non-clinical settings is non-trivial. The next case complicates the picture.

**Source:** Haynes, A. B., Weiser, T. G., Berry, W. R., et al. (2009). A surgical safety checklist to reduce morbidity and mortality in a global population. *New England Journal of Medicine*, 360(5), 491–499. https://www.nejm.org/doi/full/10.1056/NEJMsa0810119

### Case 3: Pronovost's Michigan ICU checklist — the sustained-improvement case

Pronovost et al. (2006) implemented a five-item checklist for central venous catheter insertion across 103 Michigan ICUs (the Keystone ICU project). The checklist items were elementary: wash hands; use full sterile barriers; clean skin with chlorhexidine; avoid femoral insertion when possible; remove unnecessary catheters. The median rate of catheter-related bloodstream infections fell from 2.7 per 1,000 catheter-days at baseline to 0 within three months, and the reduction was sustained at 66% below baseline at 16–18 months.

The Pronovost case adds two things the Haynes case does not. First, it documents *sustained* improvement — the gains did not fade. Second, it surfaces the cultural-implementation argument that the next case (Bosk et al.) sharpens: the checklist worked because the broader project also empowered nurses to stop procedures, established daily review of catheter necessity, and treated the checklist as a system intervention rather than a standalone document. The checklist was the visible artifact; the cultural change was the mechanism.

**Source:** Pronovost, P., Needham, D., Berenholtz, S., et al. (2006). An intervention to decrease catheter-related bloodstream infections in the ICU. *New England Journal of Medicine*, 355(26), 2725–2732. https://www.nejm.org/doi/full/10.1056/NEJMoa061115

### Failure / critique case: Bosk, Dixon-Woods, Goeschel & Pronovost (2009) — "Reality Check for Checklists"

The most-cited critique of the checklist-as-solution narrative is Bosk, Dixon-Woods, Goeschel, and Pronovost (2009) in *The Lancet*. The argument: media coverage of the Haynes and Pronovost results treated the checklist as a stand-alone intervention, when in fact the checklist worked only in conjunction with broader cultural and organizational change — empowered nurses, leadership commitment, data feedback. Deploying a checklist without the surrounding cultural work, the authors argue, is "a technical solution to a cultural problem" and is likely to fail or to be resented.

This is the limit the slide-design chapter must name. The Ch 12 checklist will work for a reader who has worked through the vocabulary in Ch 1–11 and is using the checklist as do-confirm against decks they are motivated to improve. It will not work — and probably should not be used — by an administrator who downloads it and demands faculty apply it without the prior reading. The checklist is the visible tip of the iceberg; the iceberg is the diagnostic vocabulary built by the chapters.

This is also the chapter's most honest move. Naming the limit prevents the checklist from being mistaken for a stand-alone solution, which would falsify the book's larger argument that the vocabulary is what matters.

**Source:** Bosk, C. L., Dixon-Woods, M., Goeschel, C. A., & Pronovost, P. J. (2009). Reality check for checklists. *The Lancet*, 374(9688), 444–445. https://doi.org/10.1016/S0140-6736(09)61440-9

---

## C. Connections and dependencies

**Prerequisites (what reader must already know):**
- The full diagnostic vocabulary from Ch 1–11. The checklist's questions are phrased to be retrievable by a reader who has built the vocabulary; for a reader who has not, the questions read as vague and unanswerable.
- That the reader has a deck in hand to diagnose. The checklist is a do-confirm artifact, not a pre-build recipe.
- The framing that DESIGN.md is the upstream artifact (Ch 11): when the checklist catches a failure, the fix often lives in DESIGN.md, not in the slide.

**Unlocks (what this chapter makes possible):**
- The reader has a take-home reference artifact, which transforms the book from a one-time read into a sustained practice.
- The book's promise — "the proof that the vocabulary was built" — becomes operational: working through the checklist on a novel deck is the test that the eye exists.
- The checklist becomes the artifact other faculty members see first, creating the social pathway through which the diagnostic vocabulary spreads.

**Adjacent chapter connections (the aggregation map):**
Each prior chapter contributes three to five diagnostic questions to this checklist. The aggregation is the central editorial work of Ch 12. The map:

- Chapter 1 (Slideument) → questions on live-vs-async use, redundancy, notes field
- Chapter 2 (Hierarchy) → questions on eye-flow, size levels, proximity, whitespace
- Chapter 3 (Too Much Text) → questions on per-element learning objective, word count, redundancy
- Chapter 4 (Wrong Visual Form) → questions on relationship type, form-content match
- Chapter 5 (Color) → questions on color encoding, contrast ratio, colorblind safety
- Chapter 6 (Textbook Figure) → questions on print-vs-projection, last-row test, signaling, simplification limit
- Chapter 7 (Seductive Details) → questions on learning-objective mapping, interesting-vs-essential
- Chapter 8 (Covers vs. Teaches) → questions on hook/build/consolidate, dependency order, chunking
- Chapter 9 (Live vs. Async) → questions on deck purpose, text density, notes field population
- Chapter 10 (Headline) → questions on assertion vs. label, claim-vs-reference-slide distinction
- Chapter 11 (DESIGN.md) → questions on rationale, framework-vocabulary defense

The TIKTOC.md draft (lines 1009–1076) has a first pass at these questions. The chapter's editorial work is to refine them as each prior chapter is written and the questions earn their final phrasing.

---

## D. Current state of the field

**Settled:**
- Checklists reduce error rates in high-stakes professional contexts when properly designed and implemented (Haynes et al. 2009; Pronovost et al. 2006; aviation literature since the 1930s).
- Working memory limits make unaided expert performance unreliable in complex tasks (Sweller; Miller; Hales & Pronovost 2006).
- Effective checklists are short, plain, tested in use, and architecturally appropriate to the task (read-do vs. do-confirm) (Gawande 2009; Boorman / Boeing checklist philosophy).
- Checklists work best as part of a broader cultural and organizational practice, not as stand-alone documents (Bosk et al. 2009).

**Contested or emerging:**
- *Whether the clinical-setting evidence generalizes to non-clinical, non-aviation contexts.* The slide-design case is plausibly within the generalization but is not empirically tested. The chapter should be honest about this — citing clinical evidence as inspiration, not as direct proof.
- *Whether AI-mediated tools can replace checklists or merely augment them.* An AI tool that reads DESIGN.md and applies the diagnostic questions automatically would arguably make the checklist redundant. The chapter's position should be that the human reader still benefits from explicit checklist review even when an AI tool is also running checks — the two are complementary.
- *The "checklist fatigue" critique.* In clinical settings, the proliferation of checklists has produced reports of fatigue and routinization. A single forty-question checklist used occasionally is at lower risk than the checklist-per-protocol density of modern hospitals.

**Key references:**
1. Gawande, A. (2009). *The Checklist Manifesto: How to Get Things Right*. Metropolitan Books. — The popular case and the integrative framing.
2. Haynes, A. B., et al. (2009). A surgical safety checklist to reduce morbidity and mortality in a global population. *NEJM*, 360(5), 491–499. — The canonical clinical evidence.
3. Pronovost, P., et al. (2006). An intervention to decrease catheter-related bloodstream infections in the ICU. *NEJM*, 355(26), 2725–2732. — Sustained improvement at scale.
4. Hales, B. M., & Pronovost, P. J. (2006). The checklist — a tool for error management and performance improvement. *Journal of Critical Care*, 21(3), 231–235. — The review-article framing of why checklists work.
5. Bosk, C. L., Dixon-Woods, M., Goeschel, C. A., & Pronovost, P. J. (2009). Reality check for checklists. *The Lancet*, 374(9688), 444–445. — The critical voice — essential for honest treatment.

**Recent developments (last 3 years):**
- Continued clinical implementation studies on the WHO Surgical Safety Checklist have produced mixed results — some replications show smaller effects than the original Haynes study, attributed to implementation variation. The original 2009 finding remains the most-cited single piece of evidence; effects in subsequent implementations vary with cultural conditions, consistent with the Bosk critique.
- AI-mediated workflows have introduced new analog questions: when a model can run a checklist automatically against an artifact, does the human still need to? Industry experience suggests yes — the model and the human catch different failure modes.

---

## E. Teaching considerations

**Where faculty get stuck:**
- *"I'll use the checklist once and then I won't need it."* Counter: the checklist literature suggests the opposite — sustained use produces sustained benefit; abandonment reintroduces the failures. The chapter's framing: the checklist is for tired you, not present you.
- *"This feels like bureaucracy."* Real concern, especially for academic faculty who have endured checklist-driven assessment regimes. Mitigation: the slide-design checklist is forty questions on one page, run once per deck, by the faculty member on their own deck. It is not external compliance; it is self-applied diagnostic.
- *"What if I disagree with one of the questions?"* The chapter's move: disagree, in framework vocabulary. The reader who can explain why a question doesn't apply to their context is using the checklist correctly; the reader who skips a question without reflection is using it as paperwork.

**Familiarity gradient (how the checklist is used at different stages):**
- *First read:* The reader uses the checklist as a memory aid. They look up each question, retrieve the chapter vocabulary it points to, apply it. Slow, deliberate, somewhat clumsy.
- *Fifth read:* The reader moves through the checklist faster. Some questions are obvious (the deck passes); some questions still require reflection. The vocabulary is becoming retrievable from the questions alone.
- *Tenth read:* The reader has internalized the eye. They can produce a deck that mostly passes the checklist before running it. The checklist now functions as a redundancy check — it catches the day when the eye is tired or the deck is built under pressure.

The chapter should name this gradient explicitly. The reader should expect to find the checklist slow at first, faster with use, and eventually invisible — exactly the trajectory the surgeon or pilot follows with their professional checklists.

**Analogies and framings that work:**
- *The pre-flight checklist.* The most familiar analog, but use carefully — academic readers may roll their eyes at the analogy to high-stakes domains. The honest version: the structural reason it works is the same (offloading retrieval from working memory); the stakes are different.
- *The peer review checklist.* Reviewers for journals use one. It is short, plain, run once per manuscript. The slide-design checklist is the deck's peer review, self-administered.
- *The pre-class chalkboard check.* A faculty member who walks into a classroom and confirms the chalkboard is erased, the projector works, the handouts are stacked. The pre-class check is a checklist run without paper, established by habit. The Ch 12 checklist makes the habit explicit until habit takes over.

**Exercises that build the target skill:**
- *Run the checklist on a deck you produced before reading this book.* Note which questions you cannot answer without re-examining the slide carefully. Those are the questions where the chapter's vocabulary has not yet become reflexive.
- *Run the checklist on a deck someone else produced.* Less defensive; faster. The questions you find yourself asking *before* the checklist names them are the questions you have already internalized.
- *Refuse to apply the checklist on a deck you trust.* See what fails. This is the discipline of Bosk et al. — when expertise feels sufficient, the checklist is still doing work.

---

## F. Library files relevant to this chapter

- `lecture-slides-deep-research.md` — Source of the cognitive-load framing (Sweller, Mayer) that explains *why* checklists are needed in slide design specifically. Cross-reference for the working-memory argument in Section A.
- `chapters/01-the-slideument-problem_notes.md` through `chapters/11-owning-your-design-md_notes.md` (and the corresponding drafts when written) — **The aggregation source.** Section C explicitly maps which questions come from which chapter; the actual phrasings will be drawn from each chapter's diagnostic-questions block as those chapters are drafted.
- `_lib_Teaching-for-Deeper-Learning.md` — Possibly contains material on retrieval practice and consolidation that is structurally relevant to the "checklist as retrieval scaffold" framing.
- `_lib_Thinking-Fast-and-Slow.md` — Kahneman's System 1 / System 2 framing is the deeper cognitive layer under "the checklist makes System 1 reliable when System 2 is depleted." Useful in Section A or E.
- `_lib_Building-Thinking-Classrooms.md` — Liljedahl's work on routines that scaffold productive struggle is structurally parallel — routine artifacts that free cognition for the hard work. May offer additional framings.
- `pantry/brutalist/DESIGN.md` — Referenced when the checklist points the reader to a DESIGN.md update rather than a slide tweak.

---

## G. Gaps and flags

- FLAG: The actual diagnostic questions in the checklist must be aggregated from the chapter drafts when those drafts exist. The TIKTOC.md draft (lines 1009–1076) is a first pass and is correct in structure; the final phrasings should be drawn from each chapter's diagnostic-questions section after that chapter is written. This research file describes *what type* of questions belong here; it does not invent or finalize them.
- FLAG: Haynes et al. (2009) NEJM DOI: 10.1056/NEJMsa0810119. Pronovost et al. (2006) DOI: 10.1056/NEJMoa061115. Confirm both before final citation.
- FLAG: Bosk et al. (2009) *Lancet* citation — volume 374, issue 9688, pages 444–445. DOI: 10.1016/S0140-6736(09)61440-9. Confirm pagination.
- FLAG: Hales & Pronovost (2006) — *Journal of Critical Care*, 21(3), 231–235. Confirm DOI and page range.
- FLAG: Gawande's *Checklist Manifesto* (2009, Metropolitan Books, ISBN 978-0805091748) is the popular treatment; the chapter should cite Gawande for the integrative framing but cite the underlying empirical papers (Haynes, Pronovost) for the empirical claims. Do not let Gawande's book substitute for the primary citations.
- FLAG: The B-17 Model 299 crash date (October 30, 1935) and casualty count (two of five dead) — confirm against a primary source rather than secondary Gawande citations. Aviation Geek Club and similar are reliable for the basic facts but the chapter should ideally have a primary citation if one is accessible.
- GAP: There is no published study (that I have identified) measuring whether a slide-design checklist improves slide quality or learning outcomes. The chapter's argument is by structural analogy from clinical and aviation evidence. This is honest research extrapolation and should be named as such.
- GAP: The "familiarity gradient" framing in Section E (first read → fifth read → tenth read) is the chapter's own pedagogical contribution. There is general checklist-literacy literature consistent with this gradient but no specific empirical study calibrating it for self-administered diagnostic checklists. The framing can be argued from first principles but should not be presented as empirically established.
- GAP: The chapter's production note (Ch 12 as a standalone PDF download) sets a design constraint — one page, printable. The questions must be trimmed to fit. The chapter should either (a) make the trimming editorial discipline explicit, or (b) accept a two-page format if the trimming would damage the diagnostic coverage. The TIKTOC.md draft is borderline on one-page feasibility. This is a production decision more than a research question, but worth flagging now.
