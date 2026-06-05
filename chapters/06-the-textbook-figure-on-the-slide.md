# Chapter 6 — The Textbook Figure on the Slide


## TL;DR

- A figure that works in a textbook fails on a slide.
- The chapter moves through The medium is not the message, but it is the constraint, What makes a figure readable on a slide, The limit that matters, Why the four operations are not obvious, and related ideas.
- Read it for the main argument, the vocabulary it introduces, and the practical judgment it asks you to develop.

*A figure that works in a textbook fails on a slide. The reasons are not aesthetic. The fix has four operations.*

---

You are sitting in the back of a 200-seat lecture hall. The instructor projects a slide. The slide is a metabolic pathway — glycolysis, the canonical one from any standard biology textbook. Ten enzymatic steps. Substrate names. Enzyme names. ATP and ADP boxes. Curved arrows showing electron transfers. Color-coded compartments. Reaction conditions in italics.

The instructor talks for eight minutes.

You spend the first thirty seconds trying to read the labels. The labels are too small. You give up and try to follow what the instructor is saying. They are pointing at the screen. You cannot tell where they are pointing. You wait for the slide to change.

You learn nothing about glycolysis from that slide.

This is not a story about a bad instructor or a bad figure. The figure is excellent — it is comprehensive, accurate, and exactly the figure a student should spend thirty minutes with at a desk, textbook open, on the night before an exam. The instructor chose it for precisely those virtues. And those virtues are the problem. The figure was designed for a different medium, under different reading conditions, with different time available. It traveled into the lecture hall and left its conditions behind. The form arrived. The context did not.

That is the puzzle this chapter is about. Not "how do you make a slide prettier" but something more specific: *why do figures fail when they cross from textbook to slide, and what exactly do you do about it?*

---

## The medium is not the message, but it is the constraint

A textbook figure has things a projected slide does not have. It has a caption that names the structures. It has the reader's time — minutes, not seconds. It has a reading distance of about fourteen inches. The reader can look back and forth between the caption and the elements. They can pause on the part they do not understand. They can re-read.

A projected slide has the speaker's narration, a few seconds of attention before the audience's eyes drift, a viewing distance of fifteen to sixty feet, and no caption. The labels that were legible at fourteen inches are not legible at fifty feet. The detail that rewarded careful study in the book is visual noise at projection distance. The structure that unfolded over minutes in a reading session has to transmit in the first two seconds of a glance.

Same figure. Different medium. The figure is not wrong for the textbook. It is wrong for the slide.

| Item | Meaning |
| --- | --- |
| reading distance, dwell time available, caption present, reader controls pace, label size threshold for legibility, consequence of small labels | A concrete checkpoint for applying the chapter concept. |
| the table should make the medium difference concrete and scannable rather than requiring the reader to hold both sets of conditions in working memory simultaneously | A concrete checkpoint for applying the chapter concept. |

This sounds like a simple observation, but it has a precise cognitive-science translation. Richard Mayer's Pre-Training Principle describes what happens when a student encounters a figure that uses vocabulary they do not yet know: they spend working memory learning what each term means at the same time they are trying to follow the argument the figure is making, at the same time the speaker is narrating. Three tasks. One working memory. None of the three complete.

The Pre-Training Principle says that learning is better when the names and characteristics of the main concepts are loaded *before* the lesson that uses them. A glycolysis figure with twenty unfamiliar labels is not presenting glycolysis to a student — it is asking the student to acquire a twenty-term vocabulary while simultaneously following a biochemical argument while simultaneously attending to a speaker. The failure is not motivational. It is architectural.

Mayer's Segmenting Principle adds the other half: when complex visual material is distributed across multiple slides rather than presented all at once, students build the schema in their head one piece at a time, and working memory stays within its limits. The complete pathway presented in one shot saturates working memory within thirty seconds. The same pathway built across four slides — first the three regulated steps, then the energy yield, then the redox balance, then the integration — gives working memory four separate passes, each one adding to a schema that is accumulating rather than overwhelming.

Both principles point at the same root cause: a textbook figure, imported unredesigned into a slide, asks working memory to do what it cannot do in real time. The figure is not wrong. The import operation is.

---

## What makes a figure readable on a slide

There are four operations. They are not a style preference. They are responses to specific constraints of the projection medium.

**The first is cropping.** A textbook figure typically shows more than any single slide's claim requires. The glycolysis figure shows ten enzymatic steps; a slide about the three regulated steps needs three of them. The other seven are not wrong — they are noise, relative to this slide's claim. Every element a student parses that does not contribute to the current argument is cognitive work extracted from the budget available for the argument itself. Cropping is not simplification for aesthetic reasons. It is the removal of irrelevant cognitive load.

**The second is enlarging labels.** The practical threshold for back-row legibility at a typical classroom viewing distance is around 18pt on the rendered slide — practitioners often state this as roughly one-thirtieth of the screen height. Below that, the label does not exist for the student in the back rows. A label that cannot be read is not a label; it is visual noise that implies information without delivering it. The choice is binary: enlarge it until it is readable, or remove it. There is no version where a small unreadable label earns its place on a slide.

**The third is signaling.** Colin Ware's research on perceptual primitives identifies a small set of visual features that the visual system processes in parallel before conscious attention engages: color, motion, orientation, size, contrast. An element that differs from its surroundings in one of these features is noticed immediately, without deliberate search. An element that does not differ is found only by serial scanning. On a figure with twenty elements and a three-second attention budget, serial scanning means most elements are never found. Signaling — an arrow in the accent color, a callout, a box around the three things this slide is about — redirects that budget to the elements that carry the claim. The student's eye lands on the right thing in the first second, not the fifth.

**The fourth is simplifying.** After cropping to the relevant section and enlarging the labels, there are often still elements in the figure that belong to the textbook chapter's other purposes but not to this slide's claim. Structural diagrams of intermediate molecules. Reaction conditions. Cofactor labels from steps the slide is not making a claim about. These can be removed from the slide without falsifying the figure — they are moved to the notes field, or to a later slide, or are available in the textbook. What remains is the structure the slide is actually claiming.

![Four-panel visual showing the same glycolysis figure section](images/06-the-textbook-figure-on-the-slide-fig-01.png)
*Figure 6.1 — Four-panel visual showing the same glycolysis figure section*

The four operations together convert a figure designed for one medium into a figure designed for another. This is not decoration. It is redesign in response to different reading conditions, different time budgets, and different working-memory constraints.

---

## The limit that matters

There is a limit, and it is important enough to name explicitly.

Simplification can cross into distortion. A figure that removes so much that it misrepresents the relationships between the remaining elements is not a better figure — it is a misleading one.

The simplified glycolysis example keeps the directionality of the pathway (glucose goes to pyruvate, not the other way) and the regulatory structure (three points where the cell controls flux). It does not falsify the pathway. A simplification that, say, removed the ATP-consuming steps and kept only the ATP-producing steps — leaving the student with the impression that glycolysis is a pure energy gain rather than an investment-and-return process — would have produced a worse understanding, not a better one. The figure would be teachable, memorable, and wrong.

The honest move when simplification would distort is to either segment the complexity across more slides or to send the student to the textbook for the full figure. Either is better than a slide that teaches the wrong thing clearly. Clarity and accuracy are not in tension here — a clear distortion is still a distortion. The test to run before finalizing any simplified figure is: *does this slide, read by a student who has not seen the source, give a correct-if-incomplete picture, or a misleading one?* Correct-if-incomplete is fine. Misleading is not.

---

## Why the four operations are not obvious

If the operations are that clear, why do slides with unredesigned textbook figures persist in every course in every institution?

Part of the answer is authorship incentives. The instructor who built the deck over a weekend was looking for the best figure of glycolysis, found the textbook figure, and imported it. The figure looks authoritative. It looks complete. It took five seconds to add. The redesign would have taken forty-five minutes. The instructor did not experience the figure from the back row; they experienced it from their desk at fourteen inches, where it was fine.

Part of the answer is tool defaults. Canva, Gamma, and PowerPoint all make importing a figure trivially easy and make redesigning it require multiple manual operations. The path of least resistance ends at the imported figure, unredesigned.

And part of the answer is a genuine confusion between completeness and quality. In a textbook, completeness is rigor — a figure that shows all ten steps of glycolysis is doing its job. On a slide, completeness is often failure. A slide that shows all ten steps of glycolysis while making a claim about three of them has buried its claim in its own completeness. The instructor's instinct that "more is more accurate" is correct for the medium the figure was designed for and wrong for the medium it landed in.

AI tools have made this worse in a specific way. An AI asked to generate a slide about glycolysis will produce something that looks like the textbook figure — comprehensive, labeled, color-coded — because that is what "a slide about glycolysis" looks like in the training data. The AI has learned the default. The default is the failure. Asking the AI to produce a redesigned figure requires the instructor to know the four operations and instruct explicitly. The tool will execute what it is told; it cannot supply the diagnosis.

There is also a distinct failure that AI image generators introduce. A system asked to produce "a diagram showing glycolysis" will produce something that *looks* like a metabolic pathway — boxes, arrows, enzyme-looking labels — but whose structure encodes nothing. The arrows connect arbitrary boxes. The labels are typographic shapes that resemble biochemical terms but are not accurate ones. The figure has the appearance of glycolysis and the content of noise. The four operations cannot fix this. There is nothing to crop or simplify because there was no correct figure to begin with. The only operation is to throw it out and use a real figure from a real source.

---

## What segmenting actually looks like

The Segmenting Principle deserves more than a mention, because it is the operation most instructors resist and the one most supported by the research.

The resistance is understandable. A sequence of four slides that builds up to the complete glycolysis figure feels like padding. The same information could be on one slide. The instructor knows glycolysis and can hold the complete figure in mind without difficulty; from that vantage, the four-slide build seems slow.

This is the expert blind spot. The instructor is not the audience. The student arriving at the glycolysis figure has not memorized it. They are building the schema in real time, under time pressure, while a speaker is talking. For that student, each slide in the sequence is not padding — it is the working memory reset that lets the next piece land cleanly.

What the sequence might look like: Slide one shows glucose, the three regulated enzymes in accent color, and pyruvate — the regulatory scaffold, nothing else. Slide two adds the ATP investment and return — the energy bookkeeping. Slide three adds the NAD+/NADH accounting — the redox link to the next stage. Slide four returns to the complete ten-step figure, which now makes sense because the student has the schema to hang it on.

![The textbook figure is not discarded. It is deferred to the moment the student is ready for it.](images/06-the-textbook-figure-on-the-slide-fig-02.png)
*Figure 6.2 — Four-panel storyboard of the glycolysis segmented build *

That fourth slide — the complete, unredesigned figure — is now doing legitimate work. The student in the back row looks at it and recognizes it. The vocabulary is loaded. The regulatory structure is loaded. The energy story is loaded. What was unprocessable at the start of the lecture is now a confirmation of what they have been building. The textbook figure is not discarded; it is deferred to the moment when the student is ready for it.

This is Mayer's segmenting logic applied to figures: the same content, distributed across slides so working memory builds the schema one piece at a time, with the full figure returned when the schema exists to receive it.

---

## The seductive complete figure

I want to name one more thing before leaving this chapter, because it operates at a slightly different level from the four operations.

There is a category of figure failure that is not about readability or label size or signaling. It is about the instructor's relationship to comprehensiveness. The figure is on the slide because the instructor wants students to *know* they are in the presence of the complete pathway. The figure signals rigor. It signals that this is a course that takes the material seriously, that does not simplify down to mnemonics and sketches.

That instinct is not wrong. But it is being satisfied by the wrong mechanism. A complete figure on a slide does not communicate rigor to a student in the back row who cannot read the labels. It communicates opacity — the impression that the material is too complex to engage with from a distance. The instructor experiences the figure as a signal of completeness. The student experiences it as a wall.

The thing that communicates rigor is not showing everything at once. It is *building* everything, piece by piece, in a sequence that trusts the student to hold each piece and add the next. A four-slide build that ends with the complete figure is more rigorous than a one-slide complete figure, because it shows that the instructor understands how the knowledge assembles — not just that they know the final state.

Feynman had a version of this. He would say, roughly, that if you cannot explain something to a first-year student, you do not understand it well enough yet. The test of understanding is not being able to show the complete picture. It is knowing what to show *first* — what the scaffold is, what the dependencies are, what a mind that does not yet know the answer needs before it can receive the next piece. A four-slide glycolysis sequence is that test applied. What does the student need to see before the regulatory structure makes sense? Before the energy bookkeeping makes sense? Before the full pathway is legible rather than overwhelming?

Answer those questions, in order, and the slides write themselves.

---

## Two honest disagreements

Two instructors who have read everything above can still disagree.

The first disagreement is about how aggressive simplification should be. One position: students should encounter the complete figure early, because exposure to complexity builds tolerance for complexity. A student who only ever sees simplified figures is surprised by real textbooks, real papers, real data. The other position: Mayer's research consistently finds that scaffolding through simplification produces better long-term learning for novice learners, and the full figure should return after the schema is built rather than before. Both are defensible; the resolution lives in prior knowledge. A student who already has a rough schema of glycolysis can absorb more of the figure at once. A student seeing it for the first time cannot. The diagnostic question is not "what does the complete figure look like" but "what does this particular student already know?"

The second disagreement is about the copyright implications of redesigning figures. Fair use in the United States generally covers the use of textbook figures in teaching, and the redesign operations — cropping, annotating, simplifying — typically strengthen the fair use argument by transforming the figure for an educational purpose distinct from its original context. For publicly posted lecture recordings, the analysis is more complicated. The honest answer is that standard classroom use of redesigned figures with attribution is on solid footing; public posting warrants a closer look. Attribute the source on every slide that uses an adapted figure, redesigned or not. That is both the ethical default and the legal minimum.

---

## What this chapter is the end of

Six chapters have been about individual slides. What is wrong with this slide. The slideument, the hierarchy failure, the text density, the wrong form, the color mistake, the imported figure. The eye built across those six chapters is the eye for a single slide — you can look at a slide now and name what is broken and know what to do about it.

That eye is necessary but not sufficient. A deck of individually well-designed slides can still fail to teach. The failure mode is no longer the slide. It is the sequence — the opening that does not hook, the build that skips a dependency the student needed, the deck organized around the textbook's headings rather than the learner's way of building understanding. A deck of good slides in the wrong order, covering content the learner is not ready for, ending before anyone has to use anything, is a deck that covers without teaching.

The unit of analysis shifts in the next chapter. The diagnostic questions shift with it. But the eye you have built still applies at every slide in the sequence. Good decks are made of good slides in a good order. Both conditions are necessary. You now have one. The next is Chapter 7.

---

**What would change my mind:** A controlled study showing that for novice learners — students with no prior schema for the concept being taught — exposure to the complete unredesigned figure from the start produces equivalent or better transfer performance (tested on new problems, not recognition) compared to a segmented build. Mayer's segmenting research consistently finds the opposite, but that literature uses artificially constructed materials rather than real textbook figures. A study using real figures and real classrooms would be more persuasive.

**Still puzzling:** I do not have a clean rule for how many slides a segmented build should take before the complete figure returns. The Segmenting Principle specifies that segments should be learner-paced when possible (student clicks through), but in live lectures the pace is fixed by the speaker. Whether the timing that works in Mayer's controlled experiments translates to live-lecture conditions — with social dynamics, attention drift, and varying prior knowledge in the room — is not settled in the literature I can name.

---

## LLM Exercises

**Exercise 1 — Medium audit**
Choose any figure-heavy slide from your current deck. Describe the figure to an LLM (or paste a screenshot if the tool accepts images) with this prompt: *"This figure was designed for a textbook at a reading distance of 14 inches. I am projecting it in a lecture hall where the back row is 50 feet away. List every label or annotation in this figure, then flag any that would fall below the 18pt legibility threshold at projection scale. For the flagged labels, recommend: enlarge or remove."* Use the output as a pre-flight checklist before the next lecture.

**Exercise 2 — The four operations applied**
Take a slide that imports a figure unredesigned. Ask an LLM: *"Apply four operations to this figure for use as a lecture slide. (1) Crop: identify which part of the figure serves the slide's specific learning objective and describe what to cut. (2) Enlarge: list the labels that need to be at least 18pt. (3) Signal: recommend where to place an accent-color arrow or callout, and what it should point to. (4) Simplify: list annotations that can be removed from this slide without falsifying the figure, because they belong to other parts of the lesson."* Compare the LLM's recommendations to what you originally showed.

**Exercise 3 — Distortion check**
After applying the four operations to a figure, ask an LLM: *"Here is my simplified version of [source figure]. A student who has never seen the original reads only my simplified version. Does the simplified version give a correct-if-incomplete picture, or does it misrepresent any of the relationships in the original? Identify any elements I removed that were load-bearing for accuracy rather than just completeness."* If the LLM flags a distortion, either restore the element or move it to a segmented follow-on slide.

**Exercise 4 — Segment design**
Take a complex figure you would normally show on a single slide. Ask an LLM: *"Design a three-to-four-slide segmented build for this figure. For each slide, specify: (a) what is shown, (b) what is withheld until a later slide, (c) the learning objective that slide satisfies, and (d) why the student needs that piece before the next piece. The final slide should show the complete figure."* Use the sequence design as a storyboard before building the slides.

**Exercise 5 — AI diagram legitimacy**
Take any diagram produced by an AI image generator (Midjourney, DALL-E, Gamma's image tool, or similar). Ask an LLM: *"For each arrow or connecting element in this diagram, state what specific directed relationship it encodes. If you cannot name the relationship — only that the elements look connected — flag that element as structurally empty. Count total elements and flagged elements. If more than one-third are flagged, the diagram is decorative and should be replaced with a diagram from a verifiable source."*

**Tags:** textbook-figure, Mayer-segmenting, Mayer-pre-training, spatial-contiguity, Colin-Ware, projection-medium, crop-enlarge-signal-simplify

## Prompts

Use these prompts with Claude to generate interactive D3 v7 versions of the
figures in this chapter. Each produces a standalone HTML file you can open
in a browser and modify freely.

**Prerequisites:** Load `brutalist/CLAUDE.md` and `brutalist/DESIGN.md` into
your Claude project context before using these prompts. They define the stack,
naming conventions, color system, and typography the figures use.

---

### Figure 6.1 — Four-panel visual showing the same glycolysis figure section

Create a standalone D3 v7 HTML file for Figure Four-panel visual showing the same glycolysis figure section. Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: four-panel visual showing the same glycolysis figure section at each stage of the four operations — panel 1 (Crop): full ten-step figure with a selection box around the three regulated steps; panel 2 (Enlarge): the cropped section with label sizes increased, unreadable labels called out; panel 3 (Signal): accent-color arrows added to the three regulated enzymes; panel 4 (Simplify): structural diagrams, cofactor labels, and reaction conditions removed, leaving only the core pathway and three labeled regulatory points; each panel labeled with the operation name and a one-sentence rationale. Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variabl

> Reference implementation: `d3/06-the-textbook-figure-on-the-slide-fig-01.html`

---

### Figure 6.2 — Four-panel storyboard of the glycolysis segmented build 

Create a standalone D3 v7 HTML file for Figure Four-panel storyboard of the glycolysis segmented build . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: four-panel storyboard of the glycolysis segmented build — panel 1: the sparse three-enzyme scaffold (Glucose → [HK] → G6P → [PFK] → F1,6BP → [PK] → Pyruvate, accent color on the three enzymes, nothing else); panel 2: same scaffold with ATP/ADP boxes added at the relevant steps; panel 3: same with NAD+/NADH added at step 6; panel 4: the full ten-step textbook figure, now legible because the schema exists; panels connected by a horizontal arrow labeled "working memory accumulates"; caption: "The textbook figure is not discarded. It is deferred to the moment the student is ready for it.". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variables and 

> Reference implementation: `d3/06-the-textbook-figure-on-the-slide-fig-02.html`
