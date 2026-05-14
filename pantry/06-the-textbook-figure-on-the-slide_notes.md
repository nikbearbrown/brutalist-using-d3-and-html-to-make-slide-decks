# Research Notes: Chapter 6 — The Textbook Figure on the Slide

**Source:** TIKTOC.md chapter entry
**Notes file:** 06-the-textbook-figure-on-the-slide_notes.md
**Corresponding chapter:** chapters/06-the-textbook-figure-on-the-slide.md (not yet written)
**Generated:** 2026-05-13

**Note:** This is the FIRST ACT TWO chapter. Per TIKTOC §"Three-Act Learning Arc," the transition from individual-slide diagnostics (Ch 1–5) to deck-level diagnostics begins immediately after this chapter, but Chapter 6 itself is the special case at the slide level — the textbook figure that fails on projection. It is also a hinge chapter: per TIKTOC Open Question 3, self-contained, design perspective only, not which tool, not how to use the Brutalist graphicacy book.

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns why direct textbook-to-slide figure transfer always fails and what four operations to specify in a prompt to redesign the figure for projection.

**The feeling:** A figure that looks authoritative and complete but is somehow impossible to see from more than two feet away. Labels too small. Too much labeled. No signal about where to look.

**Why it always fails:** Textbook figures are designed for print — high resolution, small size, studied closely and re-read. Slides are projected large and viewed briefly. They are different media. A figure that works in one medium fails in the other without redesign.

**The four operations:**

*Operation 1 — Crop:* Show only the part that serves the current learning objective. A full-system diagram in a lecture about one subsystem is noise. Crop to the subsystem.

*Operation 2 — Enlarge labels:* Replace small print labels with labels that pass the last-row test. If a student in the last row cannot read the label, the label does not exist.

*Operation 3 — Signal:* Add color, arrows, or callout boxes to direct attention to the specific point this slide is making. The audience cannot study the figure — they can only follow where you point.

*Operation 4 — Simplify:* Remove labels that do not serve the current objective. A neuroscience diagram labeled for a textbook chapter on the full nervous system should have all but two things removed for a lecture slide on the autonomic system.

**The limit:** Simplification can cross into distortion. A figure that removes so much that it misrepresents the relationship between the remaining elements is not a better figure — it is a misleading one. Name this limit explicitly every time.

**Prompt category:** Figure redesign — specify the four operations with the specific labels to keep, remove, and add.

**DESIGN.md variable:** Figure label font size; signaling color conventions for figures.

**Bridge:** The slide eye is built. Chapters 7–9 shift to the deck — failure modes that only appear when you look at the full sequence.

---

## A. Conceptual foundations

### 1. Print and projection are different media

The chapter's central claim is media-specific: a figure that works in a textbook does not work on a slide *because the reading conditions are different*. A textbook is held about 14 inches from the reader's eye. The reader controls dwell time — they can stare at a figure for five minutes, refer back, trace a pathway with a finger, re-read the caption. Resolution is high (300+ DPI on print, comparable on a tablet). The figure is designed to *reward* sustained close study — labels are small because the whole figure is small relative to the visual field, but the small label is sharp.

A slide is projected onto a wall 15–60 feet from the viewer. Resolution at projection scale is much coarser. Dwell time is dictated by the speaker, often a few seconds. The viewer cannot zoom in, cannot trace, cannot re-read. The visual field includes the speaker, the room, the other students. A figure designed for the textbook's reading conditions imported unchanged into the slide's reading conditions imports the *form* and discards the *conditions*. The form fails because the conditions are gone.

This is not a design preference. It is a physical and physiological fact about how reading distance and dwell time interact with visual acuity. The 20/20 standard means a typical observer resolves a one-arc-minute feature at 20 feet. At classroom-back distances (often 30–60 feet), label heights below roughly 1.5–2 inches on a projected screen become unreadable for the back rows. Most textbook figure labels, projected at typical slide scale, fall well below that threshold.

**Common misconception:** "Just make the slide bigger." Scaling a textbook figure up scales the whole figure, including its margin, white space, and unrelated content. The labels are still small relative to the figure, just bigger absolutely. The problem is not size; it is the *ratio of label to figure to projected scale*.

**Worked example:** A textbook figure of the Krebs cycle is 4 inches wide on the printed page with 8pt labels. Scaled to fill a 10-inch slide, labels become 20pt. Projected to a 12-foot screen and viewed from 50 feet, that 20pt is the angular equivalent of 8pt on a printed page held at 24 inches — still legible at a desk, illegible from the back of the lecture hall.

**Source:** General visual acuity / angular subtense reasoning is standard ophthalmology; the practitioner-level treatment for slides is in Reynolds, G. (2019) *Presentation Zen* (3rd ed.) and Tufte, E. R. (2006) *Beautiful Evidence*, Graphics Press.

### 2. Mayer's Pre-Training Principle

Mayer's Pre-Training Principle states that people learn better from a multimedia lesson when they already know the names and characteristics of the main concepts before the lesson begins. The principle's force is that working memory cannot simultaneously (a) parse what a new term means and (b) follow the argument that uses the term. Pre-loading the term names and definitions frees working memory to do the harder integration work during the main lesson.

Applied to figures on slides: a complex figure with twelve unfamiliar labels imposes pre-training failure at projection speed. The student is trying to read the labels, look up each one mentally, and follow the speaker's narration — three tasks simultaneously, all on working memory. Pre-training would mean: introduce the key terms on a previous slide, define them, *then* show the figure. The figure now lands on a working memory that has the names already loaded; the labels become recognition cues, not parsing problems.

This is also why Operation 4 (simplify) is so high-leverage. Removing labels for terms the lecture is not about reduces the pre-training burden to only the terms that matter. The student has to load three names, not twelve.

**Common misconception:** "The full figure is more rigorous." A figure that overloads working memory and produces no learning is not more rigorous. It is more comprehensive and less effective. Rigor in instruction is measured by what the student can do afterward, not by how much was on the slide.

**Worked example:** A neuroanatomy lecture on the autonomic nervous system. The textbook figure labels every cranial nerve, every plexus, every ganglion — twenty-plus labels. Pre-training-respectful design: a prior slide names the four structures the lecture is about (sympathetic chain, parasympathetic outflow, two named ganglia). The figure on the next slide highlights those four. The other sixteen labels are removed.

**Source:** Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.), ch. 8 on Pre-Training. https://pmc.ncbi.nlm.nih.gov/articles/PMC10845804/

### 3. The Segmenting Principle and progressive disclosure of figures

Mayer's Segmenting Principle states that people learn better when a complex multimedia lesson is broken into learner-paced parts rather than presented as a continuous unit. The mechanism: working memory limits make continuous complex input impossible to integrate; segments give the learner time to build a schema for one part before adding the next.

For figures on slides, segmenting is concrete: rather than showing the full figure once, build it across two to four slides. Slide 1: the skeleton (axes, frame, or main structure with no labels). Slide 2: add the primary elements with labels. Slide 3: add the secondary relationships (arrows, connections). Slide 4 (if needed): annotated highlight of the specific element this lecture is about. Each slide is a digestible segment; the cumulative effect is the full figure, built in the student's head with comprehension at each step.

This is also the operational answer to "but the figure has too many parts to leave out." If every part matters, segment over time rather than dump at once. Animation-as-segmenting is one of the few legitimate uses of slide animation — not for delight, but for working-memory management. Mayer's research consistently finds that segmented presentation outperforms continuous presentation for complex content (effect sizes vary, but the direction is robust).

**Common misconception:** "Animation is decoration." Mayer's Coherence Principle does cut decorative animation. But *pedagogically motivated* segmentation — building a figure step by step to manage working memory — is the opposite. The animation is doing essential work.

**Worked example:** A signal-transduction pathway with seven components. Dumped on one slide: working-memory failure for most students. Segmented across four slides: receptor on slide 1, two downstream components on slide 2, the second messenger system on slide 3, the cellular response on slide 4. The student builds the pathway alongside the speaker. The final slide is the full figure, but the cognitive cost of arriving there was distributed.

**Source:** Mayer, R. E. (2009) *Multimedia Learning* (2nd ed.), ch. 9 on Segmenting.

### 4. The Spatial Contiguity Principle

Mayer's Spatial Contiguity Principle states that people learn better when corresponding words and pictures are presented near each other rather than far apart on the page or screen. The mechanism is search cost: when a label and the thing it labels are separated, the student spends working memory looking for one to match the other instead of integrating the two.

Textbook figures usually respect spatial contiguity — labels are immediately adjacent to the structures they name, or arrows-with-labels point to specific features. Slide failures often violate spatial contiguity when a figure is captioned by a separate text block ("Figure shows: A is the cell membrane, B is the nucleus, C is the cytoplasm") rather than by inline labels. The student has to look at the figure, then look at the caption, then look back at the figure — three eye-movements per element. This is pure extraneous load.

The operational fix in the chapter's four operations: in Operation 2 (enlarge labels) and Operation 3 (signal), labels and signaling marks must be placed *on* the figure, adjacent to what they refer to. Never as a separate caption block. Never as a key in the corner. The label sits next to the thing.

**Common misconception:** "A clean figure with a legend is more elegant." Elegance is not the criterion. Integration is. A legend in the corner with seven entries forces seven matching operations between figure and legend, each consuming working memory.

**Worked example:** A bar chart with five categories. Bad: a color legend in the upper right pairing colors to category names. Good: each bar labeled directly underneath. Same information, half the cognitive cost.

**Source:** Mayer, R. E. (2009) *Multimedia Learning* (2nd ed.), ch. 5 on Spatial Contiguity. Practitioner translation in Reynolds (2019) *Presentation Zen*, 3rd ed.

### 5. Ware on perception, Few on dashboards — the supporting frame

Colin Ware's *Information Visualization: Perception for Design* (4th ed., Morgan Kaufmann, 2020) grounds the slide-figure redesign claims in the perceptual neuroscience of how the visual system actually processes images. Three Ware-derived points the chapter can lean on: (1) pre-attentive processing handles roughly five to seven basic features (color, orientation, motion, size, contrast) in parallel before conscious attention engages — figures that use these features for signaling get free cognitive bandwidth; (2) the visual cortex's bias toward edges and high-contrast boundaries means clean lines and high contrast are not aesthetic preferences but perceptual primitives the eye locks onto; (3) chunking in visual perception works the same way as in working memory — grouping elements through proximity, color, or shape reduces the number of items the eye has to process.

Stephen Few's *Now You See It* (Analytics Press, 2009; 2nd ed. 2021) extends these perceptual principles to dashboards — multi-element instructional surfaces designed for quick comprehension. The slide-as-figure case shares the dashboard's constraint: limited viewing time, high information density, viewer scanning for one specific thing. Few's principles around scan paths, callouts, and emphasis transfer directly.

The chapter does not need to lecture on perception, but the four operations have a perceptual basis worth referencing once: cropping respects the foveal limit; enlarging labels respects angular resolution; signaling uses pre-attentive features; simplifying respects working memory chunking.

**Source:** Ware, C. (2020). *Information Visualization: Perception for Design* (4th ed.). Morgan Kaufmann. https://shop.elsevier.com/books/information-visualization/ware/978-0-12-812875-6 — Few, S. (2009/2021). *Now You See It*. Analytics Press. https://analyticspress.com/nysi.php

---

## B. Domain examples and cases

### Case 1: The biochemistry metabolic pathway dump (failure case)

A faculty member in a biochemistry course is teaching glycolysis. They open the OpenStax *Biology 2e* chapter on cellular respiration (https://openstax.org/books/biology-2e/pages/7-2-glycolysis) and screenshot the figure showing all ten steps with substrates, enzymes, ATP/ADP balance, and structural diagrams of intermediate molecules. The figure is dropped on a slide, scaled to fit. Twenty-plus labels in 6pt-equivalent type after projection. The instructor talks through it for eight minutes.

What students see: a colorful chemistry diagram. What students retain: nothing specific. Working memory saturates within the first thirty seconds of trying to read the labels while listening. The student stops trying to integrate and waits for the slide to change. The instructor is talking to a figure the audience cannot process.

Fix using the four operations: (1) *Crop* to the three steps the lecture's learning objective is actually about (the regulated steps — hexokinase, phosphofructokinase, pyruvate kinase). (2) *Enlarge* the three remaining enzyme labels and the three substrate labels. (3) *Signal* which step is the rate-limiting one with a red callout. (4) *Simplify* — remove the structural drawings of intermediates that are not under discussion; replace with names only. Result: a slide with three labeled steps, one signaled, all readable from the last row.

### Case 2: A clinical trial flowchart simplified for a 30-second slide (positive case)

A research-methods lecture covers a published trial's CONSORT flow diagram. The original figure (from the paper) has 12 boxes with full enrollment, allocation, follow-up, and analysis counts. The instructor's learning objective is "students should be able to identify why the trial lost statistical power during follow-up." Useful operations: crop to the follow-up and analysis sections; enlarge those boxes' labels; signal the attrition with a red strike-through arrow and a bold count; simplify by removing the allocation section (which is not under discussion). The slide now shows three boxes — enrolled, completed follow-up, analyzed — with the gap between them highlighted. Same information density relevant to the objective, far higher legibility per second of viewing.

### Case 3: AI-generated figure that encodes nothing (failure case, modern variant)

A faculty member asks an AI image generator to produce "a diagram of the immune response." The output is a polished image — cells with labels, arrows connecting them, color-coded compartments. It looks like a textbook figure. On closer inspection, the labels are nonsensical (typographic shapes that resemble words but aren't), the arrows go from arbitrary cells to other arbitrary cells, and the color coding is decorative rather than encoding cell type. The figure has the *appearance* of authority and the *content* of noise. Worse, it looks polished enough that the faculty member and the students both accept it as a figure, and the lecture proceeds as if the figure means what it pretends to mean. The four operations cannot fix this case because there is nothing to crop, enlarge, signal, or simplify — the figure encodes nothing. The fix is to throw it out and use a real figure from a real source.

(This is the one-sentence acknowledgment per TIKTOC Open Question 5 — AI-generated images make the textbook-figure-on-slide failure mode worse because they look authoritative and encode nothing.)

---

## C. Connections and dependencies

**Prerequisites:**
- Chapter 4 (Wrong Visual Form): the general principle of form-fitness. Chapter 6 is the high-stakes special case where the source form was right for one medium and wrong for another.
- Chapter 5 (Color): signaling colors used in Operation 3 depend on Chapter 5's encoding rules. A red callout works because Chapter 5 established what red means.
- Chapter 2 (Hierarchy) and Chapter 3 (Too Much Text): the simplification operation depends on the reader knowing what to cut. Chapters 2 and 3 trained the cutting judgment.

**Unlocks:**
- Chapter 7 (Seductive Details): the simplification operation is a special case of cutting interesting-but-not-essential content. Chapter 7 generalizes the principle to the deck level.
- Chapter 8 (The Deck That Covers but Doesn't Teach): the same diagnostic move applied at deck scale — what serves the learning objective, what is overhead from another medium's structure.
- Chapter 10 (Headline That Says Nothing): the assertion-evidence model often uses a redesigned figure as the evidence. Chapter 6 makes the figure assertion-ready.

**Adjacent chapters:** Chapter 6 closes Act One in the sense that it is the last slide-level chapter. The Act One → Act Two interstitial (per TIKTOC §"Act One → Act Two: From Slide to Deck") follows immediately. The chapter should explicitly hand off to the deck-level perspective at its close.

---

## D. Current state of the field

**Settled:**
- Print and projection are perceptually different media; figures designed for one fail in the other. This is uncontested.
- Mayer's Pre-Training, Segmenting, and Spatial Contiguity Principles are all empirically supported with multiple replications.
- Tufte's principles on figure redesign for new media (chartjunk, data-ink ratio, small effective differences) are widely accepted as defaults.
- Color Oracle and equivalent simulators reveal colorblind failures reliably and are practitioner-standard.

**Contested:**
- How aggressive simplification should be. Some educators argue that exposing students to the full complexity early builds tolerance for ambiguity; others argue (with Mayer) that scaffolding through simplification produces better long-term learning. The empirical evidence favors scaffolding for novices.
- Whether AI-generated figures are *ever* acceptable for teaching when they're decorative rather than load-bearing. Some argue any visual stimulus aids engagement; the Coherence Principle (and Harp & Mayer 1997/1998 on seductive details) argues the opposite.
- Whether building figures over multiple slides (segmenting via animation) is helpful or distracting. The research mostly favors segmentation when it is pedagogically motivated; it usually criticizes segmentation when it is decorative.

**Key references (3–5):**
1. Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press. (Pre-Training, Segmenting, Spatial Contiguity chapters)
2. Tufte, E. R. (1990). *Envisioning Information*. Graphics Press.
3. Tufte, E. R. (2006). *Beautiful Evidence*. Graphics Press.
4. Ware, C. (2020). *Information Visualization: Perception for Design* (4th ed.). Morgan Kaufmann.
5. Few, S. (2021). *Now You See It* (2nd ed.). Analytics Press.

**Recent developments (last 3 years):** Generative AI image tools (DALL-E 2022, Midjourney 2022, integrated into Canva/Gamma 2023–24) have produced a new failure mode: polished-looking figures that encode nothing. The chapter's "AI-generated figure" sentence is the practical acknowledgment. No empirical study located that measures how often AI-generated instructional figures fail the encoding test, but instructor-side reports of the failure are common.

---

## E. Teaching considerations

**Where faculty stick:**
- Faculty believe that simplification is dishonesty. The chapter's "limit of simplification" rule is the right move: simplification that distorts is wrong, but simplification that omits-without-distorting is the responsible move. Naming the limit makes the operation defensible.
- Faculty feel that redesigning a textbook figure is "their" work — they didn't make it, they can't change it. The copyright and attribution piece (Appendix B per TIKTOC) covers the legal side; this chapter focuses on the design move and notes that fair use generally permits redesign for teaching with attribution.
- The "last row test" is unfamiliar. Faculty rarely sit in the back of their own lecture hall and look at their own slides. The exercise of doing so once is the move that converts the abstract principle into a felt diagnostic.

**Analogies that work:**
- *The road sign vs. the map.* A textbook figure is a map — comprehensive, designed to be studied. A slide figure is a road sign — single message, instant comprehension, viewed at speed. You cannot drive at highway speed reading a map.
- *The newspaper vs. the headline.* A textbook is the front page of the newspaper — rich, layered, designed to reward reading. A slide is the headline — one claim, made loud, signed off in seconds. Same story, different form.
- *Re-photographing.* Imagine taking a high-resolution textbook figure and re-photographing it through a frosted lens from across a room. That is what projection does to the original. The redesign is the equivalent of preparing a new photograph for those new conditions.

**Exercises:**
- Take three figures you've used as-is from a textbook in the last semester. For each, apply the four operations on paper. Then compare: what would each redesigned figure tell the student that the original didn't?
- Sit in the back row of your own lecture hall (or stand at projection distance from your screen at home). Project your most figure-heavy slide. List every label you cannot read. Those are the failure cases.
- Run one figure through Color Oracle. Anything that vanishes was encoded in color alone — a Chapter 5 violation visible inside a Chapter 6 case.
- Pick one figure where you would resist simplification ("everything matters"). Write down what each label serves. The ones that don't map to a learning objective for *this* lecture are candidates for cutting.

---

## F. Library files relevant to this chapter

- **`lecture-slides-deep-research.md`** — Section "Redesigning Textbook Figures for Slides" is the direct precursor. Section "Mayer's 15 Multimedia Learning Principles" for Pre-Training, Segmenting, Spatial Contiguity. Section "Where Tools Work Against You" for the AI-tool default angle.
- **`_lib_Surfaces-and-Essences.md`** — Hofstadter & Sander on how the brain handles complex visual analogies; possibly useful for the "what to keep, what to cut" judgment.
- **`_lib_Teaching-for-Deeper-Learning.md`** — likely contains figure-redesign and scaffolding heuristics for K–12 contexts that transfer.
- **`_lib_How-to-Deliver-a-TED-Talk.md`** — Anderson on visual signaling in live talks; practical for the "signal the specific point" operation.
- **`_lib_EdTech.md`** — plausibly relevant for the textbook-to-slide pipeline as an instructional-design problem.
- **`_lib_Thinking-Fast-and-Slow.md`** — Kahneman on visual System-1 processing; useful for justifying pre-attentive signaling.
- **`_lib_Building-Thinking-Classrooms.md`** — Liljedahl on what makes students engage with classroom visuals; flag for relevance.
- **`_lib_The-Digital-Delusion-Horvath.md`** — Horvath on edtech failures of cognitive design; plausibly relevant for the "AI-generated figure that encodes nothing" case.

## G. Gaps and flags

- FLAG: The "always fails" framing in the TIKTOC summary is strong. The chapter draft should soften to "almost always fails without redesign" — there are edge cases (very simple textbook figures with two or three large labels) where the figure can transfer with minimal change. The four operations still apply; sometimes Operations 1 and 4 are zero-cost.
- FLAG: Per TIKTOC Open Question 3, the chapter is explicitly self-contained and does not require the Brutalist graphicacy book. The notes file should not lean on graphicacy-book-level depth on chart construction; the four operations are sufficient.
- FLAG: Copyright treatment of textbook figures — per TIKTOC, this is Appendix B, not Chapter 6. The chapter should not get into fair use; one sentence is enough ("attribution is in Appendix B").
- GAP: No precise empirical threshold located for "label height as fraction of projected screen height" at which legibility from the back row fails. Practitioner consensus is around 1/30 of screen height; this is rule-of-thumb, not measured. [verify if a more precise threshold exists in the readability literature]
- GAP: AI-generated figure failure is observationally common but not measured. The chapter's one-sentence treatment (per TIKTOC Open Question 5) does not require a measured rate.
- GAP: One specific OpenStax pathway figure should be picked for the worked example in the chapter draft. Glycolysis from *Biology 2e* §7.2 is a strong candidate (URL above); the chapter draft should grab the specific figure URL and use it.
