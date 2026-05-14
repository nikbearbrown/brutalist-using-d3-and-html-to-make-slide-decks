# Chapter 4 — The Wrong Visual Form

> When the information is right but the format makes it hard to see, the failure has a name. Find the name. Change the form.

---

## 1. The feeling

Here is a slide you have seen, possibly made.

The title says "Three Approaches to Error Correction." Below it, three columns of bullets. The left column has five bullets about the first approach. The middle column has five bullets about the second. The right column has five bullets about the third. The bullets line up vaguely. You read the first bullet on the left, then drift to the first on the middle, then back, then forward, then you lose your place.

Or this one: a course slide titled "Key Events 1914–1945" with twelve bullets, each one starting with a year. You read the dates. You can almost feel the war approaching across the bullets but not quite — the rhythm is wrong, the gaps between events are flattened to nothing because the bullets are evenly spaced. 1929 and 1933 sit the same distance apart as 1939 and 1941. They are not the same distance apart in any way that matters.

Or this one: a slide from an AI tool, generated from the prompt "explain supervised vs unsupervised learning." Two stacked rows. Top row: supervised, with five bullets. Bottom row: unsupervised, with five bullets. Symmetric. Tidy. The reader cannot tell whether the bullets are paired across categories or independent, whether the comparison is by attribute or by example, whether anything in particular is being compared at all.

In each case, the content is fine. The slide is not.

That is the feeling this chapter is about.

---

## 2. The two diagnostic questions

**Cognitive science question:** *Is the structure of the content visible from the structure of the slide?*

When a process is shown as a list, its sequence is invisible. When a comparison is shown as side-by-side bullets, the comparison axes are invisible. When a network is shown as paragraphs, the connections are invisible. The student has to mentally reconstruct the structure the content already has. Working memory is spent on that reconstruction instead of on the content itself. That is the extraneous load Mayer keeps writing about — load you imposed by choosing the wrong form.

**Visual design question:** *What is this slide comparing, sequencing, or showing — and does the form match?*

This is the form-fit question, and it lives upstream of every other design choice. Cleveland and McGill ran experiments in the 1980s on how accurately people decode different visual marks. Position along a common scale won. Color saturation lost. Their [1984 paper in the *Journal of the American Statistical Association*](https://www.tandfonline.com/doi/abs/10.1080/01621459.1984.10478080) is forty years old and has not been overturned. The visual form is not aesthetic preference. It is a perceptual transmission rate.

Always both questions. Always in that order. Cog sci tells you why it matters that the form match. Visual design tells you which form matches what.

---

## 3. The principle named

Plain language first: **the visual grammar should match the conceptual grammar.**

If the content is a sequence, the form is a sequence — a timeline, a flowchart, an arrow chain. If the content is a comparison across attributes, the form is a table. If the content is a set of relationships, the form is a node-and-edge diagram. If the content is a trend over time, the form is a line chart. If the content is a list of genuinely independent items with no structure among them — then, and only then, the form is a list.

Bullets are the default because every slide tool defaults to them. They are not the right form. They are the no-decision-made form. Choosing bullets when bullets do not match the structure is not a design choice. It is the absence of one.

Framework vocabulary: this is Mayer's [Multimedia Principle](https://pmc.ncbi.nlm.nih.gov/articles/PMC10845804/) read tightly. *Multimedia* does not mean "add a picture." It means "the picture carries structural information the words alone do not carry." A flowchart of a process is multimedia. A bulleted list of the same process steps is words alone in a sans-serif font. Mayer's effect size for the multimedia principle, across his standard comparisons, is roughly d = 1.39 — enormous in education research. But the size depends on the picture being the right picture. A stock photo of a brain next to a list of memory types is not multimedia. It is decoration. The picture has to encode the structure.

It is also Tufte's [data-ink ratio](https://www.edwardtufte.com/book/the-visual-display-of-quantitative-information/) read carefully. A bulleted list of relationships uses a lot of marks — every letter, every bullet glyph, every line break — and shows no structure. A three-node diagram with two arrows uses fewer marks and shows the cycle. The ratio of structural information to total ink is higher. Tufte's rule is not "use fewer marks." It is "use marks that carry information." Adding an arrow that shows direction is more ink, but it earns its place.

And it is Munzner's [*Visualization Analysis and Design*](https://www.cs.ubc.ca/~tmm/vadbook/) reduced to a single sentence the reader can run in their head: before encoding anything, ask what the data is and what the task is. The visual form follows from data type and task. Aesthetic preference is the wrong layer.

---

## 4. Bad example

Slide title: **"Three Policies for Reducing Carbon Emissions: Pros and Cons"**

Here is what the AI tool produced. Three columns. Carbon Tax on the left. Cap-and-Trade in the middle. Subsidies on the right. Under each column, an "Advantages" header, four bullets. Then a "Disadvantages" header, four bullets. Sans-serif body text. Faint dividers between columns. A footer reading "Source: textbook ch. 14."

```
+------------------------------------------------------------+
| Three Policies for Reducing Carbon Emissions: Pros and Cons|
+----------------+-----------------+-------------------------+
| Carbon Tax     | Cap-and-Trade   | Subsidies               |
|                |                 |                         |
| Advantages     | Advantages      | Advantages              |
| • Predictable  | • Caps total    | • Politically easier    |
|   price        |   emissions     | • Targeted              |
| • Revenue      | • Market-set    | • Encourages innovation |
|   generated    |   price         | • Supports new tech     |
| • Simple to    | • Flexible for  |                         |
|   administer   |   firms         |                         |
| • Internalizes | • Tradeable     |                         |
|   externality  |   permits       |                         |
|                |                 |                         |
| Disadvantages  | Disadvantages   | Disadvantages           |
| • Regressive   | • Complex to    | • Costly to public      |
|   without      |   set up        | • Hard to target        |
|   rebate       | • Volatile      | • Distorts markets      |
| • Politically  |   prices        | • Picks winners         |
|   unpopular    | • Allocation    |                         |
| • Doesn't cap  |   politics      |                         |
|   total        | • Monitoring    |                         |
|   emissions    |   costs         |                         |
+----------------+-----------------+-------------------------+
```
<!-- annotation: title labels the topic but states no claim. Chapter 10 territory. -->
<!-- annotation: three columns suggest comparison, but the comparison axes are hidden inside the bullets. -->
<!-- annotation: bullets are uneven in length (3, 4, 4) — the eye reads asymmetry as data when it is just truncation. -->
<!-- annotation: "Advantages" and "Disadvantages" are repeated three times — the same word doing zero work twice. -->
<!-- annotation: to compare "predictability" across all three policies, the reader has to search column 1 bullet 1, then scan column 2 for a matching idea, then column 3. Cross-reference cost: roughly nine eye movements per axis. -->
<!-- annotation: structural relationship between elements: a set of attributes (predictability, revenue, equity, market dynamics, political feasibility) measured across three categories (the policies). That structure is a table. -->
<!-- annotation: form-fit failure: the content is a table rendered as three lists. -->

The slide is not unattractive. It is failing in a specific way. The structure of the content — a comparison of three policies across roughly five shared attributes — is a 3-by-5 table. The slide renders it as three lists with hidden axes. The reader has to do the mental work of building the table that was already implicit in the content. That mental work is extraneous load. The slide imposed it.

The AI tool did this because bullets are its default form. Canva, Gamma, and Beautiful.ai all default to bullets because bullets are the lowest-common-denominator structure that any content can be forced into. A bullet asks nothing of the structure of the content; it just stacks the words. That is the appeal, and the failure.

---

## 5. Good example

Same slide title. Same content. Different form.

```
+--------------------------------------------------------------------+
| Three Policies for Reducing Carbon Emissions                       |
| —————————————————————————————————————————————                       |
|                                                                    |
|                  | Carbon Tax    | Cap-and-Trade | Subsidies       |
| ---------------- | ------------- | ------------- | --------------- |
| Price            | Predictable   | Market-set    | n/a (no price)  |
| Emissions cap    | No            | Yes           | No              |
| Revenue          | To government | To government | From government |
| Equity           | Regressive*   | Depends on    | Regressive**    |
|                  |               |  allocation   |                 |
| Political lift   | High          | Medium        | Low             |
|                                                                    |
| * unless rebated   ** subsidies tend to capture upper-income users |
+--------------------------------------------------------------------+
```
<!-- annotation: title still topic-not-claim; that's Chapter 10. Form is the focus here. -->
<!-- annotation: comparison axes are now visible as row labels. The structure that was hidden is now the spine of the slide. -->
<!-- annotation: each cell is one phrase, not a bullet — the eye moves through the table in either direction (across a row to compare one attribute, down a column to characterize one policy) without re-reading. -->
<!-- annotation: cells that would have been "n/a" or asymmetric in a bulleted version are now legible as actual asymmetries in the data — "no emissions cap" for the tax is a real feature of the comparison, not a missing bullet. -->
<!-- annotation: footnotes carry the conditionality that was muddling the bullets ("Regressive without rebate"). The qualifier is now in a footnote, not a bullet halfway down a column. -->
<!-- annotation: total marks on the slide are fewer than the bulleted version (roughly 60 words vs. 110). Data-ink ratio is higher. -->
<!-- annotation: this is the same content. The form changed. The structure is now visible. -->

What changed: the table made the comparison axes — the rows — explicit. The bulleted version had those axes implicit inside the bullets; the reader had to extract them. The table extracts them once, in the row labels, and the cells become short answers to "how does this policy do on this axis?"

Cleveland and McGill's ranking applies even here, in a non-quantitative table: the reader uses *position along a common scale* (the row, the column) to compare values, which is the most accurate perceptual decoding humans do. The table is closer to a chart than a list. The bulleted version forced the reader to do the comparison using *memory and saccade* — read a bullet, hold it, look at another column, search for the comparable bullet, hold both. Working memory burns.

The table is also shorter. Fewer marks. Higher information density per square inch. This is Tufte's rule operating in its mildest form: more data, fewer redundant elements.

---

## 6. The prompt

Paste this into the Brutalist system on any slide where the form feels wrong.

> Look at this slide. Answer one question before you change anything: what is this slide comparing, sequencing, showing, or relating?
>
> - If it is comparing attributes across categories, render it as a table with the attributes as rows and the categories as columns.
> - If it is showing a sequence or a process, render it as a timeline (for chronology) or a flowchart (for steps with branches).
> - If it is showing relationships among items, render it as a node-and-edge diagram with the items as nodes.
> - If it is showing a quantitative trend over time, render it as a line chart.
> - If it is showing magnitudes at one moment, render it as a horizontal bar chart sorted by value. Not a pie chart unless there are two or three slices and exact comparison is not required.
> - If it is genuinely a list of independent items with no structural relationship among them, then — and only then — render it as a list.
>
> Bullets are the default in every other system. They are not the default here. Choose them only when the content is genuinely list-shaped.
>
> Do not use 3D in any chart. The depth axis adds no information and distorts magnitude judgments.

The prompt is portable. The Brutalist system can produce a D3 table or flowchart or timeline directly. In Canva or Gamma, the same prompt works for the form decision; the tool then produces a worse version of the same form. That is fine — the diagnostic was the hard part. The tool is the easier part.

---

## 7. The DESIGN.md change

Add a single rule, not a tokenized variable.

```yaml
# DESIGN.md
slide_form_decision:
  rule: "Before any slide is rendered, identify the structural relationship
         between the elements on the slide (comparison / sequence / network /
         trend / magnitude / list). The visual form follows from the
         relationship. Bullets are reserved for genuinely list-shaped content."
  default_layout_check: true
  forbidden_forms: ["3D charts", "pie charts with more than 4 slices"]
```

One sentence why: this variable converts the form decision from an aesthetic choice the system makes by default into a structural question the prompt has to answer.

---

## 8. The diagnostic questions to keep

Use these on any slide. They take under thirty seconds.

1. **What is the structural relationship between the elements on this slide?** Answer in one phrase: "comparison across attributes," "sequence with intervals," "network of dependencies," "trend over time," "single magnitude with parts." If you cannot answer, the slide does not yet know what it is showing.

2. **Does the current form make that relationship visible at a glance, or does the reader have to reconstruct it?** A reader who has to reconstruct the structure is doing the designer's work for them, using working memory you needed for the content.

3. **If I removed the form (bullets, table, chart) and kept only the words, would the structure still be readable from the words alone?** If yes, the form was decorative. If no, the form was carrying real information — but only if it was the right form.

4. **Would Cleveland and McGill rank this encoding high or low for accuracy?** Position-along-a-scale is high; angle and area (pie slices) are medium; color saturation and volume are low. The encoding choice is a perceptual transmission rate.

5. **What is the AI tool's default form for this content, and have I overridden it?** If you have not, you have accepted whatever bias the tool has. The tool's bias is almost always toward bullets.

---

## 9. What two people might disagree about

Two reasonable designers will disagree about pie charts.

One position: pie charts are almost always inferior to horizontal bar charts. Cleveland and McGill's ranking is unambiguous on this — slices encoded by angle and area are decoded less accurately than bars encoded by position. The literature has been consistent for forty years. The recommendation: never pie, always bar.

The other position: for two-to-four-slice comparisons where the reader only needs approximate magnitudes ("most of the budget went to A, a little to B and C"), a pie chart is faster to read because the part-to-whole relationship is encoded in the shape itself. The reader does not have to do the addition. The recommendation: pies for two-to-four-slice part-to-whole when precision is not the point.

The vocabulary for the disagreement: *precision* and *part-to-whole*. If the slide makes a claim about exact magnitudes ("13% went to A, 19% to B"), a bar chart is correct because exact magnitudes are read more accurately as position. If the slide makes a claim about gestalt proportion ("almost all of it went to A"), a pie chart may be acceptable because the part-to-whole relationship is what the reader is meant to see, and the pie shows it directly.

There is also a real wrinkle in the Tufte rule. Bateman et al.'s [2010 CHI paper "Useful Junk?"](https://hci.usask.ca/uploads/173-pap0297-bateman.pdf) ran an experiment on so-called chartjunk — decorative graphical elements Tufte argued should be cut — and found that some chartjunk improved long-term recall of charts *without* hurting comprehension. The honest reading: for one-off memorable charts in journalism or marketing, decorative elements can aid recall. For instructional slides where the goal is *transfer* — the student using the concept on a problem they have not seen before — Tufte's rule holds. The decoration competes with the structure the student needs to internalize. Recall is the wrong metric for teaching.

One last thing: AI-generated diagrams are a special case of the wrong-form failure mode. An AI tool asked to produce "a diagram showing how X works" will often produce something that looks like a diagram — boxes, arrows, labels — but whose structure encodes nothing. The arrows go from arbitrary places to arbitrary places. The labels are visually plausible but semantically empty. The Multimedia Principle is satisfied in appearance and violated in substance. The chapter's diagnostic still applies: ask what the structural relationship between the elements is. If the AI diagram does not show that relationship — if you cannot trace why this box connects to that one — the form is wrong, and the right move is to throw the AI diagram out and either build the diagram yourself or use words plus a real figure.

---

Once the form is right, the next question is whether the color in that form is doing any work — or whether it is decorating, miscoding, or actively making the slide harder to read. That is Chapter 5.
