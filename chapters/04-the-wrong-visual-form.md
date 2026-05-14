# Chapter 4 — The Wrong Visual Form

*When the information is right but the format makes it hard to see, the failure has a name. Find the name. Change the form.*

---

Here is a slide you have seen, possibly made.

The title says "Three Policies for Reducing Carbon Emissions: Pros and Cons." Below it, three columns of bullets. Carbon Tax on the left. Cap-and-Trade in the middle. Subsidies on the right. Under each column, an "Advantages" header and a "Disadvantages" header, four bullets each. The bullets line up vaguely. You read the first advantage of the carbon tax, then drift to the first advantage of cap-and-trade, then back, then forward, then you lose your place. You finish the slide having read everything and understood the structure of nothing.

The content is fine. The slide is the problem. And the problem is specific: the structure of the content is a comparison across shared attributes — which policy does what on price, emissions caps, revenue, equity, political feasibility — and that structure is invisible. It is buried inside the bullets. The reader has to excavate it.

Now here is the same content in a table. Five rows: price, emissions cap, revenue, equity, political lift. Three columns: one per policy. Each cell is a short phrase. You can read across a row — "which policy does what on equity?" — and get the answer in three eye movements. You can read down a column — "what does the carbon tax do overall?" — and get the answer in five. The comparison the title promises is now the structure of the slide.

I want to think through why this matters, and what the underlying rule is, because "use a table for comparisons" is not the full picture. The full picture is about something more fundamental: the relationship between the shape of an idea and the form used to show it.

---

## The grammar of a slide

Every piece of content has a structure. Not a vague structure — a precise one, the kind you can name.

Some content is a *comparison*: here are three things, here are the attributes that distinguish them, here is how each one differs on each attribute. The structure is a matrix. Rows are attributes, columns are things, cells are values.

Some content is a *sequence*: here is how one thing follows from another. The structure is a chain. The chain may be simple (step one, step two, step three) or branching (if this, then that; otherwise, this other thing). The visual form for a simple sequence is a timeline or an arrow chain. The visual form for a branching sequence is a flowchart.

Some content is a *relationship*: here are entities and here is how they connect. The structure is a network. The visual form is nodes and edges — not boxes sitting on a slide for decoration, but boxes connected by arrows whose direction and label encode the actual relationship.

Some content is a *trend*: here is how a quantity changed over time. The structure is a time series. The visual form is a line chart.

Some content is a *magnitude comparison*: here are quantities at a single moment, and we want to know which is bigger. The visual form is a bar chart, sorted by value, with bars running horizontal so the labels can be read without craning.

And some content is genuinely a *list*: here are things that do not compare, do not sequence, do not relate, and do not vary over time. They are just items. The visual form for a list is a list.

<!-- → [TABLE: the six structural types as a reference table — columns: "Structure type", "What the content is", "Correct visual form", "What bullets hide"; rows for comparison, sequence (linear), sequence (branching), relationship/network, trend over time, magnitude comparison, genuine list; student should be able to scan the table and immediately identify which row their slide falls into] -->

The problem with bullet points is not that they are ugly. The problem is that they are the default form for every piece of content regardless of its structure. A comparison becomes a list. A sequence becomes a list. A network becomes a list. A trend becomes a list. The list is the zero-decision form — the form you get when you haven't asked what the content is actually shaped like.

And when you put content into the wrong form, you impose work on the reader. Not the work of understanding the content — that's the work the reader is supposed to do. The work of reconstructing the structure that the content already has, that the wrong form erased. Every time a reader has to hold a bullet from column one in working memory while scanning column two for its counterpart, they are doing the designer's job. Working memory used for that reconstruction is working memory not available for the idea itself.

This is what cognitive scientists call extraneous load — load imposed by the presentation, not by the difficulty of the concept. John Sweller's research in the late 1980s established that extraneous load trades directly against learning: every unit of working memory spent navigating a badly formed slide is a unit not spent connecting the new idea to what the student already knows. The form is not neutral. A mismatch between the structure of the content and the structure of the form is a pedagogical cost, measurable and real.

---

## What perception tells us about form

There is another layer under the cognitive load argument, and it comes from perceptual psychology.

In 1984, William Cleveland and Robert McGill published an experiment in the *Journal of the American Statistical Association* that asked a simple question: when people try to decode a quantitative relationship from a chart, which visual marks are decoded most accurately? Their answer was a ranking. At the top: position along a common scale — the thing a bar chart uses, the thing a table uses when you compare entries in the same row. Near the bottom: angle and area — the things a pie chart uses. At the very bottom: color saturation and volume.

<!-- → [CHART: horizontal bar chart of the Cleveland-McGill accuracy ranking — bars sorted from most to least accurate; items include: position along common scale, position along non-aligned scale, length, angle/slope, area, color saturation/volume; two items (angle/area and color saturation) highlighted in a warning color to flag low accuracy; caption: "This is not an aesthetic ranking. It is a perceptual transmission rate. The form you choose determines how accurately your reader decodes the relationship."] -->

This ranking has held for forty years. It has been replicated, extended, and refined. The practical consequence is that the choice of visual form is not aesthetic. It is a perceptual transmission rate. A pie chart is not just harder to look at than a bar chart — it communicates quantitative relationships with measurably lower accuracy. The reader's judgment of "which slice is bigger" is systematically worse than their judgment of "which bar is taller," especially when slices are similar in size.

The Cleveland-McGill ranking applies to categorical comparisons too, not just quantitative ones. A table uses position along rows and columns — the most accurate perceptual encoding. A bulleted list uses serial reading order and memory — neither of which is in Cleveland and McGill's top tier. When you render a comparison as bullets, you are forcing the reader to use one of the least accurate comparison mechanisms available. They have to hold a bullet in short-term memory, shift attention to another column, search for the comparable bullet, hold both, and then compare. Every step in that chain is a place where precision is lost and cognitive capacity is consumed.

Put the two arguments together — Sweller's on extraneous load and Cleveland and McGill's on perceptual accuracy — and you get a single strong claim: the form matters because the brain is not a neutral receiver. It processes different forms with different efficiency and different accuracy. Giving a reader content in the wrong form is not just an aesthetic failure. It is a functional one.

---

## Why bullets are the default anyway

If bullets are so often the wrong form, why does every slide tool default to them?

The answer is that bullets are the lowest-common-denominator structure. Any content can be forced into a bulleted list. You do not need to ask what the content is shaped like. You do not need to decide whether it is a comparison or a sequence or a network. You just type, and the tool makes bullets.

This is appealing in the moment and catastrophic in aggregate. A tool that makes all decisions for you produces slides that reflect the tool's defaults, not the structure of your ideas. Canva defaults to bullets. Gamma defaults to bullets. PowerPoint defaults to bullets. Beautiful.ai defaults to bullets with some decorative geometry around them. None of them default to tables, or timelines, or network diagrams, because those require the author to have made a structural decision that the tool cannot make for them.

AI slide generators have the same problem, compounded. An AI asked to make a slide comparing three policies will almost always produce bullets, because bullets are what slide decks in its training data predominantly contain. The AI has learned the default, not the principle. Asking it to produce a table requires you to know the table is the right form and instruct it explicitly. The diagnosis has to come from you. The tool will execute, but it will not decide.

There is a related failure that AI diagram generators produce that is worth naming separately. If you ask an AI tool to make "a diagram showing how X works," you will often get something that looks like a diagram — boxes, arrows, connecting lines — but whose structure encodes nothing. The arrows go from box to box for visual plausibility, not because there is an actual directed relationship between those elements. The labels are typeset inside shapes but do not answer the question "why does this connect to that?" The result satisfies the visual expectation of a diagram while failing the structural requirement. The Multimedia Principle — which Richard Mayer's research established as the strongest single effect in educational media, with an effect size around d = 1.39 in his standard comparisons — requires that the picture carry structural information the words alone do not carry. A decorative arrangement of boxes and arrows is not multimedia. It is words arranged in shapes.

<!-- → [IMAGE: side-by-side diagram mockup illustrating the AI diagram failure — left: boxes and arrows in a plausible-looking layout but with generic labels and arrows that go nowhere meaningful; right: the same topic rendered as a genuine node-and-edge diagram with directed, labeled edges that encode the actual relationships; caption: "Both look like diagrams. Only the right one is one. The test: can you trace why this box connects to that one?"] -->

The diagnostic question that cuts through all of this is the same whether you are looking at a bullet slide or an AI-generated diagram: *what is the structural relationship between the elements?* Not what the slide looks like. What the content actually is. Answer that question honestly, and the right form usually becomes obvious.

---

## Finding the right form

The matching is not complicated once you have named the structure. Here is the full set of cases.

If the content is a **comparison** — things by attributes — it is a table. Attributes are rows. Things are columns. Cells are answers. The table makes the comparison axes explicit rather than implicit. A reader can move across a row to compare one attribute across all things, or down a column to characterize one thing across all attributes. Both directions are available without working-memory cost.

If the content is a **sequence without branches** — events or steps in time order — it is a timeline. The horizontal axis is time, scaled to the actual intervals. 1929 and 1933 are not the same distance apart as 1939 and 1941. A timeline shows the compression and expansion of time. A bullet list cannot, because the bullets are evenly spaced regardless of what they represent.

If the content is a **sequence with branches** — a process that depends on conditions — it is a flowchart. The branch is the thing that bullets cannot show. "If A, do this; if not A, do that" is a fork. A flowchart shows the fork. A list pretends it is not there.

If the content is a **network** — entities with connections among them — it is a node-and-edge diagram. The edges carry the relationship. The direction of an edge says something. The label on an edge says something. A list of nodes with no edges shows nothing about why those nodes matter in relation to each other.

If the content is a **trend over time** — a quantity changing — it is a line chart. The line encodes rate of change. A steep segment says something a shallow segment does not. A list of numbers with their years cannot show you the shape of the trend; it can only give you the individual values.

If the content is a **magnitude comparison at a single moment** — how big is this relative to that — it is a horizontal bar chart sorted by value. Horizontal because the labels are usually words, and horizontal bars let you read the labels without rotating your head. Sorted because the rank relationship is often what matters, and sorting makes it visible instantly. Not a pie chart. Pie charts encode magnitude as angle and area, which are low in the Cleveland-McGill ranking. Bar charts encode magnitude as position, which is at the top. Use bars.

If the content is a **list** — genuinely independent items with no comparison, no sequence, no relationship, no trend — then, and only then, use bullets.

The question to ask before choosing a form is: *what is the structural relationship between the elements on this slide?* State it in one phrase. "Comparison across attributes." "Sequence with two branches." "Dependencies among five components." "Trend from 2010 to 2024." "Five unrelated examples." The form follows from the answer. If you cannot state the structural relationship, the slide does not yet know what it is showing, and no choice of form will fix that.

<!-- → [IMAGE: the carbon emissions example rendered in both forms, side by side at full text width — left: the three-column bulleted version with Advantages/Disadvantages headers; right: the five-row table (Price, Emissions cap, Revenue, Equity, Political lift) with one column per policy; annotations on the left version marking the hidden comparison axes with dotted lines; annotations on the right version marking the explicit row labels; caption: "Same content. The left version has the comparison axes implicit in the bullets. The right version has them explicit in the rows. The reader's working memory pays the difference."] -->

---

## The form decision upstream of everything else

One thing I want to be precise about, because it is easy to get backwards.

The form decision is not a design decision in the sense of "how should this look." It is a semantic decision — a decision about what the content is. The table is not better than bullets because it is cleaner or more sophisticated. It is better because it encodes the actual structure of the comparison, and bullets do not. If you switched to the table for aesthetic reasons but your content was genuinely a list, the table would be the wrong choice. The form follows the structure. That is the whole rule.

This means the form decision has to happen before the slide is built, not after. You cannot look at a finished bullet slide and say "let me find a better form for this." You can, but you are working backwards. The right sequence is: *what is the structural relationship between these elements?* Then: *which form encodes that relationship best?* Then: build the slide.

It also means that the form decision cannot be delegated to a tool. The tool does not know whether your three items are comparable across shared attributes or genuinely independent. You know. The tool can execute whatever form you specify, but the specification has to come from your understanding of the content. The diagnosis is yours.

---

## A note on Tufte's rule and its one complication

Edward Tufte's data-ink ratio — the fraction of a chart's marks that carry information versus the fraction that are decoration — is the cleanest way I know to see whether a form is doing work. A bulleted comparison uses many marks (every letter, every bullet glyph, every line break) and encodes no structure. A table uses fewer marks and makes the comparison axes explicit. The ratio of structural information to total ink is higher in the table. More information, fewer marks.

Tufte's rule is usually stated as "maximize data-ink ratio" or "eliminate chartjunk." The direction is right. But there is one finding that complicates the strong version.

Bateman and colleagues, in a 2010 paper at the CHI conference, ran an experiment on charts with and without decorative elements — the "chartjunk" Tufte argued should be cut. They found that some decorative elements improved long-term recall of the chart's content without hurting immediate comprehension. The chartjunk-decorated charts were remembered better two weeks later.

This seems like a refutation of Tufte. I think it is a refinement. The Bateman result holds for memorability — the reader can later recall that "the chart about fuel costs had the gas pump" — but the experiment measured recall of the chart's topic, not transfer of the concept to a new problem. For journalism and marketing, where you want readers to remember your chart, some chartjunk may be acceptable. For instructional slides, where the goal is that the student can use the concept to solve a problem they have not seen before, Tufte's rule holds. Decoration competes with structure in the student's working memory. The concept the student needs to internalize is the structure, not the decoration. Recall is the wrong metric; transfer is what teaching is for.

So: eliminate chartjunk in instructional slides. Accept it, cautiously, in slides whose purpose is to be memorable rather than to teach.

<!-- → [TABLE: two-column decision table for chartjunk — columns: "Context" and "Chartjunk verdict"; rows: instructional slide (goal: transfer), journalistic chart (goal: memorability), marketing slide (goal: recall), technical reference (goal: precision); each cell states the verdict and one-line rationale; caption: "Tufte's rule is not wrong. It applies to the wrong goal in the wrong context."] -->

---

## Two honest disagreements

Before leaving this chapter, I want to name the two places where careful people will disagree.

The first is about pie charts. The strong position — which is Cleveland and McGill's, and Tufte's, and mine — is that pie charts should almost never be used because angle and area are low-accuracy encodings. Use a horizontal bar chart instead. The weaker position is that for two-to-four-slice comparisons where the reader only needs approximate magnitudes — "most of the budget went to A, a little to B and C" — a pie chart is faster to read because the part-to-whole relationship is encoded in the shape itself, and the reader does not need to add up the bars to get the gestalt. The vocabulary for the disagreement: *precision* and *part-to-whole*. If the slide is making a claim about exact magnitudes, use a bar chart. If the slide is making a claim about rough proportions and part-to-whole relationship, a pie chart with two or three slices may serve. Never more than four slices. Never 3D. And if you are unsure, use the bar chart. The accuracy cost of the bar chart approaches zero; the accuracy cost of the pie chart climbs with the number of slices.

The second disagreement is about when a table is the wrong form for a comparison. A table is ideal when the comparison axes are stable — the same attributes apply to all the things being compared, and the cells can be filled with consistent entries. It breaks down when the attributes are not parallel — when Policy A has three advantages and Policy C has two, and the two are not the same advantages. In that case, a table with empty cells can look like a claim about absence rather than a signal of asymmetry. The original bulleted format, for all its structural failures, does at least make asymmetry easy to represent. The fix is not to go back to bullets, but to add a footnote convention or to split the slide: one table for the attributes that are parallel, one section for the asymmetries that are not. Forcing unparallel content into a symmetric table is its own form of mismatch.

Both disagreements reduce to the same underlying question: *what is the structural relationship between the elements, and does this form encode it honestly?* That question is the whole diagnostic. When the answer is yes — the form is encoding the actual structure — the form is right, whatever it looks like. When the answer is no — the form is hiding structure, inventing structure, or encoding the wrong thing — the form is wrong, however attractive it appears.

---

Once the form is right, the next question is whether the color inside that form is doing any work. Color can reinforce the structure or undermine it — and the way it undermines is specific and fixable. That is Chapter 5.

---

**What would change my mind:** A well-controlled study showing that for genuinely comparative content — same things, same attributes, same claim — a bulleted layout produces equivalent learning outcomes to a table, when the student is tested on their ability to use the comparison to solve a new problem. I have not seen that study. The cognitive load literature points strongly in the other direction, but the specific comparison between bulleted comparisons and tables in instructional slides has not, to my knowledge, been run cleanly. If it has and I have missed it, I want to know.

**Still puzzling:** I do not have a clean rule for when a comparison is "close enough to parallel" that a table is honest. Some content is almost a matrix — the attributes mostly apply, with occasional asymmetries — and the choice between a table-with-footnotes and a bulleted-with-structure is genuinely ambiguous. The principle is clear; the threshold is not.

---

## LLM Exercises

**Exercise 1 — Structure diagnosis**
Take any slide you have built in the last month that uses bullets. Paste the slide content to an LLM with this prompt: *"Identify the structural relationship between the elements on this slide. State it in one phrase: comparison, sequence, network, trend, magnitude comparison, or genuine list. Then tell me which visual form matches that structure and why bullets do or do not fit."* Compare the LLM's diagnosis to your original intent. If they diverge, identify which element of the structure the bullets were hiding.

**Exercise 2 — Table conversion**
Find a slide that uses bullets to compare two or more things. Ask an LLM: *"Convert this bulleted comparison to a table. The rows should be the shared attributes; the columns should be the things being compared. If any attribute does not apply to all columns, note it in the cell rather than leaving it blank. Return the result as a plain-text markdown table."* Then evaluate: are the comparison axes in the resulting table the same axes you would have named if asked to state the slide's claim? If not, the bullets were hiding the wrong structure.

**Exercise 3 — Timeline conversion**
Find a slide that presents historical events or process steps as bullets. Ask an LLM: *"Convert this bulleted list to a timeline description. For each event, state: the label, the date or step number, and the interval since the previous event. Identify any intervals that are significantly larger or smaller than the others — those are the gaps that a bullet list flattens but a timeline would show."* Use the output to decide whether a visual timeline would reveal something the bullets cannot.

**Exercise 4 — Diagram legitimacy check**
Take an AI-generated diagram from any tool — Gamma, Canva, or any other. Paste a description of it (or the diagram itself, if the LLM accepts images) with this prompt: *"For each arrow or connecting line in this diagram, state what directed relationship it encodes. If you cannot state a specific relationship — only that it looks connected — flag that arrow as structurally empty. Count the total arrows and the flagged arrows. A diagram where more than one-third of the arrows are flagged is decorative, not structural."* Use the count to decide whether to rebuild or discard the diagram.

**Exercise 5 — Pie vs. bar decision**
Describe a chart you are planning to a LLM: *"I want to show [content] to [audience]. The claim I am making is [claim]. Should I use a pie chart or a horizontal bar chart? Apply the Cleveland-McGill accuracy ranking and the precision/part-to-whole distinction to justify the recommendation."* Then apply the recommendation and ask a colleague to state the claim they read from the chart without you explaining it. Their answer is the accuracy test.

**Tags:** form-fit, Mayer-multimedia, Cleveland-McGill, Tufte-data-ink, cognitive-load, table-vs-bullets, visual-grammar
