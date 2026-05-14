# Research Notes: Chapter 9 — Live Deck vs. Study Artifact

**Source:** TIKTOC.md chapter entry (lines 848–891)
**Notes file:** 09-live-deck-vs-study-artifact_notes.md
**Corresponding chapter:** chapters/09-live-deck-vs-study-artifact.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader accepts that a single deck cannot serve both live delivery and async study, makes the choice for their specific deck, and adjusts it accordingly.

**The feeling:** A deck posted as study materials that students found nearly useless — "it just has bullets, it doesn't explain anything." Or: a deck so text-dense it explains everything but is impossible to use in a live lecture without reading from the screen.

**The two products:** Live lecture deck (text minimal, speaker is the text, notes carry detail, speaker controls pacing) vs. study artifact (slide carries explanation, may be empty notes, student controls pacing, retrieval prompts must be self-contained).

**The decision:** Which is this deck for? This is a use question, not a design question. Design follows the decision.

**Solutions when both are needed:** (1) build two versions; (2) populate notes field fully; (3) record the lecture.

**Prompt category:** Text density adjustment + notes field population.
**DESIGN.md variable:** Notes field conventions; text density target per use case.

---

## A. Conceptual foundations

### A1. The slideument — Reynolds' diagnosis at the deck level

Garr Reynolds in *Presentation Zen* (2008, 3rd ed. 2019) named the failure mode: the "slideument" is the deck that tries to be both a live-presentation visual and a self-contained document, and serves neither role well. Reynolds' aphorism: *"Slides are slides. Documents are documents. They are not the same thing — and a slide that tries to be a document fails as a slide; a document that tries to be a slide fails as a document."*

Chapter 1 of this book introduced the slideument problem at the level of a single slide — too much text on a slide that's also being narrated, violating Mayer's Redundancy Principle. Chapter 9 takes the same idea to the deck level. A deck designed as a live anchor — sparse slides, speaker carrying the explanation — fails as a study artifact, because there's nothing to study. A deck designed as a study artifact — dense slides that carry the explanation — fails as a live anchor, because the audience reads instead of listening.

The original concept comes from Reynolds, drawing on Tufte's *The Cognitive Style of PowerPoint* (2003), which argued that the bullet-point format degrades analytical thinking by imposing a flat hierarchy that obscures the actual relationships among ideas. Tufte's prescription was: stop using slides for analytical content, hand out written documents instead. Reynolds softened the move: *use slides for what slides do, and documents for what documents do, and don't pretend one artifact can do both.*

**Common misconception:** "If I make the slides good enough, they can be both." The trade-off is structural, not effort-based. The features that make a slide good for live use (minimal text, speaker-anchored visual) are the same features that make it bad for async use (no explanation without a speaker). You cannot optimize both simultaneously because the optimization criteria conflict.

**Worked example:** A professor's slide on the central limit theorem has the title "CLT" and a single graph showing the sampling distribution narrowing as n grows. In a live lecture, this is a strong slide — it gives the speaker something to point at while explaining sampling distributions. Posted as a study artifact, it's nearly useless: a student looking at it three days later has a graph with no axes labeled, no narration, no explanation of what's narrowing or why. Same slide, opposite verdict, because the use case changed.

**Source:** Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders. Tufte, E. R. (2003). *The Cognitive Style of PowerPoint*. Graphics Press.

### A2. Mayer's Modality Principle — why the redundancy is unfixable

Mayer's Modality Principle, in *Multimedia Learning* (2009), states: people learn more deeply from pictures and spoken words than from pictures and printed words. Across seventeen experimental tests, students performed better on problem-solving transfer when animations were paired with narration than when they were paired with on-screen text.

The mechanism is dual-channel processing. Working memory has separate verbal and visual channels (Baddeley's model, extended by Mayer). When a slide shows a picture and the speaker narrates, the picture enters the visual channel and the narration enters the verbal channel. Two channels, parallel processing, no bottleneck. When a slide shows a picture and on-screen text, both enter the visual channel — the eye has to read the text while also processing the picture. Visual channel overloaded, learning degraded.

The Modality Principle is why the slideument is structurally broken. The live mode wants narration + minimal visual text (modality respected). The async mode requires on-screen text because there's no narration (modality violated, but unavoidable — you can't have narration without a narrator). The two use cases impose opposite design constraints because they have different audio channels available.

Mayer specifies boundary conditions where the modality advantage weakens: when the text is long and technical, when the learner is non-native, when the material is paced by the learner (async), when the content is highly familiar. The boundary conditions are exactly the conditions of asynchronous study. The principle is most powerful for live, instructor-paced, novel-content instruction — which is the live deck. For the study artifact, the trade-off shifts.

**Common misconception:** "If I just add narration to a text-heavy slide, I get the best of both." This is what slideuments often try to do — full bullets plus a recorded narration that reads the bullets. Mayer's Redundancy Principle says specifically: do not narrate the same words that appear on screen. The redundant verbal-and-visual presentation overloads both channels because the brain processes the same content twice. The fix is either narration without on-screen duplicate, or on-screen text without redundant narration. Not both.

**Worked example:** A Loom recording of a slide deck has the instructor reading every bullet aloud. The student watches and reads simultaneously. Their retention is worse than for either a sparser deck with full narration or a dense deck they read silently. Two channels both fully loaded with the same content is worse than either channel fully loaded with that content.

**Source:** Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press. Chapter 8: Modality Principle.

### A3. Atkinson's Beyond Bullet Points — the assertion-evidence move

Cliff Atkinson's *Beyond Bullet Points* (2005) is the practical operationalization of Mayer's principles for slide design. Atkinson's argument is that the default PowerPoint structure (topic header + bullets) violates multiple Mayer principles at once: redundancy (the bullets duplicate spoken content), modality (text-heavy slides force visual-channel processing), and coherence (bullet structure imports hierarchy regardless of whether hierarchy is the actual relationship).

His prescription is the assertion-evidence structure: a full-sentence headline stating a claim, and a visual that provides evidence for the claim. The headline is the only text. Everything else is the speaker.

The structure has been empirically tested. Garner & Alley (2013) in *Technical Communication* compared traditional bullet decks against assertion-evidence decks across multiple studies and consistently found higher retention and lower perceived cognitive load in the assertion-evidence condition. The mechanism: the headline gives the audience a schema to hang the visual evidence on, and the absence of competing text frees the visual channel to actually process the evidence.

The assertion-evidence structure is fundamentally a *live-deck* structure. It assumes a speaker. Without a speaker, the headline plus visual is a claim plus a graph — true but unexplained. The student studying from an assertion-evidence deck three days later sees a series of claims with images and no machinery for understanding why each claim follows.

**Common misconception:** "Assertion-evidence is always better." It's better for the use case it's designed for: live, expert-narrated, instructor-paced. For async, the same structure may underexplain. The Chapter 10 chapter on headlines makes this distinction; Chapter 9 generalizes it to the whole deck.

**Worked example:** An assertion-evidence slide reads "Working memory holds about four items — slide design must respect this limit" with a diagram showing four objects in a circle. Live, the instructor explains Cowan's revision of Miller, the experimental evidence, and the design implications. Three days later, a student looks at the slide. They see a claim and a circle. They cannot reconstruct the explanation. The slide was designed for an audience that has the speaker. It does not function for an audience that doesn't.

**Source:** Atkinson, C. (2005). *Beyond Bullet Points*. Microsoft Press. Garner, J. K. & Alley, M. (2013). How the design of presentation slides affects audience comprehension: A case for the assertion-evidence approach. *International Journal of Engineering Education*.

### A4. Async learning and the missing speaker

Means et al. (2010) conducted a meta-analysis for the U.S. Department of Education comparing online and face-to-face learning across 99 studies. The headline finding was that online learning produced modest gains over F2F on average, with blended learning showing the largest gains. The number is debated, and the studies are heterogeneous, but for the chapter's purposes the takeaway is narrower: async learning *can* be effective, but it requires materials designed for the absence of the speaker.

The async-learning literature converges on a consistent set of requirements for self-paced study materials: (1) explicit segmentation (learner-paced chunks, Mayer's Segmenting Principle); (2) embedded retrieval (questions the student attempts before being given the answer); (3) self-contained explanation (the artifact carries the content, not just the visual anchors); (4) navigation (the student can review and jump back).

A live deck designed for an expert speaker fails all four conditions when posted as async study material. There is no explicit segmentation because the speaker did the pacing. There is no embedded retrieval because the speaker asked the questions in the room. There is no self-contained explanation because the speaker carried it. Navigation is minimal because the linear sequence assumed a presenter walking through.

The Brutalist solution is the chapter's central practical move: produce *two artifacts from one source*. The speaker deck is sparse and visual-first. The study deck is annotated, with notes-field content baked into the slide or accompanying handout. Both derive from the same DESIGN.md but with a use-mode toggle.

**Common misconception:** "I'll just post the live deck and add a note saying 'see lecture recording for full content.'" In practice, students do not watch the recording for material they think they can study from the slides. The slides become the study artifact whether designed for it or not. If the live deck is what they study, the live deck has failed at the job it inherited.

**Worked example:** During COVID-era remote teaching, many faculty posted their live decks as the primary study material. Student complaint patterns were consistent: "the slides don't have enough information," "I can't tell what the bullet points mean," "I have to watch the whole recording every time I want to review one concept." The structural failure was visible at scale: live decks repurposed as study artifacts fail predictably.

**Source:** Means, B., Toyama, Y., Murphy, R., Bakia, M., & Jones, K. (2010). *Evaluation of Evidence-Based Practices in Online Learning: A Meta-Analysis and Review of Online Learning Studies*. U.S. Department of Education. [ed.gov/media/document/evaluation-of-evidence-based-practices-online-learning-meta-analysis-and-review-of-online-learning-studies-revised-september-2010-107159.pdf](https://www.ed.gov/media/document/evaluation-of-evidence-based-practices-online-learning-meta-analysis-and-review-of-online-learning-studies-revised-september-2010-107159.pdf)

### A5. The Brutalist solution — two artifacts from one source

The book's distinctive move is treating the live/study distinction as a *prompt-level toggle* rather than a manual rebuild. The DESIGN.md variable is the mode — `mode: live` or `mode: study` — and the same content source produces two output artifacts.

In `live` mode: assertion-evidence headlines, sparse slides, visual-first, notes field populated with full speaker script. In `study` mode: assertion plus full-sentence explanation, denser slides, embedded retrieval prompts every several slides, notes field optional. The content is the same; the rendering is different.

This requires the reader to have built up the diagnostic vocabulary from chapters 1–8: knowing what to put on the slide, what to put in notes, what to put in headlines, what to delete entirely. Chapter 9 is the integration chapter that says: now that you know what each element does, you can make the same source produce two artifacts because you know which elements promote to slide vs. notes vs. handout for each mode.

**Common misconception:** "Two decks is double the work." The Brutalist claim is that two decks from one source is *less* work than one slideument that tries to do both — because the slideument requires constant negotiation between competing constraints. Two clean artifacts each respect their own constraint and are easier to produce. The empirical test is whether the reader, having tried both approaches, prefers the split. Most do, by the second deck.

**Worked example:** A faculty member maintains a course in Brutalist. The source is `lecture-04.md` — markdown with content, learning objectives, and prompts. They build `lecture-04.live.html` (the speaker deck) and `lecture-04.study.html` (the study deck) from the same source with different DESIGN.md mode flags. When they update the content, both artifacts rebuild. The slideument failure — having to maintain a hybrid that fails both jobs — is replaced by two artifacts each doing their own job well.

**Source:** This is the chapter's contribution; no direct primary source. The supporting machinery is Mayer's principles and Reynolds' / Atkinson's design prescriptions.

---

## B. Domain examples and cases

### Case 1: The COVID-era posted live deck

Spring 2020, faculty across the country posted their live lecture decks as the primary remote study material. Student outcomes were poor and complaints were uniform: the slides didn't explain anything. The mechanism was the slideument failure at scale — decks designed for a speaker's narration, used by students who had no speaker. The faculty members who fared best either (a) recorded full narrated videos to accompany the live deck, or (b) produced separate study handouts. Neither group tried to make the live deck stand alone.

### Case 2: TED talk slides as live-deck exemplars

TED slides are aggressively sparse — usually a single image, a single phrase, or a single statistic. They are designed for an expert speaker holding a global audience for 18 minutes. They are useless as study artifacts; nobody would attempt to learn TED-talk content from the slides alone. The TED format is the existence proof that live decks can be radically minimal and still work *for their use case*. The same slides would fail every test of an async study artifact.

### Case 3: Atkinson's assertion-evidence engineering decks

Atkinson and Alley's research uses engineering education as the test bed. The traditional engineering lecture deck is dense with formulas, derivations, and labeled diagrams — partly because students are expected to study from it. Atkinson's assertion-evidence redesign strips the dense formulas off the slide and into a handout, leaving the slide as headline + one visual. The student gets two artifacts: the slides for the live experience, the handout for study. Garner & Alley's 2013 studies show this combination outperforms the dense slideument on both immediate and delayed retention.

### Failure case: the notes field "solution"

A common faculty solution is to populate PowerPoint's notes field with the full script and tell students to read the notes when studying. In practice, students rarely use the notes field. They study from the visible slides. The notes field is technically a study-artifact channel but its discovery and adoption rate is low. A better solution: produce a study artifact as a *handout* or *separate deck* that students will actually use. The notes field works if the workflow forces students through it (e.g., the LMS shows notes by default); it fails if it requires the student to know the feature exists and open it.

---

## C. Connections and dependencies

**Prerequisites (from earlier chapters):**
- Chapter 1 (Slideument): the slide-level version of the same failure. Chapter 9 is the chapter that finally teaches the distinction explicitly at the deck level.
- Chapter 3 (Too Much Text): the text-density target depends on use case. Chapter 9 makes the use-case decision that Chapter 3 left implicit.
- Chapter 7 (Seductive Details): the notes-field move (relocate rather than cut) only works once the reader has accepted that notes are a different channel.
- Chapter 8 (Covers but doesn't teach): the backward-design question "what is the deck for?" naturally extends to "what is the deck for — live or async?" Chapter 9 is the immediate follow-on.

**Unlocks (for later chapters):**
- Chapter 10 (Headline That Says Nothing): the assertion-evidence structure is the slide-level expression of the live-deck design philosophy.
- Chapter 11 (Owning Your DESIGN.md): the mode-toggle variable is one of the most consequential DESIGN.md decisions. Chapter 9 makes the reader configure it.

**Adjacent chapters:**
- Chapter 9 is the chapter TIKTOC.md flags as conceptually hardest. The acceptance that one deck cannot do both jobs is the load-bearing move of the entire deck-level half of the book. Everything in Act Three of the book assumes this acceptance.

---

## D. Current state of the field

**Settled:**
- The Modality Principle is among the most replicated in multimedia learning research (Mayer 2009 reviews 17 tests, 17 positive). Spoken narration plus visual outperforms on-screen text plus visual for the boundary conditions the principle specifies.
- The Redundancy Principle (don't narrate the same words shown on screen) is similarly well-established.
- Async learning effectiveness depends substantially on artifact design — sparse decks alone don't transfer.

**Contested:**
- Whether the assertion-evidence structure is always superior to bullet decks. Some practitioners argue specific use cases (reference slides, quick-recall lists) favor traditional structures. The "two people disagree about" section in the TIKTOC entry handles this.
- The strength of Means et al. (2010) findings on online vs. F2F. The meta-analysis has been criticized for heterogeneity and selection effects. The blended-learning advantage is more robust than the pure-online advantage.
- The growth of generative-AI tools that propose to "auto-explain" slides — turning sparse live decks into expanded study versions on the fly. The chapter should acknowledge this trajectory; whether it works empirically is unsettled.

**Key references:**
1. Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders.
2. Atkinson, C. (2005). *Beyond Bullet Points*. Microsoft Press.
3. Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press.
4. Garner, J. K. & Alley, M. (2013). How the design of presentation slides affects audience comprehension: A case for the assertion-evidence approach. *International Journal of Engineering Education*.
5. Means, B. et al. (2010). *Evaluation of Evidence-Based Practices in Online Learning*. U.S. Department of Education.

**Recent developments (last 3 years):**
- Post-pandemic, hybrid/HyFlex teaching has normalized the production of multiple artifacts from one course. The discipline of producing two-mode decks is more common than it was in 2019.
- Generative-AI auto-conversion tools (Gamma, Beautiful.ai) increasingly offer "compact view" vs. "presentation view" modes. The chapter should note this is the right direction but typically with default-quality output. The Brutalist move is making the toggle *intentional* and rooted in DESIGN.md.
- A continuing research thread on "slidecasting" (recorded narrated slides for async use) — see work by Jonathan Schroeder and others — suggests that narrated live decks can serve async use *if* the narration is dense and the deck is sparse. The trade-off shifts but does not disappear. [verify exact citations]

---

## E. Teaching considerations

**Where faculty stick:**
1. "But my students need to study from the slides." The most common defense. Response: yes — give them a study artifact. The slides they study from should not be the slides they watch.
2. "Two decks is too much work." Addressed by the DESIGN.md mode toggle — one source, two builds. The cost is mainly the upfront investment in source structure.
3. "I've always done it this way." The acceptance question is the hardest in the book per TIKTOC.md. The chapter has to earn the move with evidence (Modality, Redundancy, assertion-evidence research) and an existence proof (the two-artifact workflow demonstrably works).
4. "What about hybrid live-and-recorded?" Recording the live lecture makes the live deck retrospectively-studyable via the recording. The recording is the study artifact in that case; the slide deck is still the live artifact. Two artifacts, one being the recording.
5. "Aren't notes fields the standard solution?" Notes fields work *if* the student workflow uses them. In most LMS contexts they don't — students download the PDF of the slides and study from that. The notes field is a partial solution at best.

**Analogies:**
- *A screenplay vs. a novel.* A screenplay is sparse — it relies on actors, direction, performance to fill in. Hand a screenplay to a reader who has never seen a film and they get fragments. A novel is dense — it carries its own performance. Two artifacts, two purposes, no confusion. A "screenplay-novel hybrid" would be unreadable.
- *Sheet music vs. a recording.* Sheet music tells a performer what to play. A recording is the performance itself. A student of music wants both, separately. A "sheet-music-with-recording-baked-in" is not a thing.

**Exercises:**
1. *Warm-up:* Take a slide. Ask: "could a student understand this slide without the speaker?" If yes — it's a study slide. If no — it's a live slide. Most decks are mixed. Count the mix.
2. *Application:* Take a single live slide and produce its study-artifact version. What changed? Headline becomes full sentence? Visual gains annotations? A retrieval prompt is appended?
3. *Synthesis:* Take a 20-slide live deck. Specify what would change to convert it to a study deck — slide by slide. Where do you add content? Where do you remove? Where do you keep?
4. *Challenge:* Defend a slideument that the faculty member uses currently and likes. What does it do well? What does it fail at? Where could a use-case split improve it?

---

## F. Library files relevant to this chapter

- **`pantry/lecture-slides-deep-research.md`** — section on "Slides for Live Presentation vs. Async/Self-Paced Viewing" (lines 228–240) is the single most directly relevant prior research. Tufte/Reynolds on signal vs. noise (lines 129–133) and the typography/layout sections also load-bearing.
- `pantry/_lib_How-to-Deliver-a-TED-Talk.md` — likely relevant for live-deck exemplars (TED-style sparse decks).
- `pantry/_lib_EdTech.md` — async learning and online-learning context.
- `pantry/_lib_The-Digital-Delusion-Horvath.md` — likely critical-perspective check on the async-as-effective claim.
- `pantry/brutalist/DESIGN.md` — operationalizes the mode-toggle variable that is the chapter's central practical mechanism.
- `pantry/brutalist/CLAUDE.md` — defines how the two-artifact build is invoked.

---

## G. Gaps and flags

- **FLAG:** Atkinson's *Beyond Bullet Points* was originally published 2005 and is now in its 4th edition (2018). The chapter should cite the edition being referenced. The assertion-evidence research is largely by Garner & Alley and colleagues; Atkinson is the practitioner-popularizer.
- **FLAG:** Reynolds' *Presentation Zen* aphorism about slideuments is widely paraphrased. The exact wording should be checked against the actual text before being put in quotation marks. [verify the precise phrasing]
- **FLAG:** Means et al. (2010) is sometimes cited as if it proves online is better than F2F. The actual finding is more nuanced — online and especially blended learning show small advantages on average, but the effect is heterogeneous and dependent on what's being compared. The chapter should report the finding carefully if it cites the meta-analysis at all.
- **FLAG:** The "Atkinson + Mayer 2005/2010 papers comparing slideument vs. presenter-anchored slides" referenced in the task brief is not a single canonical pair of papers. The relevant work is Atkinson's book (2005), Mayer's *Multimedia Learning* book (2009), and Garner & Alley's empirical papers (2009, 2013). The task brief framing should be corrected to the actual citation chain.
- **GAP:** Empirical research directly comparing "live deck only" vs. "live deck + study artifact" vs. "slideument used both ways" on student outcomes is thin. The Garner & Alley research compares slide *designs* but not the *two-artifact workflow* the chapter proposes. The chapter's central practical claim — that two artifacts beat one slideument — is theoretically well-grounded but lacks a head-to-head empirical test. Acknowledge.
- **GAP:** The chapter's discussion of generative-AI auto-conversion is speculative. As of 2026, the empirical evidence on whether auto-generated "study versions" of live decks are effective is essentially nonexistent. The chapter should treat this as a near-future development worth flagging, not as a current solution.
