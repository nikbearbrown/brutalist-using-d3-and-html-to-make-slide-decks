# Deep Research: Rules & Guides for Making Lecture Slides from Textbook Chapters

Two domains. Both matter. Most bad decks fail the first one.

---

## Domain 1: Instructional Design — The Cognitive Science

### The Foundation: Cognitive Load Theory (Sweller)

All slide design for teaching ultimately derives from **John Sweller's Cognitive Load Theory (CLT)**, first formalized in 1988. The core premise: human working memory has severely limited capacity, and instructional design must respect that limit or learning collapses.

Sweller identifies three types of load:

- **Intrinsic load** — the inherent difficulty of the material itself. You can't eliminate it; you can scaffold it.
- **Extraneous load** — cognitive effort caused by *poor design*. A cluttered slide, redundant text, or a confusing figure all impose extraneous load without contributing to learning. This is the instructor's fault and is entirely preventable.
- **Germane load** — productive cognitive effort that builds schemas and deepens understanding. Good design frees working memory for this.

**Rule:** Your primary job as a slide designer is to reduce extraneous load so students have cognitive resources available for germane load.

---

### Mayer's 15 Multimedia Learning Principles

Richard Mayer built directly on CLT to produce the most empirically grounded set of slide design rules available. His **Cognitive Theory of Multimedia Learning (CTML)** is supported by hundreds of studies. The 15 principles fall into three clusters:

**Reducing Extraneous Load:**
- **Coherence Principle** — remove interesting but irrelevant material (see Seductive Details, below)
- **Signaling Principle** — use visual cues (headings, arrows, highlights) to direct attention to what matters
- **Redundancy Principle** — don't repeat narrated content as on-screen text; it overloads the verbal channel
- **Spatial Contiguity** — place labels and diagrams next to each other, not separated across slides
- **Temporal Contiguity** — show words and images simultaneously, not sequentially

**Managing Intrinsic Load:**
- **Segmenting Principle** — let students control pace; break instruction into learner-paced segments
- **Pre-Training Principle** — teach key concepts and vocabulary before the main lesson
- **Modality Principle** — narration + visuals beats on-screen text + visuals for complex material

**Fostering Generative Processing:**
- **Multimedia Principle** — words + pictures > words alone
- **Personalization Principle** — conversational tone ("you") promotes engagement
- **Voice Principle** — human voice outperforms synthesized voice for narration
- **Embodiment Principle** — on-screen instructors with natural gestures improve learning

**Practical implication for slides:** When you pull a dense textbook section, your job is to strip it to its structural core (coherence), pair concepts with diagrams (multimedia), narrate the detail rather than write it on the slide (redundancy + modality), and sequence it in manageable stages (segmenting).

---

### The Seductive Details Effect — The Most Counterintuitive Rule

Harp and Mayer (1997, 1998) ran six experiments and found consistently that **interesting but irrelevant content actively harms learning.** Students who received a lesson on lightning formation *with* entertaining anecdotes and dramatic photos recalled structurally important content at *one-third the rate* of students who received the stripped-down version.

A subsequent meta-analysis (Rey, 2012) confirmed small-to-medium negative effect sizes on both retention *and* transfer across text-based and multimedia studies.

The mechanism: seductive details cause **diversion** — students form inappropriate schemas around the interesting material and integrate the core content poorly. The effect is strongest when:
- Seductive details appear early in the instruction (not late)
- Students have low prior knowledge
- The intrinsic load of the material is already high

**Rule:** Anything that doesn't directly serve a learning objective should be cut — even if it's interesting, even if it's a good story, even if it "motivates" students. Motivation that comes at the cost of comprehension is a net loss.

**Counterintuitive corollary:** The "fun fact" you put on a slide to warm up the room may be damaging the retention of everything that follows it.

---

### Identifying the "Teachable Core" of a Chapter

Textbooks are written to be comprehensive; lectures are designed to teach. These are different things. A textbook chapter must cover the full territory; a lecture must cause learning. They are not the same operation.

**Process for extracting teachable core:**

1. **Write the learning objectives first.** Before opening the chapter, answer: "What should students be able to *do* at the end of this lecture?" Use Bloom's Taxonomy verbs (explain, apply, analyze, compare, evaluate). The objectives constrain everything else.

2. **Identify structural ideas, not supporting details.** A textbook chapter typically has 3–6 conceptual load-bearing ideas. Everything else is elaboration, example, or context. Find those ideas.

3. **Map content to objectives.** For each piece of content you're considering including, ask: "Which objective does this serve?" If the answer is none, it's a seductive detail.

4. **Distinguish the teaching script from the study artifact.** Slides used during a live lecture serve a different function than notes students study later. A slide in a live lecture should *prompt* your explanation, not contain it. A study artifact contains the explanation itself. Most instructors confuse these and produce "slideuments" — Reynolds' term for the hybrid that does neither job well.

---

### Chunking and Sequencing — Restructuring Chapter Narrative into Lecture Arc

Textbooks sequence content for reference and comprehension reading. Lectures sequence content for *building mental models in real time*. These sequences are often different.

**Lecture arc structure:**
- **Hook** — a problem, question, or phenomenon that creates the need to know. Students learn better when they understand *why* they need the information before receiving it (Kapur's "productive failure" research supports this).
- **Build** — concepts introduced in dependency order: prerequisites before complex ideas, concrete before abstract.
- **Consolidate** — retrieval practice, worked example, or application that forces students to use what they just learned before moving on.

**Chunking rules (from CLT and working memory research):**
- Working memory can hold roughly 4 ± 1 items at once (updated from Miller's original 7 ± 2)
- Each "chunk" of slides should develop one concept before introducing the next
- Optimal video lecture length for retention: 6–9 minutes per chunk (Guo et al., 2014 — MIT/edX data)
- For live lectures: pause or activity every 15–20 minutes to prevent working memory saturation

---

### Retrieval Practice and Active Learning — Embedding Evidence-Based Strategies

The three highest-effect learning strategies from cognitive science research (Dunlosky et al., 2013 meta-analysis):

1. **Retrieval practice** — testing yourself *produces* learning, not just measures it (the "testing effect," Roediger & Butler)
2. **Spaced practice** — distributing study across time produces better retention than massed studying
3. **Interleaving** — mixing problem types or concepts within study sessions outperforms blocked practice

**Practical integration into a slide deck:**

- **Retrieval practice slides:** Every 10–12 slides, include a low-stakes "what do you know so far?" question or brain dump prompt. Research (Lyle & Crawford, 2011) shows that retrieving material at the end of a lecture significantly improves exam performance.
- **Worked examples:** For complex or procedural content, a fully worked example before asking students to attempt a problem reduces intrinsic load and improves transfer (Sweller).
- **Interleaved review:** Don't open a new lecture with only new material. Start with a retrieval question from the *previous* chapter. Interleaving old and new content during instruction improves long-term retention substantially.

---

### Common Instructional Design Mistakes When Converting Textbooks to Slides

1. **Treating the chapter outline as the slide structure.** Chapters are organized for reading; lectures are organized for learning. These structures differ.
2. **Importing textbook text directly.** Textbook prose is written to be read slowly, re-read, and annotated. Slide text is processed in 3–5 seconds while someone is also listening to you talk.
3. **Covering rather than teaching.** "I need to get through chapter 4" is not an instructional objective.
4. **Including content with no mapped objective.** Every element should earn its place by serving a stated learning outcome.
5. **Neglecting prior knowledge.** A textbook assumes the reader can re-read; a lecture cannot. Content that assumes unavailable schemas creates unmanageable intrinsic load.
6. **No consolidation phase.** A lecture that ends when the content ends misses the most powerful retention-boosting opportunity: making students use what they just learned before leaving.

---

## Domain 2: Visual & UX Design

### The Core Principle: Signal vs. Noise

Edward Tufte's foundational contribution is the concept of **data-ink ratio** — the proportion of a graphic's ink devoted to non-redundant data. Extended to slides: maximize the ratio of information to visual elements. Every element that doesn't carry information is noise that competes with signal. Tufte's argument (2003) that PowerPoint's defaults actively degrade analytical thinking remains the most important critique of the medium. The bullet point forces ideas into a hierarchy that obscures relationships; the template encourages decoration at the cost of information.

Garr Reynolds (*Presentation Zen*, 2008) approaches the same problem from a design perspective: simplicity is not emptiness, it is the removal of everything that obscures meaning. His axiom — "slides are slides, documents are documents; they are not the same thing" — directly parallels the instructional design distinction above.

---

### Typography Rules for Projected Slides

**Font choice:**
- Sans-serif typefaces are generally preferred for projection (Helvetica, Gill Sans, Calibri, Futura). At large sizes, quality serif fonts like Garamond are legible, but serifs are more fatiguing at body text sizes on screens.
- Maximum 2 typefaces per deck. Size and weight variation creates hierarchy without requiring a third font. More than 2 is visual noise.
- Never combine two similar-but-not-identical fonts (e.g., Gill Sans and Optima together — they clash subtly).

**Size hierarchy:**
- Title/headline: 36–48pt
- Body text: 24–28pt minimum (design for the last row)
- Anything below 18pt is generally not readable from the back of a standard classroom

**Line spacing and kerning:**
- At large display sizes, manually adjust letter-spacing (kerning) — software defaults are calibrated for body text, not 40pt headlines
- Generous line spacing (1.3–1.5x) improves readability on projected backgrounds

**The fundamental rule:** If you're reducing font size to fit more text, you're solving the wrong problem. The text is the problem.

---

### Layout, Grid, and Whitespace

- **One idea per slide.** Not one topic — one *idea*. If a slide contains two ideas, it should be two slides.
- Whitespace is not wasted space. It focuses attention. Cluttered slides require viewers to figure out what to look at first, which is extraneous cognitive load.
- Use an implicit grid (halves, thirds, or quarters) to align elements. Unaligned objects create visual tension that the brain reads as disorder.
- **Gestalt principle of proximity:** elements placed close together are perceived as related. Use spatial grouping deliberately.
- **Signaling** (from Mayer): arrows, circles, color highlights, and bold text should be used systematically — always meaning the same thing (e.g., red = warning, bold = key term). Random use of emphasis destroys the signal.

---

### Text vs. Diagram vs. Table vs. Chart — Choosing the Right Visual Form

| Content type | Best visual form |
|---|---|
| Relationships between concepts | Diagram, node map |
| Processes and sequences | Flowchart, timeline |
| Comparisons of attributes | Table |
| Trends over time | Line chart |
| Part-to-whole relationships | Pie or stacked bar (use sparingly) |
| Magnitudes at a point in time | Bar chart |
| Distributions | Histogram or box plot |
| Cause-effect mechanisms | Annotated diagram |
| Definitional content | Key term + short phrase (not a paragraph) |

**Rule from Tufte:** Avoid 3D charts in almost all cases. The depth axis adds visual complexity without adding information and actively distorts perception of magnitudes. The third dimension is decoration, not data.

---

### Redesigning Textbook Figures for Slides

Textbook figures are designed for print: high resolution, small size, meant to be studied closely. Slides are projected large and viewed briefly. They are different media.

When adapting textbook figures:
1. **Remove all labels that don't serve your current learning objective.** A figure of the human nervous system in a neuroscience textbook labels everything; in a lecture on the autonomic nervous system, you want to highlight two things. Everything else is noise.
2. **Add visual signaling.** Use color, arrows, or callout boxes to direct attention. The audience cannot study the figure; they can only follow where you point.
3. **Simplify before you scale.** Don't scale up a complex figure; strip it down first.
4. **Credit the source.** Attribution on the slide or at the end of the deck (more below, under copyright).

---

### Color for Instructional Contexts

**Contrast first:**
- WCAG 2.1 AA standard requires 4.5:1 contrast ratio for text against background (7:1 for AAA)
- In projection environments, ambient light degrades perceived contrast; target 7:1+ for classroom use
- Light text on dark background vs. dark on light: both work; consistency matters more than choice

**Colorblind-safe palettes:**
- 8% of men and 0.5% of women have red-green color blindness (deuteranopia/protanopia)
- Never use red/green alone to convey distinctions
- Safe pairing: blue/orange is the most reliably distinguishable combination across color vision types
- Tools: Colorbrewer (colorbrewer2.org) for data visualizations; Viz Palette or Coolors for interface colors

**Semantic color use:**
- Reserve color for signaling, not decoration. If everything is colored, nothing stands out.
- Limit to 3–4 functional colors per deck (background, text, accent, highlight). Beyond this, color becomes noise.

---

### Slide Density — What the Evidence Says

Research from a study of 105 CME lectures (Wittich et al., 2016) found that **image fraction** (percentage of slides with at least one educationally relevant image) significantly predicted higher speaker evaluation scores. Mean text density was ~26 words per slide, but text density alone was not a significant predictor of evaluations — suggesting that how information is conveyed (visual vs. text) matters more than raw word count.

Evidence-based benchmarks:
- **Maximum 4 bullets per slide** (from multimedia learning research, UCSD; Kosslyn, 2007)
- **Each bullet: 4 or fewer "units" of information** (verbs + key nouns)
- **Assertion-evidence format** outperforms traditional bullet-point format: Garner & Alley (2013) found that slides with a full-sentence headline stating the main point + visual evidence produced higher retention on both immediate and delayed tests than traditional topic-header + bullets
- **1 slide per 1–2 minutes** of lecture time (rule of thumb; density-dependent)

---

### Slides for Live Presentation vs. Async/Self-Paced Viewing

This is the most underappreciated distinction in slide design. They are different products.

| Dimension | Live lecture slides | Async/standalone slides |
|---|---|---|
| Text density | Minimal — the presenter is the text | Higher — the slide must carry the explanation |
| Notes section | Contains full script | May be empty or brief |
| Pacing | Presenter controls | Student controls |
| Retrieval prompts | Inserted as discussion moments | Must be self-contained |
| Navigation | Linear | May need bookmarks or sections |

If you design slides for live delivery and then post them as study materials, students will find them nearly useless — they contain the visual anchors but not the verbal content. Solutions: record the lecture, provide a companion document, or build a separate set of study slides.

---

### Where Tools Work Against You

PowerPoint, Keynote, and Canva share common failure modes:
- **Default templates** encourage decoration and branded consistency over information clarity
- **Bullet-point default formatting** imposes hierarchical structure regardless of whether hierarchy is the right relationship
- **Slide size constraints** force spatial compression of complex diagrams
- **Animation defaults** often add transitions with no pedagogical purpose (Mayer's research suggests gratuitous animation imposes extraneous load)
- **Auto-format features** reduce control over whitespace and alignment

Reynolds' specific advice: Start from a blank slide, not a template. Add elements deliberately. Templates solve a visual identity problem; they don't solve a learning problem.

---

## Copyright Rules for Textbook Content in Slides

This is not optional and is frequently mishandled.

### The Four-Factor Fair Use Test (U.S. Copyright Law, §107)
Every use of copyrighted material must be evaluated against:
1. **Purpose** — educational, nonprofit use favors fair use
2. **Nature** — factual/scientific content more favorable than highly creative works
3. **Amount** — the smaller the portion, the more favorable
4. **Market effect** — does the copying substitute for purchasing the work?

### Key Rules for Lecture Slides

**Text:**
- Short quotations incorporated into lecture slides are **generally fair use** (Penn Libraries guidance)
- Distributing more than a short quotation as part of a coursepack typically **requires permission**
- Practical benchmark (CONFU educational multimedia guidelines): up to 10%, no more than 1,000 words from a single work

**Figures and diagrams from textbooks:**
- Reproducing a figure in a classroom slide that you directly critique or teach from is a strong fair use case — especially if the course requires students to purchase the textbook
- One chart, graph, diagram, or picture per book per course (CONFU guideline)
- The 2008 publisher agreement (including many major academic publishers) allows **two figures/tables from a journal article** for scholarly/educational use without permission
- If the textbook was *prepared for the higher education market*, this weighs **against** fair use, since copying reduces its commercial value

**The TEACH Act (2002):**
- Applies to distance/online instruction at accredited nonprofit institutions
- Permits more flexible use of copyrighted material *if* access is restricted to enrolled students, materials are not downloadable, and the institution has a copyright policy in place

**Practical rules:**
1. Always attribute the source on or near the figure (slide-level or final credits slide)
2. For recorded lectures posted publicly, fair use arguments are significantly weaker than for closed classroom use
3. Reproduce figures at sufficient quality for the educational purpose, but not at print-publication quality
4. If in doubt: link to the original rather than reproducing it

---

## The Synthesis: What Changes When You Start with a Textbook Chapter

The specific challenge of *chapter-to-slides* conversion (vs. building a deck from scratch) is that you start with too much, not too little. The textbook chapter is comprehensive by design; your task is aggressive subtraction guided by clear learning objectives.

**Recommended workflow:**
1. Write 3–5 learning objectives *before* opening the chapter
2. Read the chapter to find content that serves those objectives
3. Identify the 3–6 structural concepts (the load-bearing ideas)
4. For each concept: what is the single best visual representation? (diagram, chart, worked example)
5. Build slides around visuals, not around text
6. Add retrieval/consolidation moments every 10–15 minutes
7. Strip everything that doesn't serve an objective
8. Ask yourself: is this a seductive detail? If interesting but not essential — cut it
9. Decide: is this deck for live delivery or study? Design accordingly

---

## Key Sources

**Cognitive / Instructional Design:**
- Sweller, J. (1988). Cognitive load during problem solving. *Cognitive Science, 12*, 257–285
- Mayer, R.E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press
- Harp, S.F. & Mayer, R.E. (1998). How seductive details do their damage. *Journal of Educational Psychology, 90*(3)
- Dunlosky, J. et al. (2013). Improving students' learning with effective learning techniques. *Psychological Science in the Public Interest*
- Roediger, H.L. & Butler, A.C. (2011). The critical role of retrieval practice. *Trends in Cognitive Sciences*
- Garner, J.K. & Alley, M. (2013). How the design of presentation slides affects audience comprehension. *Technical Communication*

**Visual / UX Design:**
- Tufte, E.R. (2003). *The Cognitive Style of PowerPoint*. Graphics Press
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders
- Duarte, N. (2008). *slide:ology*. O'Reilly Media
- Kosslyn, S.M. (2007). *Clear and to the Point*. Oxford University Press
- Wittich, C.M. et al. (2016). Speakers with high evaluation scores use more image-based slides. *Western Journal of Emergency Medicine*

**Copyright:**
- U.S. Copyright Act §107 (Fair Use)
- TEACH Act, 2002
- CONFU Educational Multimedia Guidelines (1996)
- Penn Libraries: Copyright Resources for Online Courses
- Harvard OGC: Copyright and Fair Use
