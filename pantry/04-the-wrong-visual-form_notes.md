# Research Notes: Chapter 4 — The Wrong Visual Form

**Source:** TIKTOC.md chapter entry
**Notes file:** 04-the-wrong-visual-form_notes.md
**Corresponding chapter:** chapters/04-the-wrong-visual-form.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns the visual form decision matrix and how to name the mismatch between content type and presentation form precisely enough to prompt the correct fix.

**The feeling:** A slide where the information is right but something about the format makes it hard to see. A list of things that should be connected. A comparison that requires reading back and forth. A process that has no flow.

**The decision matrix:**

| Content type | Right form | Wrong form signal |
|---|---|---|
| Relationships between concepts | Diagram, node map | Bulleted list |
| Processes and sequences | Flowchart, timeline | Numbered list |
| Comparisons of attributes | Table | Side-by-side bullets |
| Trends over time | Line chart | Text description |
| Part-to-whole | Bar chart | Pie chart (usually) |
| Cause-effect mechanisms | Annotated diagram | Paragraph |
| Definitional content | Key term + short phrase | Full sentence |

**Cognitive science failure:** The visual channel is underused. Mayer's Multimedia Principle: words + pictures > words alone. A bulleted list of a process is words alone. A flowchart is words + pictures.

**Visual design failure:** Tufte's data-ink ratio. A list of relationships has infinite ink and almost no data. A node map shows the same relationships with structure the eye can read in seconds.

**The Tufte rule on 3D:** Never. The depth axis adds visual complexity without adding information and actively distorts perception of magnitudes.

**Prompt category:** Visual form replacement — specify the correct form, the content, and the encoding.

**DESIGN.md variable:** Default visual forms per content type (as conventions the reader sets).

**Bridge:** Once the right form is chosen, the question is whether the color in that form is doing work or just decorating. That is Chapter 5.

---

## A. Conceptual foundations

### 1. The Multimedia Principle as form-fitness, not decoration

Richard Mayer's Multimedia Principle is short: people learn better from words and pictures than from words alone. The 2009 second edition of *Multimedia Learning* reports a median effect size of d = 1.39 across 11 experimental comparisons — an effect size that, in education research, qualifies as enormous. What gets less attention is the corollary: the principle does not say "add a picture to your words." It says "the picture must be the right picture for the words." A decorative stock-photo of a brain next to a bulleted list of memory types is not a multimedia treatment. It is a slide with a picture on it.

The diagnostic move for Chapter 4 is therefore not "is there an image?" but "does the visual form match the relationship the content actually has?" A list of three steps in a process *is* the process described in words; a flowchart *is* the process described in words plus an arrow structure that encodes sequence. The flowchart is multimedia. The list is words alone in a font.

**Common misconception:** Faculty often add an image to a slide and assume the Multimedia Principle is satisfied. The principle requires the picture to *correspond* — to encode the same structural information the words encode, so the learner can make connections between channels.

**Worked example:** A slide titled "The Krebs Cycle" with eight bullets naming eight intermediate molecules satisfies no part of the Multimedia Principle. The same content rendered as an annotated cycle diagram with arrows showing transformations — same eight molecules, but their relationships are now visible to the eye — is a real multimedia treatment. Mayer's claim is that the second produces better transfer to new problems, not just better recall of the eight names.

**Source:** Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press. Effect size d = 1.39 cited in National Academies summary at https://sites.nationalacademies.org/cs/groups/dbassesite/documents/webpage/dbasse_072589.pdf

### 2. Cleveland & McGill's ranking of perceptual tasks

In 1984 William Cleveland and Robert McGill published "Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods" in the *Journal of the American Statistical Association* (vol. 79, pp. 531–554). The paper ranked elementary perceptual tasks by how accurately people can decode quantitative information from each. The ranking, in roughly descending accuracy:

1. Position along a common scale (most accurate)
2. Position along non-aligned scales
3. Length, direction, angle
4. Area
5. Volume, curvature
6. Shading, color saturation (least accurate)

This is the empirical foundation for "use bar charts over pie charts" — bars encode magnitude as position along a common scale (rank 1); pie slices encode magnitude as angle and area (ranks 3 and 4). When the faculty member picks a pie chart for a part-to-whole comparison, the chart works against the reader's perceptual system. The same data in a bar chart is decoded faster and more accurately.

**Common misconception:** "It's just a stylistic preference whether you use bars or pies." It is not. The ranking is empirical and replicated. Cleveland and McGill ran controlled experiments on humans decoding visual marks.

**Worked example:** Five departments' budget shares. As a pie chart, the reader squints to compare two slices that look similar. As a horizontal bar chart sorted by value, the comparison is automatic — the eye picks up position-along-a-scale without effort. The data is identical; the cognitive cost is not.

**Source:** Cleveland, W. S. & McGill, R. (1984). Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods. *Journal of the American Statistical Association*, 79(387), 531–554. https://www.tandfonline.com/doi/abs/10.1080/01621459.1984.10478080 — PDF: http://euclid.psych.yorku.ca/www/psy6135/papers/ClevelandMcGill1984.pdf

### 3. Munzner's "what-why-how" framework

Tamara Munzner's *Visualization Analysis and Design* (A K Peters/CRC, 2014) generalizes the form-fit question into a framework: before choosing a visual encoding, decide *what* data you have (categorical, ordered, quantitative; tables, networks, geometry), *why* the user is looking at it (the task — identify, compare, summarize, find anomaly), and only then *how* to encode it. The point: the visual form is a function of data type and task, not aesthetic preference.

For slide design this collapses to a simpler question the faculty member can run in their head: "What is the structural relationship between the things on this slide?" If the answer is "ordered sequence," the form is a timeline or flowchart. If the answer is "set of attributes across categories," the form is a table. If the answer is "trend over time," the form is a line chart. The structure of the relationship determines the form.

**Common misconception:** That picking the visual form is the designer's problem and the instructor just provides content. The structural relationship is in the content — the instructor knows it best. Munzner's framework just makes the choice explicit.

**Worked example:** "Compare three methods of error correction across four properties." The structural answer: a set of attributes across categories. The form: a 3-by-4 table. Anything else (side-by-side bullets, three slides each with bullets, paragraphs) requires the reader to mentally construct the table that was already there in the structure.

**Source:** Munzner, T. (2014). *Visualization Analysis and Design*. A K Peters/CRC Press. Companion site: https://www.cs.ubc.ca/~tmm/vadbook/

### 4. Tufte's data-ink ratio applied to slides

Tufte's foundational concept from *The Visual Display of Quantitative Information* (Graphics Press, 2nd ed. 2001, originally 1983) is the data-ink ratio: the proportion of a graphic's ink devoted to non-redundant data. A high data-ink ratio means most of what is on the page is information; a low ratio means most of what is on the page is decoration, background, or redundant elements competing with the data.

The slide version: a bulleted list of relationships ("X causes Y; Y causes Z; Z feeds back to X") has high ink — every word, every bullet, every line break is a mark — and almost no data structure made visible. The same content as a three-node diagram with two arrows shows the *same information* with a fraction of the marks, and now the cycle structure is visible at a glance instead of requiring the reader to mentally assemble it from text. Tufte's argument is not that diagrams are prettier. It is that they have a higher information-to-mark ratio for the right kind of content.

**Common misconception:** "Tufte says minimize ink." Tufte says minimize *non-data* ink. Adding ink that carries information (a clearer label, an arrow that shows direction) raises the ratio, not lowers it. The rule is not minimalism for its own sake.

**Worked example:** A slide listing five steps of a clinical workflow as numbered bullets. Total marks: roughly fifty words plus five bullet glyphs. As a flowchart with five labeled boxes and four arrows: roughly fifteen words plus eight geometric marks. The flowchart uses fewer marks *and* encodes the sequence structure visually. The data-ink ratio rises.

**Source:** Tufte, E. R. (2001). *The Visual Display of Quantitative Information* (2nd ed.). Graphics Press. https://www.edwardtufte.com/book/the-visual-display-of-quantitative-information/

### 5. The 3D rule

A specific corollary that the chapter should land hard: Tufte's case against 3D charts. The depth axis adds visual complexity without adding information. Worse, perspective distortion makes magnitude comparisons unreliable — bars further from the viewer look smaller than bars closer, regardless of value. 3D pie charts are the worst offenders: the slice nearest the viewer's eye appears proportionally larger. AI slide tools default to "nicer-looking" 3D variants. They are not nicer-looking. They are perceptually broken.

**Source:** Tufte (2001) op. cit.; also covered in Cleveland & McGill (1984) under "volume" being one of the lowest-accuracy perceptual tasks.

---

## B. Domain examples and cases

### Case 1: The history-dates bullet list (failure case)

A history course slide titled "Key Events 1914–1945" with twelve bullets, each beginning with a year. The information is correct. The form is wrong: the structural relationship is temporal sequence with intervals, and bullets erase both the sequence and the intervals. The same content as a horizontal timeline with proportional spacing — 1914, 1917, 1918, 1929, 1933, 1939, 1941, 1945 — shows the *clustering* (interwar gap, rapid escalation 1939–41) that bullets cannot show. Pickering at a slide of dates is not the same cognitive operation as reading a timeline. Cleveland & McGill rank position along a common scale as the most accurate perceptual task; a timeline puts dates on a common axis. Bullets don't.

### Case 2: The methods-comparison table (positive case)

A chemistry course slide comparing three synthesis methods across yield, cost, hazard, and scalability. The instinct is twelve bullets. The right form is a 3-column, 4-row table. The reader's eye scans rows for one property across methods, or columns for one method across properties — two reading directions, one form. Bullets force the reader to mentally reconstruct the table that was already implicit in the content. The table is not extra work for the designer; it is the structural form the content already had.

### Case 3: The AI-tool default failure mode

Canva, Gamma, and Beautiful.ai default to bullet layouts because bullets are the lowest-common-denominator structure that any content can be coerced into. A faculty member asks Gamma for "a slide on the difference between supervised and unsupervised learning," and Gamma produces two columns of bullets. The structural relationship — a set of attributes across two categories — is a table. The AI tool produced bullets because bullets are its default, not because bullets fit the content. The diagnostic the reader needs is: "What is the structural relationship here?" Once they can answer that, they can override the default with a prompt that names the right form.

This is the chapter's portable diagnostic move. The AI tool is not stupid. It is biased toward a single form. The reader needs vocabulary to name what the form should be.

---

## C. Connections and dependencies

**Prerequisites:**
- Chapter 1 (Slideument Problem): the reader can already see when a slide is doing the wrong job. Chapter 4 extends this from "wrong job" to "wrong shape."
- Chapter 2 (Hierarchy): once hierarchy is established, the question of form arises. A clear hierarchy of bullets is still wrong-form if the content is a process.
- Chapter 3 (Too Much Text): Chapter 3 cuts what shouldn't be there. Chapter 4 changes the shape of what remains.

**Unlocks:**
- Chapter 5 (Color): once the form is right, the question of whether color is doing work in that form arises. Color in a chart is encoding; color in a bulleted list is usually decoration.
- Chapter 6 (Textbook Figure): the special case where the content is already in visual form but in the wrong visual form for projection. Chapter 4 establishes the principle; Chapter 6 applies it to a high-stakes special case.
- Chapter 10 (Headline That Says Nothing): the assertion-evidence structure depends on the body being the right visual form. A claim headline over the wrong-form body is still failure.

**Adjacent chapters:** Chapter 4 sits between general slide diagnostics (1–3) and the textbook-figure case (6). It is the chapter that introduces "form" as a diagnostic category.

---

## D. Current state of the field

**Settled:**
- Cleveland & McGill's ranking is replicated and uncontested as a description of human perceptual accuracy on graphical marks. Forty years of subsequent visualization research builds on it.
- Mayer's Multimedia Principle has hundreds of replications and one of the largest effect sizes in instructional design research.
- 3D distorts magnitude judgments. Not contested.

**Contested:**
- Whether the Cleveland-McGill ranking holds when the data is sparse (a few items) versus dense (hundreds). Some research suggests pie charts perform acceptably for two-to-three slice comparisons.
- Whether "chartjunk" (Tufte's term for decorative graphical elements) is always harmful. Bateman et al. (2010) found that some chartjunk improves recall *without* harming comprehension. This is a real wrinkle the chapter should not ignore — Tufte's rule is a strong default, not an absolute.

**Key references (3–5):**
1. Cleveland & McGill (1984), JASA 79(387). Foundational ranking paper. https://www.tandfonline.com/doi/abs/10.1080/01621459.1984.10478080
2. Tufte, E. R. (2001). *The Visual Display of Quantitative Information* (2nd ed.). Graphics Press.
3. Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press.
4. Munzner, T. (2014). *Visualization Analysis and Design*. A K Peters/CRC. https://www.cs.ubc.ca/~tmm/vadbook/
5. Bateman, S., Mandryk, R. L., Gutwin, C., Genest, A., McDine, D., & Brooks, C. (2010). Useful junk? CHI '10. The contested-chartjunk paper.

**Recent developments (last 3 years):** Munzner's framework has become standard in HCI/visualization curricula. The 2020 4th edition of Colin Ware's *Information Visualization: Perception for Design* (Morgan Kaufmann) consolidates the perceptual basis for form selection with updated neuroscience. Generative AI slide tools (Gamma launched 2022, Beautiful.ai expanded its AI features in 2023–24) have made bullet-default failures more common at scale, not less — the diagnostic vocabulary in this chapter is therefore more useful than five years ago, not less. [verify exact Gamma launch date — believed 2022 based on company announcements but worth confirming for the chapter draft]

---

## E. Teaching considerations

**Where faculty stick:**
- Faculty over-trust the structural integrity of bullets. Bullets feel safe — every textbook has them, every slide template has them. The move "bullets are a default, not a form" is harder than it sounds.
- Faculty under-trust their own structural intuition. They know the content has a shape — sequence, comparison, network — but the default tool flattens that knowledge into bullets before they can act on it.
- "Diagram" feels designerly to faculty who don't think of themselves as designers. The chapter should reassure: a diagram with three labeled boxes and two arrows is not a design problem. It is the right form for a three-element causal chain. Brutalist will draw it.

**Analogies that work:**
- *The shape of the content.* Some content has a sequence-shape. Some has a comparison-shape. Some has a network-shape. Bullets are a list-shape. Forcing comparison-shape content into list-shape is the failure mode. The visual form should match the shape the content already has.
- *Translation, not invention.* The faculty member is not inventing a new visual. They are translating a structure that's already in the content into a form that makes the structure visible.

**Exercises:**
- Take three slides from your most recent deck. For each, write one sentence: "The structural relationship between the elements on this slide is _____." Now: does the current form match? If not, what's the right form? Write the prompt.
- Take a textbook chapter heading list. For each subhead, predict the right visual form *before* writing any slide content. The form is in the structure of the topic, not in your design choice afterward.
- Identify one slide in a recent deck that uses a pie chart, a 3D chart, or "side-by-side bullets that should be a table." Convert it. Notice how much faster the new form reads.

---

## F. Library files relevant to this chapter

- **`lecture-slides-deep-research.md`** — Sections "Text vs. Diagram vs. Table vs. Chart" (the decision table this chapter expands), "The Core Principle: Signal vs. Noise" (Tufte), and "Mayer's 15 Multimedia Learning Principles" (the Multimedia Principle). The primary cross-chapter reference; pull the Cleveland-McGill ranking and the Mayer effect size from here rather than re-citing.
- **`_lib_EdTech.md`** — plausibly relevant for the Mayer/multimedia angle in instructional design context.
- **`_lib_Surfaces-and-Essences.md`** — Hofstadter & Sander on analogy and structural mapping. Possibly relevant: the move from "list of relationships" to "diagram of relationships" is a structural-mapping move. Worth a look during drafting.
- **`_lib_Thinking-Fast-and-Slow.md`** — System 1 reads diagrams; System 2 reads bullets. The form-fit argument has a dual-process backbone worth checking against Kahneman.
- **`_lib_How-to-Deliver-a-TED-Talk.md`** — likely contains practitioner advice on visual form selection; flag for skim, not deep read.
- **`_lib_Teaching-for-Deeper-Learning.md`** — McTighe & Silver may have a form-fit framing useful for the "what does this teach?" hook.
- **`_lib_Building-Thinking-Classrooms.md`** — less directly relevant; flag plausibly.
- **`_lib_The-Digital-Delusion-Horvath.md`** — Horvath's critique of edtech defaults likely overlaps the AI-tool-default angle.

## G. Gaps and flags

- FLAG: The chapter's decision matrix (from TIKTOC.md) is broadly defensible but the "Part-to-whole — Bar chart, not pie (usually)" line is the contested one in the visualization literature. Worth a "two people might disagree" pass naming the conditions under which a pie is acceptable (two or three slices, qualitative not precise comparison).
- FLAG: Bateman et al. (2010) "useful junk" paper is a real wrinkle in the Tufte rule. The chapter should acknowledge it rather than pretend the rule is absolute. The honest reading: chartjunk can aid recall for one-off memorable charts; for instructional slides where transfer matters more than recall, Tufte's rule holds.
- GAP: No direct empirical study found that AI slide tools (Canva, Gamma, Beautiful.ai) measurably default to bullets at higher rates than human designers. The claim is observationally true but I have not located a study quantifying it. The chapter should phrase this as observed pattern rather than measured fact, or [verify] with a small audit if Nik wants to make the empirical claim.
- GAP: One sentence on AI-generated images as a Chapter 4 trigger (per TIKTOC.md Open Question 5) — the failure mode is that AI-generated diagrams often *look* like diagrams but encode no real structural information. The arrows go nowhere; the boxes are decorative. The Multimedia Principle is satisfied in appearance and violated in substance. The chapter draft should include this one sentence in "the feeling."
- GAP: Gamma's exact launch date and the timing of Beautiful.ai's AI feature rollout — flagged [verify] in the field-state section.
