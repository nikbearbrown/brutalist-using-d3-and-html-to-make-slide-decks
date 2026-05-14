# Chapter 6 — The Textbook Figure on the Slide

> A figure that works in a textbook fails on a slide. The reasons are not aesthetic. The fix has four operations.

---

## 1. The feeling

You are sitting in the back of a 200-seat lecture hall. The instructor projects a slide. The slide is a metabolic pathway — glycolysis, say, from the OpenStax [*Biology 2e* §7.2](https://openstax.org/books/biology-2e/pages/7-2-glycolysis). The figure is the canonical one. Ten enzymatic steps. Substrate names. Enzyme names. ATP and ADP boxes. Curved arrows showing electron transfers. Color-coded compartments. Reaction conditions in italics.

The instructor talks for eight minutes. You spend the first thirty seconds trying to read the labels. The labels are too small. You give up and try to follow what the instructor is saying. They are pointing at the screen. You cannot tell where they are pointing. You wait for the slide to change.

You learn nothing about glycolysis from that slide. You may learn that your instructor knows glycolysis. That is a different lesson.

That is the feeling this chapter is about, and it is also the feeling about to be repeated across every figure-heavy lecture in every science, engineering, and medicine course that imports figures directly from textbooks into slides. The figure looks authoritative. The figure looks complete. The figure is unreadable.

This chapter sits at a pivot. The five chapters before it built the eye for individual slide failures: slideument, hierarchy, text density, wrong form, color. This is the last of those — the highest-stakes individual-slide failure mode, the one that takes the most time to fix and produces the largest gain when you do. Chapter 7 turns the unit of analysis from slide to deck. The questions stop being "what is wrong with this slide?" and start being "what is wrong with this sequence?" The transition is announced in the interstitial that follows this chapter. Mark this as the last slide-level chapter; the rest of the book is about decks.

---

## 2. The two diagnostic questions

**Cognitive science question:** *Can the student process this in the time they will look at it?*

The Pre-Training and Segmenting principles in Mayer's *Multimedia Learning* are both pointed at the same constraint: working memory has a hard limit, and complex visual material plus narration plus unfamiliar vocabulary saturates it within seconds. The [Pre-Training Principle](https://pmc.ncbi.nlm.nih.gov/articles/PMC10845804/) says that people learn better when they already know the names and characteristics of the main concepts before the lesson begins. A figure with twelve unfamiliar labels imposes pre-training failure at projection speed: the student is parsing what each term means while also trying to follow the speaker's narration while also trying to extract the structure of the figure. Three tasks, one working memory, no room.

**Visual design question:** *Is this figure designed for a slide, or for a textbook with a caption and the reader's time?*

A textbook figure has things a slide figure does not have: a caption that names the structures, several minutes of dwell time, the option to re-read, a reading distance of about fourteen inches. A slide figure has the speaker's narration, a few seconds of attention, a viewing distance of fifteen to sixty feet, and no caption at all. Same image. Different medium. Different reading conditions. A figure designed for one medium imports its *form* into the other and discards its *conditions*. The form fails because the conditions are gone.

Always both questions. Always in that order. The cognitive science tells you why the figure cannot survive unredesigned. The visual design tells you what to change.

---

## 3. The principle named

Plain language first: **figures travel poorly between media.** A figure that works in a textbook does not work on a slide. The fix is not "make it bigger." The fix is four operations: crop, enlarge, signal, simplify.

Framework vocabulary: this is Mayer's Pre-Training, Segmenting, and [Spatial Contiguity](https://pmc.ncbi.nlm.nih.gov/articles/PMC10845804/) principles operating together. Pre-training says the figure cannot ask the student to learn vocabulary *and* follow the argument at the same time; either the vocabulary is loaded ahead of the figure or it is cut from the figure. Segmenting says a complex figure should be revealed across multiple slides rather than dumped on one, so the student builds the structure in their head one piece at a time. Spatial contiguity says labels go *on* the elements they refer to, never in a separate legend that requires the eye to make two trips.

And it is [Colin Ware](https://shop.elsevier.com/books/information-visualization/ware/978-0-12-812875-6) on perceptual primitives. The visual system processes a handful of basic features in parallel before conscious attention engages — color, orientation, motion, size, contrast. A figure that uses those features for signaling (an arrow in the accent color pointing at the one thing the slide is about) gets free cognitive bandwidth. A figure that uses none of those features — uniform color, uniform size, uniform contrast everywhere — gives the student nowhere to land.

It is also Tufte in his most operational form. The textbook figure has a high data-ink ratio for its medium. Projected, it does not. The cropped, simplified, signaled slide version has a higher data-ink ratio *for the slide medium*. The figure is the same in the abstract. The figure as a perceptual object is different.

---

## 4. Bad example

A biochemistry course slide. The instructor's learning objective is "students should be able to identify the three regulated steps of glycolysis and explain why each is regulated."

```
+----------------------------------------------------------+
|  Glycolysis                                              |
|                                                          |
|  [a screenshot of the OpenStax Biology 2e figure         |
|   showing all ten steps of glycolysis:                   |
|     - 10 enzyme labels in 7pt projected (~12pt scaled)  |
|     - 10 substrate names with structural diagrams        |
|     - ATP/ADP boxes between each relevant step          |
|     - phosphate group annotations                        |
|     - Pi labels                                          |
|     - NAD+/NADH labels between steps 6 and 7            |
|     - curved arrows showing electron transfers           |
|     - color coding: substrates in green, enzymes in blue,|
|       energy in red — no key, all three colors           |
|       distributed across the figure with no obvious      |
|       hierarchy                                          |
|     - a small caption at the bottom: "Figure 7.7         |
|       Glycolysis (OpenStax Biology 2e)"]                 |
+----------------------------------------------------------+
```
<!-- annotation: figure scaled to fit the slide width. Original labels at 7pt in the textbook, scaled to about 12pt on a 10-inch slide. Projected on a 12-foot screen, viewed from the back row at 50 feet, those labels are below the angular resolution of typical 20/20 vision. Most of the class cannot read them. -->
<!-- annotation: figure shows ten enzymatic steps. The learning objective requires three of them. Seven steps are noise relative to the lecture's claim. The student spends working memory parsing all ten before realizing only three matter. -->
<!-- annotation: pre-training failure. The student needs to know what hexokinase, phosphofructokinase, and pyruvate kinase are *before* the figure is useful — but the figure introduces twenty unfamiliar terms simultaneously, with no scaffolding. Working memory saturates within thirty seconds. -->
<!-- annotation: no signaling. There is no visual indication that hexokinase, phosphofructokinase, and pyruvate kinase are the three the slide is making a claim about. The student has no entry point. -->
<!-- annotation: color in the figure is decorative (or at least decorative-at-projection-distance) — three colors with no key, and the color encoding from the textbook chapter does not map to the lecture's claim about regulation. -->
<!-- annotation: spatial contiguity is fine inside the figure (labels are next to their elements), but the figure is so dense that contiguity is not the binding constraint. Density is. -->
<!-- annotation: the figure is authoritative. It is also unusable. The instructor talks to it for eight minutes. The students wait it out. -->

The failure here is not careless. The instructor chose a high-quality figure from a reputable open-source textbook. The figure is correct. The figure is comprehensive. The figure is exactly the figure a student should study before an exam, *at their desk, with the chapter in hand, for thirty minutes*. Those are not the conditions of a lecture slide.

This is the failure mode AI tools have made worse, not better. Asked to generate a slide about glycolysis, Gamma will produce something like the slide above — a figure dropped onto a slide, scaled, with no operations applied. The tool is biased toward "complete-looking" output. Completeness in a textbook is rigor. Completeness on a slide is failure.

There is also the AI-generated variant of this failure, which deserves one sentence: AI image generators produce figures that *look* like textbook figures — boxes, arrows, labels, color coding — but encode nothing. The arrows connect arbitrary cells. The labels are typographic shapes resembling words but are not real terms. The figure has the appearance of a metabolic pathway and the content of static. AI-generated diagrams amplify the textbook-figure-on-a-slide failure by adding a new failure underneath it: there is no figure to redesign because there was never a figure. There was an image of a figure. The fix is to throw it out and use a real figure from a real source.

---

## 5. Good example

Same learning objective. Same source. Four operations applied.

```
+----------------------------------------------------------+
|  The three regulated steps of glycolysis are             |
|  irreversible — and the cell controls flux at each one.  |
|                                                          |
|        [a simplified diagram: three labeled boxes        |
|         in a horizontal sequence, with arrows between]   |
|                                                          |
|    Glucose ──▶  G6P  ──▶  F1,6BP  ──▶  PEP  ──▶  Pyruvate|
|                  ↑          ↑                  ↑         |
|                  │          │                  │         |
|              [hexokinase] [PFK]         [pyruvate kinase]|
|              (24pt, red)  (24pt, red)   (24pt, red)      |
|                                                          |
|              [each labeled "STEP 1", "STEP 3", "STEP 10" |
|               beneath the enzyme name, 18pt gray]        |
|                                                          |
|    [Figure adapted from OpenStax Biology 2e §7.2]       |
+----------------------------------------------------------+
```
<!-- annotation: title is now a full-sentence assertion (Chapter 10 territory, but illustrated here because the figure redesign reaches for it). The slide is making a claim. -->
<!-- annotation: Operation 1 — Crop. The slide shows the pathway as a single horizontal chain from glucose to pyruvate. Of the ten enzymatic steps in the original, only the three regulated ones are highlighted with enzyme names. The other seven are present in the chain (Glucose → G6P → F1,6BP → PEP → Pyruvate is not anatomically every intermediate; it is the simplification) but not labeled. -->
<!-- annotation: Operation 2 — Enlarge. The three enzyme labels are at 24pt. The substrate labels are at 18pt. All labels are above the threshold for last-row legibility on a typical 12-foot screen at 50 feet. -->
<!-- annotation: Operation 3 — Signal. The three regulated enzymes are in the accent color (red from Chapter 5's palette). The arrows pointing to them are in the same accent. The eye lands on the three things the slide is making its claim about within the first second of looking. -->
<!-- annotation: Operation 4 — Simplify. Seven labels removed. The structural diagrams of intermediate molecules are removed. The ATP/ADP boxes are removed. The Pi labels, the NAD+/NADH labels, the electron-transfer arrows — all removed for this slide. They will return on subsequent slides if they are part of subsequent claims; they are not part of *this* claim. -->
<!-- annotation: the figure is now reading-ready in five seconds. Glance test passes. -->
<!-- annotation: attribution is preserved ("adapted from OpenStax Biology 2e"). The original figure's structural information that this slide does not show is not falsified — the slide does not claim that glycolysis has only four steps; it claims that the three regulated ones are the load-bearing points. -->
<!-- annotation: this is one slide in what may be a four-slide segmented sequence. A subsequent slide adds the ATP/ADP boxes — yield. A subsequent slide adds the NAD+/NADH — redox. A subsequent slide returns to the full ten-step figure now that the student has the regulatory framework loaded. That is Mayer's Segmenting Principle in operation: same content, distributed across slides so working memory can build the schema one piece at a time. -->

What changed: the figure dropped from twenty visible labels to four primary ones plus three regulatory labels. The figure's structural information for the lecture's claim — *which steps the cell controls* — became visible at a glance. The other thirteen labels did not disappear from the pathway; they disappeared from this slide. They are in the textbook. They are in the notes field. They may be on subsequent slides. They are not on the slide making this claim.

There is a limit. Simplification can cross into distortion. A figure that removes so much that it misrepresents the relationships between the remaining elements is not a better figure — it is a misleading one. The simplified glycolysis above keeps the directionality (glucose → pyruvate) and the regulatory structure (three points where flux is controlled). It does not falsify the pathway. If the simplification had, say, omitted the step where ATP is consumed and shown only the steps where ATP is produced — "glycolysis makes ATP" — that would have distorted the energy bookkeeping of the pathway and produced a worse student understanding, not a better one. Name the limit every time. The honest move when simplification would distort is to either segment across more slides or to send the student to the textbook for the full figure. Either is better than a slide that teaches the wrong thing simply.

---

## 6. The prompt

Paste this into the Brutalist system on any slide that contains a figure imported from a textbook, paper, or AI image tool.

> Look at this figure. Answer one question before any redesign: which three or four elements of the figure carry this slide's specific claim?
>
> Apply four operations.
>
> 1. **Crop.** Show only the part of the figure that serves the current learning objective. Remove sections of the source figure that are about other things.
> 2. **Enlarge labels.** Replace small labels with labels readable from the back row — minimum 18pt on the rendered slide, larger where the slide will be projected at scale. Use the figure_label_size_min variable.
> 3. **Signal.** Add an accent color, arrow, or callout to direct attention to the three or four elements the slide is making its claim about. Use the accent color from DESIGN.md.
> 4. **Simplify.** Remove labels and annotations that do not serve this slide's objective. If a label is on the original figure for a different chapter's purpose, it does not belong on this slide. Move excised content to the notes field or to a subsequent slide.
>
> If the figure has more than four primary elements the slide is making a claim about, build a 2-to-4 slide sequence that introduces the elements progressively (segmenting). Do not put it all on one slide.
>
> If simplifying would distort the relationships in the figure — change what the figure asserts — stop. Either segment across more slides or send the student to the source figure for full context. Never produce a figure that simplifies into misrepresentation.
>
> Preserve attribution. Cite the source figure on the slide ("adapted from [source]") or on the deck's final attribution slide.

The prompt is portable. The Brutalist system can render the redesigned figure directly in D3/HTML. In Canva or Gamma, the same four operations apply as instructions to whatever the tool produces — they will produce a less precise version, but the diagnostic was the hard part.

---

## 7. The DESIGN.md change

```yaml
# DESIGN.md
figure_element_max_per_slide: 4
figure_label_size_min: 18pt          # rendered slide size; back-row legible
figure_signaling_color: "{{palette.accent}}"  # red from Chapter 5
figure_attribution_required: true

figure_rule: "Imported figures must be redesigned for the slide medium.
              Apply crop / enlarge / signal / simplify. Maximum 4 primary
              elements on a single slide; segment across slides if more
              elements are needed. Simplification must not distort the
              relationships in the original. Attribution required."
```

One sentence why each variable matters:

- `figure_element_max_per_slide: 4` — beyond four elements, working memory saturates within the figure alone, before the speaker's narration is integrated. The number comes from working-memory chunk limits (~4 ± 1), translated into the slide medium.
- `figure_label_size_min: 18pt` — below this, the back row of a typical classroom cannot read the label. Practitioner consensus is around 1/30 of screen height as a rule of thumb; 18pt rendered at typical slide proportions is at or near that floor.
- `figure_signaling_color` inherits from the palette accent — the accent's job here is the same as everywhere else in the deck, so the figure participates in the deck's consistent signaling rather than introducing a new color.

The reader's DESIGN.md may have different specific values. The discipline is that figure redesign is a default expectation, not an exception. Importing a figure unredesigned is the failure mode the variable exists to prevent.

---

## 8. The diagnostic questions to keep

Run these on any slide that contains a figure.

1. **Was this figure designed for print or for projection?** If it came from a textbook, a paper, or a textbook screenshot, it was designed for print. It needs the four operations. There is no exception.

2. **Can a student in the last row read every label?** If not, the labels do not exist for them. The fix is either enlarge or remove. There is no version where small unreadable labels stay on a slide.

3. **Is there a visual signal directing attention to the specific claim this slide is making?** If the student does not know within two seconds where to look, the signal is missing. Add an accent, an arrow, or a callout.

4. **Have I removed labels and annotations that do not serve this slide's claim?** Every element on a figure should be earning its place against this specific slide's objective. Elements from the source figure's other purposes are noise here.

5. **Does any simplification I have applied distort the relationships in the figure?** Cutting irrelevant labels is fine. Cutting elements that change what the figure claims about the system is not. Name the limit.

6. **If this figure has more than four primary elements I need, am I segmenting across multiple slides — or am I dumping it all on one?** Segmenting is the legitimate alternative to losing information. Animation built around segmenting is one of the few uses of animation Mayer's research supports.

---

## 9. What two people might disagree about

Two reasonable instructors will disagree about how aggressive simplification should be.

One position: the textbook figure is the complete picture, and students should see the complete picture early. Exposure to complexity builds tolerance for complexity. Simplification spoon-feeds students and produces graduates who are surprised by real-world complexity. The recommendation: keep more of the original figure than the four-element rule suggests, and trust students to manage the load.

The other position: working memory limits are not optional. A student who is overloaded does not learn complexity-tolerance; the student stops paying attention. Mayer's research consistently finds that scaffolding through simplification produces better long-term learning, particularly for novices. The recommendation: aggressive simplification at first encounter, with the full figure returning later in the lecture sequence (after the student has the scaffolding in place to absorb it).

The empirical evidence favors the second position for novice learners. The first position has merit for advanced learners and for the *return to the full figure* later in the sequence. Both can be right at different points in the build. The vocabulary for the disagreement is *prior knowledge* and *intrinsic load*: a student who already has the schema can absorb the full figure; a student building the schema for the first time cannot.

A second disagreement: whether AI-generated figures are ever acceptable as instructional visuals when they are decorative rather than load-bearing. One position: any visual stimulus aids engagement, even a decorative one. The other position: the Coherence Principle plus the seductive-details research (Harp & Mayer 1997/1998) argues the opposite — decorative visuals on instructional slides reduce retention. The book takes the second position. The reader is welcome to take the first if they can defend it in those terms.

A note on copyright. Reusing a textbook figure in a teaching slide is a common case under U.S. fair use, and the redesign operations in this chapter generally strengthen the fair use argument by transforming the figure for an educational purpose. The legal details — the four-factor test, the CONFU guidelines, the TEACH Act for online instruction — are covered in Appendix B, not here. One sentence is the rule: attribute the source, redesign for teaching purposes, and the practice is on solid ground in standard classroom contexts. If you are recording the lecture for public posting, the fair use argument weakens — that is also in Appendix B.

---

You have been looking at slides.

A slide with a clear hierarchy, the right visual form, color that encodes one thing well, a figure redesigned for the last row. You can now see these things and name them. That is the eye this book set out to build. Six chapters in, you have it.

The next four chapters are about a different problem. A deck of individually well-designed slides can still fail to teach. The failure mode is no longer the slide. It is the sequence. The opening that does not hook. The build that skips a dependency. The deck organized around the textbook's headings rather than the learner's mental model. The deck that is meant for live delivery and also expected to work as a study artifact, doing neither well.

The unit of analysis shifts. The diagnostic questions shift with it. Everything you built in Chapters 1 through 6 still applies — a deck of bad slides is still a deck of bad slides — but a deck of good slides in the wrong order, covering content the learner is not ready for, ending before anyone has to use anything, is a deck that covers without teaching.

That is the failure mode Chapter 7 addresses.

---

**[verify]** APCA's current normative status in WCAG 3.0 (mentioned briefly in Ch 5 cross-reference); believed still draft in 2026 but worth confirming.

**[verify]** Specific URL stability for the OpenStax Biology 2e §7.2 glycolysis figure cited in the worked example; OpenStax pages have stable URLs but the specific figure number (7.7 or 7.8 depending on edition) should be confirmed in the published version.
