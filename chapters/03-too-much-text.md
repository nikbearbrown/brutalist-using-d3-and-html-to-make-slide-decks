# Chapter 3 — Too Much Text

> A slide that looks like a page is three different failures wearing one face — which one is yours?

---

## 1. The feeling

You paste the section from chapter 4 of your textbook into Gamma. You tell it to "make a slide on this topic." Gamma returns a slide that looks like a clean rendering of the textbook paragraph — single-spaced, 18pt, formatted as flowing prose with one bolded term. The slide has a small title. Below the title is the entire paragraph.

You preview the slide. You think *good — the content is here*. You move to the next one.

In lecture, you project the slide. A student in row three reads it. She is still reading it forty seconds later when you have moved on to your second sentence of explanation. She is now lost — partway through your spoken sentence, partway through the slide's third sentence, encoding neither well. The student in row twelve has given up on reading the slide (too small, too dense) and is half-listening. The student in the back row has stopped listening entirely and is on her phone, because nothing on the screen rewards looking up.

Two weeks later you ask the class a question whose answer was in that paragraph. Nobody can answer it. You think *they didn't study*. The truth is the slide ate the lecture and the lecture ate the slide and neither of them landed.

The slide looks like a page. That is the feeling. It is also three different failures, and the prompt that fixes one will not fix the others.

## 2. The two diagnostic questions

Always two, always in this order.

**From cognitive science:** *Can a student read this slide and listen to me at the same time?* The honest answer for anything above roughly forty words is no — not because students are weak, but because the verbal and visual working-memory channels saturate quickly. Reading prose forces both channels into the visual one (decoding text is visual processing routed through phonological working memory), which is the same channel your spoken words use. Two streams, one pipe, the student suppresses one. Usually you.

**From visual design:** *What is the one thing this slide is asserting?* If you cannot finish the sentence "this slide asserts that ____" in ten words, the slide has no claim. A slide with no claim has nothing to compress *around*, which means the text on it has no center of gravity, which means you cannot decide which sentences are load-bearing and which are along for the ride.

## 3. The principle named

Plain language: **"too much text" is not one problem. It is three, and each one needs a different cut.**

- **Type 1 — redundancy.** The text duplicates what you are about to say out loud. Verbal channel collides with itself. (Same mechanism as Chapter 1, now diagnosed slide by slide.)
- **Type 2 — seductive detail.** The text is interesting but not essential to the learning objective. The student remembers the anecdote, not the structural claim. (Mayer's Coherence Principle territory.)
- **Type 3 — density.** The text is all essential, but it arrives as a single working-memory load. The student saturates before they finish reading. (Sweller and Mayer's split-attention and segmenting territory.)

Different mechanisms, different fixes. Type 1 you delete from the slide and move to notes. Type 2 you delete entirely (or relegate to "background" in notes). Type 3 you split — across two slides, or progressively revealed.

In framework vocabulary, these are three Mayer principles meeting at one slide. The Redundancy Principle (identical narration + on-screen text degrades learning) names Type 1 ([Mayer & Johnson, 2008](https://doi.org/10.1037/0022-0663.100.2.380); [Mayer, *Multimedia Learning*, 3rd ed., 2020](https://www.cambridge.org/core/books/multimedia-learning/E64FFFAB9D984ECCFEA38D63A9DAA4E5)). The Coherence Principle (extraneous material reduces learning even when it is interesting) names Type 2, anchored by Harp and Mayer's seductive-details experiments ([Harp & Mayer, 1998, *Journal of Educational Psychology*](https://doi.org/10.1037/0022-0663.90.3.414); [Rey, 2012 meta-analysis, *Educational Research Review*](https://doi.org/10.1016/j.edurev.2012.05.003) `[verify DOI]`). The Segmenting Principle and the split-attention effect — essential content presented all at once is worse than the same content in sequence — name Type 3 ([Sweller, Ayres, & Kalyuga, *Cognitive Load Theory*, 2011](https://link.springer.com/book/10.1007/978-1-4419-8126-4); [Tindall-Ford, Chandler, & Sweller, 1997](https://doi.org/10.1037/1076-898X.3.4.257) `[verify DOI]`).

The diagnostic test that picks among the three: ask, for each text element, *what would happen if I deleted this?* If the spoken lecture becomes incoherent without it — load-bearing, keep it (and consider whether the speaker really needs to say it aloud, or whether the slide is saying it for them). If the lecture is intact but a flourish is missing — seductive, cut. If everything is necessary but the slide is overwhelming — segment.

## 4. Bad example

The slide is a content slide from a deck on the 2008 financial crisis. The body is a paragraph the AI tool produced from the textbook chapter. Word count: 119 on the slide body alone, 134 with the title.

A detailed prose mockup, with line-by-line annotation. The slide as rendered would look like this:

---

> **Title (28pt, bold):**
> The Subprime Mortgage Crisis and Its Causes
>
> **Body (18pt regular, full-width paragraph, single-spaced, justified):**
> The subprime mortgage crisis emerged in the United States between 2007 and 2010, triggered by a sharp decline in home prices that followed nearly a decade of rising house values. Lenders had expanded mortgage origination to borrowers with weaker credit profiles — so-called *subprime* borrowers — often through adjustable-rate mortgages whose initial low payments reset to substantially higher payments after two to three years. When the housing market peaked in 2006 and began to decline, these resets coincided with declining home equity, producing widespread defaults. Lehman Brothers, founded in 1850 by Bavarian immigrants and one of Wall Street's oldest investment banks, filed for bankruptcy on September 15, 2008, an event widely regarded as a turning point in the crisis.

---

Now the line-by-line audit.

- **Title — "The Subprime Mortgage Crisis and Its Causes."** A topic label, not an assertion. The student leaves the slide knowing the slide was *about* the crisis. They do not leave with a claim about it. (This is also a Chapter 10 issue but it surfaces here because a slide with no central claim cannot resist seductive details — they have nothing to compete *with*.)
- **Sentence 1 — "The subprime mortgage crisis emerged in the United States between 2007 and 2010..."** Type 1 (Redundancy). This is exactly what the speaker will say. The student reads "between 2007 and 2010" while the speaker says "between 2007 and 2010." The verbal channel collides with itself for two beats.
- **Sentence 2 — "Lenders had expanded mortgage origination to borrowers with weaker credit profiles..."** Type 1 again, but with a Type 3 wrinkle. The sentence contains four pieces of structural information (subprime defined, ARM defined, reset window, payment magnitude). On the page in a textbook, the student can re-read. On the slide, in fifteen seconds, while you talk over them, they cannot process four facts at once. This is what split-attention looks like at the sentence level — essential, dense, and presented in a configuration the working memory cannot handle without help (segmenting, layering, or moving to notes).
- **Sentence 3 — "When the housing market peaked in 2006 and began to decline..."** Type 1 again. The speaker will deliver this verbatim.
- **Sentence 4 — "Lehman Brothers, founded in 1850 by Bavarian immigrants..."** Type 2 (Seductive detail). The 1850 / Bavarian immigrants clause is interesting and irrelevant. Harp and Mayer ran six experiments on lessons exactly like this, and the version with the entertaining anecdote produced roughly *one-third* the retention of structurally important content compared to the stripped version ([Harp & Mayer, 1998](https://doi.org/10.1037/0022-0663.90.3.414)). The mechanism, in their language, is *diversion*: students form mental models around the interesting material and integrate the core content poorly. The effect is strongest when seductive details appear early in instruction (which this does — slide one or two of the deck), when prior knowledge is low (introductory undergraduates), and when intrinsic load is already high (a four-fact opening sentence — see Type 3 above). All three conditions are present. This is the textbook configuration for damaging learning.
- **Whole slide.** 119 body words, single-spaced 18pt, justified — visually a paragraph from a page. The student reads it like a page (slowly, sequentially) while the speaker delivers it like a lecture (in real time). Two cadences, one screen, no win condition.

The slide is *complete*. It is also failing in three distinct ways at once. The cure for any one of them is different from the cure for the other two. If the faculty member's diagnosis is just "too much text," they reach for a single fix — usually "less text" — and end up with a sparser slide that still has the same three problems in miniature.

## 5. Good example

Same content. One headline assertion + a short evidence list. Three diagnoses, three cuts.

The slide as rendered:

---

> **Headline (44pt, bold, full sentence):**
> Subprime ARM resets met falling home equity — defaults followed.
>
> **Body — three bullets (22pt regular, with generous spacing between):**
> - **Borrowers:** weaker credit, adjustable-rate mortgages.
> - **Trigger:** ARM resets coincided with 2006 price peak.
> - **Result:** widespread defaults, 2007–2010.
>
> **Notes field (visible only to the speaker; exported with slide for async study):**
> Between 2007 and 2010, the subprime mortgage crisis emerged in the United States, triggered by a sharp decline in home prices following a decade of rising values. Lenders had expanded origination to subprime borrowers — weaker credit profiles — often through adjustable-rate mortgages whose low introductory payments reset to substantially higher payments after two to three years. When the housing market peaked in 2006 and began to decline, the resets coincided with declining home equity, producing widespread defaults. Background: Lehman Brothers' September 15, 2008 bankruptcy is the canonical inflection point of the crisis; the firm was founded in 1850.

---

What changed, by diagnosis.

- **Type 1 cut (Redundancy).** Every sentence the speaker was going to deliver verbatim moved off the slide and into the notes field. The slide now carries labels and a claim — not narration. The speaker can talk over the slide without colliding with it.
- **Type 2 cut (Seductive detail).** The 1850 / Bavarian immigrants clause is gone from the slide. The Lehman date is in the notes, marked "Background" so the speaker knows it is optional. The interesting material is recoverable for the curious student studying from the export, and absent from the live deck where it would otherwise capture schema-building attention away from the structural claim.
- **Type 3 cut (Density).** The four-fact opening sentence is segmented into three labeled chunks (Borrowers / Trigger / Result). The student can take in one chunk while the speaker explains it, then move to the next. Segmenting Principle: same content, sequenced into working-memory-sized loads instead of arriving as one wall.

Word count on the live slide body: 27. Word count on the headline: 9. Total visible on the slide during lecture: 36. The notes field carries 100+ words of full prose for whoever needs it later. Same source, two products — the live-deck and the study artifact — neither of which lies about the content.

The interesting part is what changed about the *headline*. "The Subprime Mortgage Crisis and Its Causes" was a topic label. "Subprime ARM resets met falling home equity — defaults followed" is a claim. Once the headline is a claim, every body element has a job to do: explain *which borrowers*, *what trigger*, *what result*. The headline made the diagnosis possible. Without a claim, the chapter's three-failure-mode test cannot be run — the slide has no center to measure other elements against.

## 6. The prompt

Paste this into the Brutalist system. The principles are portable to any AI slide tool — only the system name changes.

```
Audit this slide for text density using the three-failure-mode test.
For each text element on the slide:

1. Is this text repeating, word-for-word or in paraphrase, what the
   speaker will say aloud? If yes — TYPE 1 (Redundancy). Move it to
   the notes field.

2. Is this text interesting but not essential to a stated learning
   objective for this slide? If yes — TYPE 2 (Seductive detail).
   Remove it from the slide. If it has any retention value at all,
   move it to the end of the notes field under "Background."

3. Is this text essential but presented as a dense paragraph or
   complex multi-fact sentence? If yes — TYPE 3 (Density). Segment
   it into 2–6 short bullets (<= 8 words each) organized by category
   labels, or split the slide into 2–3 slides revealing the content
   in sequence.

After auditing, rewrite the slide to these constraints:

- One headline as a full-sentence assertion (<= 12 words).
- At most six bullets at <= 8 words each, supporting the headline.
- No body paragraph. No prose blocks. Diagrams or labeled images
  preferred where they can carry the structural relationship.
- Move the full reading text to the notes field.

Return the slide as Brutalist HTML with the .slide and .notes
structure preserved. List, in a comment at the top, which failure
mode (1/2/3) applied to each cut.
```

The audit step is the point. A naive "reduce text" prompt cuts indiscriminately. The three-failure-mode audit produces principled cuts you can defend — and, more important, principled relocations, so the seductive Bavarian-immigrants clause is not lost (some students want it in study; nobody wants it in lecture) but also is not allowed to compete for the learning objective's attention.

## 7. The DESIGN.md change

Two variables, tied together. One sentence on each.

```
bullet_word_limit: 8                  # was: unlimited
body_text_density_max: 60_chars       # was: unlimited (consistent with Ch 1)
```
`[verify variable naming against Brutalist DESIGN.md conventions. If your
system uses a single density variable rather than two, set one cap and
document the bullet rule in a comment.]`

Why these two: a hard cap on bullet length forces the slide author to compress to the load-bearing phrase, which forces the question *what is this bullet's job* to be answered before the bullet renders. A character cap on the slide body forces the question *what belongs on the slide versus in the notes* — which is the slideument diagnosis from Chapter 1, applied at the variable level. The two caps together produce slides whose density cannot accidentally drift back to paragraph form between drafts.

Reynolds' worked examples in *Presentation Zen* typically run 5–15 words per slide; Kosslyn endorses a max of 4 bullets at 4 "information units" each — roughly 30–50 words ([Kosslyn, *Clear and to the Point*, 2007](https://global.oup.com/academic/product/clear-and-to-the-point-9780195320695)) `[verify URL]`. Practitioner consensus puts the live-delivery range at roughly 30–50 words per slide; above 75 words you have built a document. Treat the caps as a forcing function, not a sacred number.

## 8. The diagnostic questions to keep

Run any slide through these. If two or more answers say "yes I have that problem," do the audit before you cut anything.

1. **For each text element: which learning objective does it serve?** If the answer is *general context* or *it's interesting*, you have a seductive detail. Cut, or move to notes background.
2. **Is any text on this slide a sentence I am about to say aloud?** If yes, Type 1 redundancy. The slide is not a teleprompter — that is what the notes field is for.
3. **Is any single sentence carrying three or more pieces of structural information?** If yes, Type 3 density. Segment into labeled chunks or split the slide.
4. **Is the total word count above ~50 for a live-delivery slide?** Not automatic failure — but a signal that the audit is worth running before lecture.
5. **If I removed each text element and asked "did the lesson lose anything?" — for which elements is the answer no?** Those are the cuts. The exercise of forcing yourself to answer per-element is the teaching; it's what builds the eye for next time.

## 9. What two people might disagree about

Two faculty can agree the slide has too much text and disagree honestly about the cure. The disagreement worth naming sits between two real schools, neither wrong.

**The Reynolds-style ultra-sparse approach.** Garr Reynolds' [*Presentation Zen*](https://www.presentationzen.com/) advocates slides that approach the limit — one image, one short phrase, sometimes a single word — paired with a speaker who carries the full explanation. The aesthetic is image-led; the slide is closer to a magazine cover than a textbook page. Reynolds defends this on grounds the Modality Principle supports: narration + visual dominates text + visual for novice learners, and the speaker's spoken explanation does work the slide cannot.

**The Atkinson / Alley assertion-evidence approach.** Cliff Atkinson's [*Beyond Bullet Points*](https://www.microsoftpressstore.com/store/beyond-bullet-points-9781509302987) `[verify URL]` and Michael Alley's assertion-evidence work (see [Garner & Alley, 2013, *International Journal of Engineering Education*](https://www.ijee.ie/) `[verify URL]`) prescribe a headline that is a full sentence asserting a claim, supported by sparse evidence — bullets, yes, but bullets of evidence beneath an assertion, not bullets standing alone. The result runs higher word count than Reynolds (20–40 words per slide is typical) but is more structured and arguably more teachable in technical fields where the claim itself is non-trivial.

Both approaches outperform the bullet-only topic-header slide that AI tools default to. Both share the diagnostic the chapter teaches — the three failure modes, the audit, the relocation to notes. Where they disagree is the upper bound on text, and the resolution depends on the discipline and the audience. The vocabulary the disagreement needs: *is the headline a label or a claim, and how much evidence does the audience need to see while the speaker explains it?* Reynolds-camp answers "minimal — I am the evidence." Atkinson-camp answers "enough that the student can follow the structural argument in real time without me reading the slide to them."

Most faculty will land somewhere in between, and the chapter is fine with that. The point is not the word count. The point is that the slide's text has been audited — type by type — and the cuts have reasons.

Sometimes the text is right but the visual form is wrong — a list of relationships that should be a diagram, or a comparison that should be a table. That is Chapter 4.

---

**What would change my mind:** A controlled study comparing the three-failure-mode audit against naive "reduce text" prompts in actual lectures, finding that the principled audit produces no measurable improvement in retention over a simple word-count cap. I am not aware of such a study. The audit is grounded in three well-replicated principles (Redundancy, Coherence, Segmenting) but the *combined* claim — that distinguishing the three modes matters more than just reducing density — is mine, not measured.

**Still puzzling:** I do not have a clean rule for how dense a notes field needs to be before it substitutes for a textbook chapter. The chapter's prescription is "as dense as the textbook section it replaces" but that is qualitative. Whether students actually study from notes-field exports — and how much density they tolerate there — is, to my reading, not yet measured at the granularity faculty would want.

**Tags:** redundancy-principle, coherence-principle, seductive-details, Harp-Mayer, segmenting-principle
