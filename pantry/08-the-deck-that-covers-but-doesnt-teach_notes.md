# Research Notes: Chapter 8 — The Deck That Covers but Doesn't Teach

**Source:** TIKTOC.md chapter entry (lines 800–846)
**Notes file:** 08-the-deck-that-covers-but-doesnt-teach_notes.md
**Corresponding chapter:** chapters/08-the-deck-that-covers-but-doesnt-teach.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns to diagnose coverage failure at the deck level — a deck organized around the textbook's structure rather than the learner's build — and restructure the opening arc.

**The feeling:** A deck that seems complete — every topic from the chapter is in there — but students zone out after the first fifteen minutes and retention on the exam is low.

**The coverage vs. teaching distinction:** A textbook chapter must cover the full territory. A lecture must cause learning. These are different operations.

**The lecture arc (Hook / Build / Consolidate):** *Hook* — problem or question that creates the need to know. *Build* — concepts in dependency order. *Consolidate* — retrieval practice or application before moving on.

**The 15-minute chunking rule:** Working memory saturates after ~15–20 minutes of continuous input. A 50-minute lecture needs at least two consolidation moments.

**Prompt category:** Deck resequencing.
**DESIGN.md variable:** Deck opening conventions; retrieval prompt slide template.

---

## A. Conceptual foundations

### A1. Coverage vs. teaching — the core distinction

Wiggins & McTighe (1998, 2nd ed. 2005) introduced this distinction in *Understanding by Design* and named it as the central failure mode of well-meaning instruction. Coverage means marching through content — page by page, slide by slide, topic by topic — until the territory is traversed. Teaching means producing change in the learner. These can look the same from the front of the room. They produce different results on the test.

Wiggins & McTighe call coverage "the twin sin of unfocused activity and content coverage" — instruction that has either lots of doing without understanding, or lots of telling without doing. Their corrective is **backward design**: start with the desired learning outcome, work backward to the assessment evidence that would show the learner has it, and only then design the instruction that builds toward it. The slide deck is the last step, not the first.

The instructor who builds a deck by walking through the textbook chapter is doing forward design — what they have (the chapter) determines what the students get (the slides). The backward-design move inverts this: what should the student be able to *do* after the lecture? What evidence would show they can do it? Now what slides cause that?

**Common misconception:** "If I cover the material, I've done my job — what students do with it is on them." This is the coverage default. It treats teaching as a transmission operation: information leaves the slide, enters the student. The cognitive-science evidence (Sweller, Mayer, Roediger) consistently shows transmission is not learning. Learning is what the student's mind does *with* the input. A deck that does not give them the input in a form they can process — and does not give them an opportunity to use it — has not taught.

**Worked example:** A 60-slide deck on Chapter 4 of an econometrics textbook covers OLS estimation, assumptions, hypothesis testing, multicollinearity, heteroscedasticity. Each topic gets 12 slides. The deck is exhaustive. After the lecture, students can recognize all the terms on a flashcard. None can correctly diagnose which assumption is violated in a given residual plot. Coverage: complete. Teaching: failed. The diagnostic move is not "add more slides." It is "what should students be able to *do* — diagnose residual plots — and what arc builds them to that?"

**Source:** Wiggins, G. & McTighe, J. (2005). *Understanding by Design* (2nd ed.). ASCD. [andymatuschak.org/files/papers/Wiggins, McTighe - 2005 - Understanding by design.pdf](https://andymatuschak.org/files/papers/Wiggins,%20McTighe%20-%202005%20-%20Understanding%20by%20design.pdf)

### A2. Cognitive load theory at the deck level — Sweller scaled up

Chapter 1 introduced cognitive load theory at the slide level. Chapter 8 generalizes it to the deck. The same three loads apply, but the failure mode is different.

A deck that covers without teaching imposes **intrinsic load** the student cannot process, because the prerequisite concepts have not been built first. Slide 12 assumes the student has internalized the schema introduced on slide 4 — but they haven't, because slide 4 also assumed they had internalized slide 1, which they didn't, because slide 1 was a definition. The intrinsic load compounds. By slide 20 the student is processing nothing.

A coverage-organized deck also imposes high **extraneous load** at the deck level — not from any individual slide's design, but from the *sequence*. The student spends working memory tracking where they are in the topic list rather than building the concept. This is the deck-level analog of Mayer's signaling principle (which says: at the slide level, signal what matters). At the deck level: signal where you are in the arc.

**Common misconception:** "If I add more examples, students will get it." More examples is more intrinsic load. The fix is sequencing examples in dependency order, not adding them. Sweller's worked-example research (1985 onward) is specifically about *which* examples and in *what order*, not *how many*.

**Worked example:** A 50-minute deck on regression analysis introduces a regression equation on slide 3 ("Y = β₀ + β₁X + ε"). It does not unpack what β represents, what ε does, or why we care about either. Slide 4 introduces R². Slide 5 introduces the F-statistic. By slide 6, the student is being asked to interpret an output table that uses all three. The deck has covered four concepts in five minutes. The deck has taught zero of them. The fix is not "speak slower." The fix is: spend slides 3–8 on β alone, including a worked example, a misconception ("β₁ is the slope, not the prediction"), and a retrieval moment. Only then introduce R².

**Source:** Sweller, J. (1988). Cognitive load during problem solving: Effects on learning. *Cognitive Science*, 12, 257–285. See also Sweller's worked-example research; Deans for Impact (2015) *The Science of Learning* summarizes the load implications for instruction. [deansforimpact.org/files/assets/thescienceoflearning.pdf](https://www.deansforimpact.org/files/assets/thescienceoflearning.pdf)

### A3. The lecture arc — hook, build, consolidate

The arc isn't speculative. Each move maps to specific evidence.

**Hook.** The motivating problem before the content is the move backed by Manu Kapur's "productive failure" research and by curiosity-and-learning work (Berlyne; Loewenstein's information-gap theory). Students who attempt a problem before being given the solution show better transfer than students given the solution first. The hook is the textbook deck's version: present the puzzle, let the student feel the gap, then offer the resolution.

**Build.** Dependency order is the operationalization of cognitive load theory plus what cognitive science calls "schema construction." Concepts have to be introduced in an order that lets the student build each one on a foundation they already have. The textbook chapter is often organized for *reference* — alphabetical, topical, comprehensive. The lecture deck has to be organized for *construction*.

**Consolidate.** Retrieval practice. Karpicke & Roediger (2008) in *Science* showed that students who attempt to retrieve information from memory after learning it retain substantially more than students who restudy the same material. The retrieval moment is *productive* — it produces learning, it does not just measure it. A deck that ends when the content ends throws away the most powerful retention opportunity available.

Spaced retrieval is even better: Cepeda et al. (2006) meta-analysis in *Psychological Bulletin* (839 effects from 317 experiments) confirms the spacing effect. A retrieval moment 15 minutes into a 50-minute lecture, and a second one at 40 minutes, beats a single retrieval moment at the end. Bjork & Bjork (2011) call these "desirable difficulties" — the student feels the moment is hard, the retention shows the moment is doing work.

**Common misconception:** "I'll add a Q&A at the end and that counts as consolidation." Q&A is voluntary retrieval by the few students who ask questions. Consolidation is forced retrieval by every student — a problem on the slide they have to attempt, a question they have to answer on a clicker, a peer-instruction prompt. The "any questions?" slide does not consolidate.

**Worked example:** A 50-minute lecture on supply and demand opens with a question: "Why did rents in San Francisco rise 30% during 2021?" Build: introduce demand curves (15 minutes, with one mid-build retrieval question on a shifted curve), then supply curves (15 minutes, with retrieval), then equilibrium (10 minutes). Consolidate: 10 minutes on the rent question, students attempt the analysis, then the instructor walks the resolution. The student leaves having *done* economics, not having *seen* economics done.

**Source:** Karpicke, J. D. & Roediger, H. L. (2008). The critical importance of retrieval for learning. *Science*, 319(5865), 966–968. [science.org/doi/abs/10.1126/science.1152408](https://www.science.org/doi/abs/10.1126/science.1152408). Cepeda, N. J. et al. (2006). Distributed practice in verbal recall tasks: A review and quantitative synthesis. *Psychological Bulletin*, 132(3), 354–380. Bjork, E. L. & Bjork, R. A. (2011). Making things hard on yourself, but in a good way: Creating desirable difficulties to enhance learning. In M. A. Gernsbacher et al. (Eds.), *Psychology and the Real World*. Worth.

### A4. Mayer's Segmenting Principle — learner-paced segments

Mayer's Segmenting Principle states that people learn better when a multimedia message is presented in learner-paced segments rather than as a continuous unit. The evidence is that learning improves when long instructional messages are broken into smaller, learner-controlled chunks.

In a live lecture, the instructor controls pace — segmentation is enforced by the instructor pausing for questions, calling on students, or transitioning to a retrieval slide. In an async setting (a recorded lecture or a self-paced slide deck), segmentation is enforced by the artifact itself — a "pause and try this" slide, a chapter break, a question that won't advance until answered. The segmenting principle is the cognitive-science version of "15-minute chunking" as a deck-design rule.

The empirical anchor for the "15 minutes" figure is mixed. The number circulating in pedagogy literature comes from various sources (Hartley & Davies 1978 on attention; Bligh 2000 *What's the Use of Lectures?*; Guo et al. 2014 on edX video engagement at 6–9 minutes). The Guo et al. number is more precise but is for asynchronous video, not live lecture. For live lecture, "15–20 minutes between consolidation moments" is a working rule, not a settled finding. [verify the exact 15-minute claim against Bligh or a more recent source before stating as fact]

**Common misconception:** "Segmenting means making slides shorter." The principle is about *the learner's pace*, not slide count. A 50-slide deck can be poorly segmented (continuous lecture with no pause points) and a 20-slide deck can be well-segmented (clear consolidation moments at slides 7, 14, and 20).

**Worked example:** A faculty member converts a 50-minute lecture to a Loom recording. The recording is a single 50-minute clip with no breaks. Mayer's Segmenting Principle predicts (and the data confirm) that retention will be worse than the same content delivered as five 10-minute clips, each with a question between them. The slide artifact has to enforce segmentation; the live instructor's pauses are gone.

**Source:** Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Chapter 9: Segmenting and Pre-training Principles.

### A5. The hidden curriculum — who is the deck for?

The chapter's deepest move is naming the silent decision behind every slide deck: is this for the syllabus or for the learner? Faculty default to syllabus-coverage because syllabi are the visible institutional artifact — they get reviewed, accredited, complained about when topics are missing. Student learning is invisible until the exam.

Brown, Roediger & McDaniel (2014) *Make It Stick* puts this bluntly: the things instructors do that *feel* like teaching (fluent presentation, comprehensive coverage, immediate feedback) often correlate negatively with retention. The things that produce retention (retrieval practice, spacing, desirable difficulty) often feel harder for both instructor and student. The faculty member optimizing for the experience of the room is sometimes optimizing against the learning of the students in it.

The Brutalist move is to make the question explicit. For this deck: *what should the student be able to do after this lecture?* If the answer is "recognize the terms," the deck is fine as a coverage artifact. If the answer is "produce a regression analysis," "diagnose a market failure," "explain why a vaccine works" — the deck has to be rebuilt around the production.

**Common misconception:** "I have to cover the syllabus or I'll get in trouble." Often true at the level of *topics listed*. Rarely true at the level of *time allocated per topic*. A deck can hit all syllabus topics and spend 70% of its time on the three the students actually need to build a schema around, 30% on the rest. That is teaching with coverage as a constraint, not coverage as the goal.

**Worked example:** An intro biology deck has to cover photosynthesis, respiration, mitosis, and meiosis (syllabus). The students need to be able to compare photosynthesis and respiration as inverse processes (deep schema) and tell mitosis from meiosis (recognition). The deck spends 30 of 50 minutes on photosynthesis-and-respiration (the schema work) and 20 minutes on mitosis-meiosis (the recognition work). Coverage: all four topics present. Teaching: built around what the student needs to *do*.

**Source:** Brown, P. C., Roediger, H. L., & McDaniel, M. A. (2014). *Make It Stick: The Science of Successful Learning*. Belknap Press / Harvard University Press. [hup.harvard.edu/books/9780674729018](https://www.hup.harvard.edu/books/9780674729018)

---

## B. Domain examples and cases

### Case 1: The 60-slide deck of a 90-page chapter

A finance instructor generates a deck from chapter 14 of a corporate finance textbook (capital structure). Gamma produces 60 slides that walk the chapter section by section: Modigliani-Miller assumptions, no-tax case, with-tax case, financial distress, pecking order theory, signaling, agency costs. Each topic gets a clean slide. The deck is comprehensive. After the lecture, students cannot answer a basic question: "should a firm with stable cash flows take on debt?" The deck covered the answer but did not build it. The fix: organize around the one decision the student should be able to make (debt vs. equity for a given firm), and pull in the theory in service of that build.

### Case 2: The textbook table of contents as deck outline

A neuroscience deck mirrors the textbook chapter headings exactly: anatomy, function, neurotransmitters, disorders, treatments. The textbook organizes this way because the reader can flip back and forth. The lecture deck has no flipping — the student moves linearly through the sequence. The textbook order assumes random access; the deck has only sequential access. Backward design would ask "what should the student understand?" and might land on disorders-first (a hook) or anatomy-as-needed (build in dependency order from a particular disorder backward to its mechanism).

### Case 3: The Hook / Build / Consolidate restructure

A statistics deck that opened with "the central limit theorem states..." is restructured. The new opening is a question: "I roll a six-sided die 100 times and average the rolls. I roll it 10,000 times. Which distribution is more concentrated around 3.5?" Students vote. The CLT is then introduced as the explanation for why both distributions are concentrated and one more so. Build: sampling distribution, standard error, the n→∞ result. Consolidate: a new question students attempt before leaving — "if I want my standard error to halve, how many additional samples do I need?" The same content, sequenced backward from what students should be able to do.

### Failure case: the "comprehensive review" deck

End-of-semester review deck, 100 slides, covers the whole course. Students complain it was "useful but overwhelming." Retention on the final is no better than for students who got no review deck at all. The deck failed because it imported the coverage logic to a context where consolidation was the actual job. A 20-slide deck of *retrieval prompts* — questions the students attempt cold, with answers revealed only after attempt — would have outperformed the 100-slide review on the metric that mattered (final exam performance). The instructor optimized for "did I review everything?" rather than "did the students practice retrieval?"

---

## C. Connections and dependencies

**Prerequisites (from earlier chapters):**
- Chapter 7 (Seductive Details): the diagnostic question "which learning objective does this serve?" generalizes from element-level to deck-level. Chapter 8 applies it to entire slides and entire sections, not just images and text.
- Chapter 1 (Slideument): the awareness that one deck can have multiple jobs sets up the live-vs-async distinction that Chapter 9 makes explicit.
- Chapter 3 (Too Much Text): density at the deck level (too many slides) is the deck-scaled version of density at the slide level.

**Unlocks (for later chapters):**
- Chapter 9 (Live vs. study artifact): the natural next move. Once the reader has accepted that the deck has a job, the question becomes *which* job — and one deck cannot do both.
- Chapter 10 (Headline That Says Nothing): the assertion-evidence headline is the slide-level expression of "what should this slide make the student think?" — same question, slide scale.
- Chapter 11 (Owning Your DESIGN.md): the deck-opening convention and retrieval-prompt template become reusable defaults the reader can encode.

**Adjacent chapters:**
- Chapter 7 is the immediate paired chapter. Both Ch 7 and Ch 8 are "more = less learning" findings — Ch 7 about decorative additions, Ch 8 about comprehensive sequencing. The shared insight: subtraction is often the corrective move.

---

## D. Current state of the field

**Settled:**
- Retrieval practice produces better long-term retention than restudy (Karpicke & Roediger 2008 and dozens of replications).
- Distributed practice beats massed practice (Cepeda et al. 2006 meta-analysis, 839 effects).
- Worked examples reduce intrinsic load for novice learners (Sweller's research program, ~40 years of evidence).
- Backward design is the dominant framework in K–12 curriculum development (Wiggins & McTighe, two editions, broad adoption).

**Contested:**
- The exact "chunking" interval. Working memory limits are well-established (Miller's 7±2 revised to ~4±1 by Cowan), but how that maps to lecture-time chunking is less precise.
- Whether "hook with a problem" works across all content types. Some highly cumulative domains (formal mathematics) may require building before a problem can be posed.
- The strength of online vs. F2F learning. Means et al. (2010) found small advantages for online and blended learning over pure F2F, but the effect is contested and depends heavily on what's being compared. [ed.gov/media/document/evaluation-of-evidence-based-practices-online-learning-meta-analysis-and-review-of-online-learning-studies-revised-september-2010-107159.pdf](https://www.ed.gov/media/document/evaluation-of-evidence-based-practices-online-learning-meta-analysis-and-review-of-online-learning-studies-revised-september-2010-107159.pdf)

**Key references:**
1. Wiggins, G. & McTighe, J. (2005). *Understanding by Design* (2nd ed.). ASCD.
2. Karpicke, J. D. & Roediger, H. L. (2008). The critical importance of retrieval for learning. *Science*, 319, 966–968.
3. Cepeda, N. J., Pashler, H., Vul, E., Wixted, J. T., & Rohrer, D. (2006). Distributed practice in verbal recall tasks: A review and quantitative synthesis. *Psychological Bulletin*, 132(3), 354–380.
4. Bjork, E. L. & Bjork, R. A. (2011). Making things hard on yourself, but in a good way. In *Psychology and the Real World*.
5. Brown, P. C., Roediger, H. L., & McDaniel, M. A. (2014). *Make It Stick*. Belknap Press.

**Recent developments (last 3 years):**
- Retrieval-based learning has consolidated as a research program — see the "Retrieval-Based Learning: A Decade of Progress" review.
- Active-learning research continues to show large effects in STEM education (Freeman et al. 2014 PNAS, subsequent replications). [verify for relevance to Ch 8 specifically — may belong more in Ch 9]
- A 2023 meta-analysis of retrieval-practice in classroom settings (vs. lab) confirms the effect, with smaller magnitude than lab studies. [verify exact citation]

---

## E. Teaching considerations

**Where faculty stick:**
1. "I have to cover the syllabus." The hidden curriculum problem. Address by separating *topics included* from *time allocated*.
2. "Students need a complete reference after the lecture." Conflates live deck with study artifact. Punt to Chapter 9 — that distinction is the next chapter's job.
3. "Hook with a problem feels like I'm wasting time." The opening-problem move feels like delay; the evidence shows it accelerates schema construction.
4. "Retrieval practice in lecture is just calling on students." Voluntary participation is not retrieval practice. Every student has to attempt, not just the ones who raise hands.
5. Sunk-cost in existing decks. Restructuring is expensive; the chapter has to make the restructure feel tractable — usually by restructuring only the opening five slides.

**Analogies:**
- *Architecture vs. inventory.* A house is not a list of materials. A house is materials arranged for the people who will live in it. A textbook chapter is inventory. A lecture deck is architecture.
- *A meal vs. a grocery list.* The grocery list is comprehensive — it has to be, you can't go back. The meal is curated — only what serves the dish.
- The chapter's bridge from Chapter 7 is the strongest single move: both are "more = less learning" findings. Chapter 7 is slide-level subtraction (decorative content). Chapter 8 is deck-level subtraction (comprehensive coverage).

**Exercises:**
1. *Warm-up:* Take a deck's table of contents. For each topic, write what the student should be able to *do* with that topic. If the answer is "know about it," flag.
2. *Application:* Take a deck's opening five slides. Rewrite them as Hook / Build / Consolidate. The rewrite should preserve no slide unchanged.
3. *Synthesis:* Map a 50-minute deck to the timeline. Mark every slide where consolidation could occur. Insert at least two retrieval prompt slides.
4. *Challenge:* Defend the original deck against the restructure. What does the original sequence do that the restructure loses? (This is the chapter's "two people disagree" move.)

---

## F. Library files relevant to this chapter

- **`pantry/lecture-slides-deep-research.md`** — sections on chunking and sequencing (lines 82–96), retrieval practice and active learning (lines 98–112), common instructional design mistakes (lines 115–123). All directly relevant.
- `pantry/_lib_Teaching-for-Deeper-Learning.md` — likely overlaps with Wiggins & McTighe / backward design. Cross-reference.
- `pantry/_lib_Building-Thinking-Classrooms.md` — task-design literature; relevant for the "build in dependency order" move.
- `pantry/_lib_EdTech.md` — relevant for AI-tool failure framing (the tool generates topic-by-topic by default).
- `pantry/brutalist/DESIGN.md` — operationalizes the deck-opening convention and the retrieval-prompt slide template.

---

## G. Gaps and flags

- **FLAG:** The "15–20 minute chunking" rule is widely cited but the empirical anchor is loose. Hartley & Davies (1978), Bligh (2000), and various attention-research papers contribute but no single study establishes the number cleanly. Guo et al. (2014) found 6–9 minutes optimal for *online video*, which is shorter. The chapter should state the rule with appropriate calibration — "the working-memory and attention research supports periodic consolidation; the exact interval is less settled than the principle." [verify before stating "15 minutes" as a hard rule]
- **FLAG:** Wiggins & McTighe is a K–12 curriculum design framework imported to higher education. The move is defensible but not automatic. Some higher-ed instructors will push back on the import. The chapter should acknowledge the source domain and defend the generalization.
- **FLAG:** "Backward design" sometimes gets conflated with "constructivism" or "active learning" as a single bundle. Wiggins & McTighe are specifically about *outcome-first design*, which is compatible with traditional lecture if the lecture is designed backward from outcomes. Don't let the framing collapse into "lectures are bad."
- **GAP:** The chapter implies that coverage-organized decks have lower retention than arc-organized decks. Direct empirical comparison of deck-organization-type on retention is thin in the literature. The claim is supported by the *components* (retrieval practice works, schema construction works, etc.) but not by a study that compares "coverage deck" vs. "arc deck" head to head. [verify — there may be a Freeman or Wieman study that comes closer]
- **GAP:** The book's diagnostic move ("what should the student be able to do?") is closer to learning-objectives pedagogy than to Wiggins & McTighe specifically. The Bloom-revised taxonomy (Anderson & Krathwohl 2001) is the more precise reference for the action-verb framing if the chapter wants to cite it. [verify whether the chapter wants to go this direction]
