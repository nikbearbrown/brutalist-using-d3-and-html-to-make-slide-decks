# Chapter 5 — Color Is Doing Nothing (or Harm)


## TL;DR

- Every color on the slide is either encoding something or competing with what is.
- The chapter moves through What color can and cannot do, The contrast problem, What the failure looks like, What the repair looks like, and related ideas.
- Read it for the main argument, the vocabulary it introduces, and the practical judgment it asks you to develop.

*Every color on the slide is either encoding something or competing with what is. Find out which. Cut the rest.*

---

Let me tell you about a puzzle I find genuinely interesting.

Take a slide with six colors on it. A gradient background, a navy headline, four bullets in red, green, orange, and blue, a colored chart, a yellow badge in the corner. The slide looks polished. It came out of Canva or Gamma or some AI tool's "professional" preset. It looks, in the ordinary sense of the word, designed.

Now ask: what does red mean? What does green mean? Are they paired? Is the red bullet the one that is bad news and the green the one that is good news, or are they just different colors for different bullets? Sit with the question for a moment. If you were a student in the third row, which element on the slide is calling for your attention?

The puzzle is that the slide does not have an answer. There is no code. The colors were chosen to look interesting, not to mean anything. And "looking interesting" while meaning nothing is not a neutral outcome. It is a specific kind of damage.

Here is why that matters: your brain does not know the colors mean nothing. The moment a color appears on a visual display, your brain's pattern-recognition system begins searching for the rule. Red appears on bullet A. Green on bullet B. A rule must exist. Your brain is looking for it. It runs a search — *is red the warning? is green the progress? are they paired by some category?* — and the search fails, and your brain has spent cognitive resources on the failure. Resources that were supposed to go to the content.

This is not a minor inefficiency. Working memory is small. The search for a pattern that does not exist is a real cost. And there is another cost that is harder to see: the colors that are doing real work — if any are — are now drowned out by the colors that are not. The signal is lost in the noise.

This chapter is about the rules that determine which colors are signal and which are noise, and what to do about each.

---

## What color can and cannot do

Start with what the research says about color as an information channel.

William Cleveland and Robert McGill published a paper in 1984 that ranked visual encoding channels by how accurately people could read quantitative information from them. Position along a common scale came first — you can read a bar chart accurately because you are judging where the bar's end lands on a shared axis. Then length, then angle, then area. Near the bottom of the list, below most other channels: color saturation.

This is worth sitting with. Color is one of the *weakest* channels for conveying quantitative information accurately. When a chart uses color as its primary encoding — four bars, four different saturated colors, no other distinguishing feature — it is asking the weakest available channel to do the heaviest work. The same information, encoded in position (bars sorted by value on a labeled axis), would be read more accurately by more readers with less effort.

![Color saturation ranks near the bottom. Most slide designers use it as their primary encoding channel.](images/05-color-is-doing-nothing-or-harm-fig-01.png)
*Figure 5.1 — Horizontal ranked bar chart of Cleveland-McGill perceptual accuracy*

This does not mean color is useless. It means color has a specific job it is good at, and a specific job it is bad at. Color is excellent for categorical distinction when the categories are few (two or three), when the color is paired with a second encoding (a label, a shape, a position in a sort), and when the color choice is consistent — the same category uses the same color throughout the deck. Color is bad at encoding quantity, bad at working alone without a backup channel, and catastrophically bad when used inconsistently.

The Signaling Principle, which Richard Mayer derived from his multimedia learning experiments, makes the consistency requirement precise. Signaling means a cue that directs attention toward the organization of essential material. The principle's force is not "use color cues." It is "the cue must mean the same thing every time it appears." A color that means one thing on slide three and something else on slide seven — or means nothing, and is just decorative variation — is not a weak signal. It is anti-signal. The reader's brain searches for the rule, finds no rule, and has paid a cognitive cost for nothing.

There is also a fact about human vision that is non-negotiable and widely ignored. Approximately eight percent of men of Northern European ancestry have some form of red-green color vision deficiency. In a lecture hall of one hundred men from that population, about eight of them cannot reliably distinguish red from green. A chart encoded in red and green alone is, for those eight students, an unencoded chart. They are not paying less attention. They are receiving information that is invisible to them, through no fault of their own. This is not a rare edge case. It is a routine fact about a significant fraction of the population that most slide authors ignore every time they make a chart.

---

## The contrast problem

Separate from encoding is the question of legibility — whether the text on the slide can be read at all.

The W3C Web Content Accessibility Guidelines specify a contrast ratio of at least 4.5:1 for normal text against its background, and 3:1 for large text (roughly 18-point regular or 14-point bold and above), to meet Level AA. The ratio is a measure of relative luminance: a ratio of 1:1 is the same color on the same color; a ratio of 21:1 is black on white. The AA standard represents approximately the minimum readable contrast for someone with moderately reduced vision.

But here is the thing about projection: a classroom is a harder environment than a laptop screen. Ambient light from windows and overhead fluorescents washes out perceived contrast. Projector bulbs vary in quality and age. The student in the back row is at a greater distance, with less resolution, in a room the slide designer has never visited. Practitioner consensus — Tufte, Reynolds, the visual design literature broadly — targets 7:1 or higher in projection contexts as a margin against environmental degradation. WCAG's AAA level, 7:1 for normal text, is the practical target for any slide that will be projected.

Gradient backgrounds fail this test structurally, not just in specific implementations. A gradient is a continuous range of luminance values across the slide. The headline that achieves 6:1 contrast at the light end of the gradient achieves 2:1 at the dark end. The same headline, on the same slide, is legible in one region and invisible in another. There is no gradient configuration that keeps every text element in every region above a stable contrast ratio. The only fix is a solid background, which has one luminance value, and every text element can be checked against it precisely.

This is worth naming directly: a gradient background is an architectural choice that makes contrast compliance impossible to verify or guarantee. It is not a style preference. It is a structural obstacle to legibility.

![A gradient is not one contrast ratio. It is hundreds. You cannot pass them all.](images/05-color-is-doing-nothing-or-harm-fig-02.png)
*Figure 5.2 — Showing same headline text ("Q3 Results") rendered at*

---

## What the failure looks like

The slide I want to examine has a title: "Q3 Results: Three Initiatives." The content is a status report on four projects. The AI tool produced it from a brief.

The background is a teal-to-purple gradient. The headline is navy. Four bullets list the four initiatives, each in a different color: red, green, orange, blue. Below the bullets, a bar chart shows percent complete for each initiative, with each bar in a saturated color matching its bullet. A yellow badge in the upper right reads "NEW" in white text.

![Mockup of the failing slide ](images/05-color-is-doing-nothing-or-harm-fig-03.png)
*Figure 5.3 — Mockup of the failing slide *

Let me count the problems.

The yellow badge: white text on yellow background. The contrast ratio is approximately 1.07:1. That is functionally indistinguishable from white on white. The badge is invisible. The constraint it was supposed to satisfy — calling attention to what is new — is not met.

The headline: navy text on a teal-to-purple gradient. The contrast ratio varies from approximately 6:1 at the lightest part of the gradient to 2.1:1 at the darkest. The headline is readable on part of the slide and invisible on another part. Whether a given student can read it depends on which region of the gradient happens to sit behind the specific letters they are trying to parse.

The bullet colors: four distinct saturated colors, one per bullet. What does red mean? Nothing. What does green mean? Nothing. The four colors are decorative differentiation, not semantic encoding. But wait — red is on bullet A, which is labeled "on track," and green is on bullet B, which is labeled "ahead of plan." Red for "on track" and green for "ahead of plan" accidentally inverts a deeply learned color convention. In most contexts, red signals a problem and green signals success. The slide has assigned them backwards relative to their actual content. The decorative choice has become a misleading signal, which is worse than no signal at all.

The chart: four bars, each in a saturated color, rendered in 3D perspective. The 3D perspective means bars closer to the viewer appear larger than bars farther away, regardless of their actual values. A reader trying to compare the four percent-complete values by bar height is getting distorted information from the visual encoding. Cleveland and McGill named this in 1984: volume is near the bottom of the accuracy ranking. The 3D chart is a device for making the data harder to read while appearing more sophisticated.

And the underlying color problem: Initiative C is the one that is delayed. That is the piece of information the slide should be organized around — the one claim the slide should make. But Initiative C's bullet is in orange, which has no more salience than the red, green, and blue of the other three. The signal — "this one is the problem" — is invisible under three other colors of equal visual weight.

The slide has six colors doing decorative work and zero colors doing the one job that matters.

---

## What the repair looks like

Same content. Different decisions.

![Mockup of the repaired slide ](images/05-color-is-doing-nothing-or-harm-fig-04.png)
*Figure 5.4 — Mockup of the repaired slide *

The background becomes a single solid near-white. Every contrast relationship on the slide is now stable and checkable.

The color budget for the slide is two: a dark neutral for everything that is body content, and one accent for the one thing the slide is saying.

What is the slide saying? Initiative C is delayed. That is the claim. That is where the accent goes.

The four bullets are now in dark gray — body text, no color differentiation. Next to Initiative C's entry, the word "DELAYED" appears in the accent color. The chart is four horizontal bars sorted by percent complete, three in dark gray, one — Initiative C — in the accent. The chart is two-dimensional, axis-labeled, sorted so the reader can compare bars by position along a common scale.

Red appears exactly twice on this slide: once in the text ("DELAYED") and once in the chart (the C bar). Both instances mean the same thing. A reader scanning the slide for half a second knows where to look. The encoding survives colorblindness because red is paired with the text label and with bar position — a reader who cannot see the red still reads "DELAYED" in the text and still sees the bar sitting last in the sort. The encoding survives projection because dark gray on near-white passes contrast requirements by a wide margin.

Total colors visible on the live slide: two. Color attention spent: one place. The eye has nowhere to go but where the slide is pointing it.

The word count on the bad slide and the good slide is identical. The content is identical. The only thing that changed is the decision about what each color is *for*.

---

## The asymmetry of detection

The bad slide looks more designed than the good slide. That is not an accident and it is not a trivial observation.

AI tools that generate slides are optimizing for a signal they can measure from training data: visual interest. Visual interest, measured at the level of pixel patterns in the training corpus, correlates with color variety, gradient sophistication, and decorative density. The tool produces the gradient, the four saturated bullet colors, the 3D chart, and the yellow badge because those features appear in slides that human raters have called polished or professional.

But the tool has no access to the cognitive experience of the student in the third row of a lecture hall, trying to process a gradient-background slide while a speaker is talking. The tool cannot measure working memory load, cannot simulate colorblindness, cannot check a contrast ratio, cannot ask "what does red mean on this slide?" The tool has learned the surface of professionalism and not its function.

This is the same asymmetry as Chapter 1's midnight desk problem, applied to color. The slide that looks finished is the one that is failing. The slide that looks spare — two colors, solid background, the accent where the claim is — looks underdesigned by the tool's aesthetic standard and works correctly by the cognitive standard.

The fix, when working with AI tools, is to give the tool an explicit color policy before it generates. Not "use professional colors" but specific rules: what the palette is, what the accent is for, what the background is, what the contrast floor is. The tool will follow explicit constraints more reliably than it will infer good design from vague aesthetic direction.

The prompt, portable to any AI slide tool:

---

*Restrict this slide to a two-color palette: one neutral for backgrounds, body text, and chart marks, and one accent for the elements that carry the slide's claim.*

*Reserve the accent for exactly the parts of the slide the audience should look at first. Every other element uses the neutral.*

*If color encodes categories in a chart, pair it with at least one other channel: shape, position in a sort, or a text label. The encoding must survive loss of color discrimination.*

*Ensure every text-against-background pairing meets WCAG contrast of 4.5:1 minimum. For projection, target 7:1.*

*Use a solid background. No gradients.*

*If a colorblind-safe pair is needed for two categorical colors, use blue-orange rather than red-green.*

---

Two things to notice about this prompt. First, it specifies the role of each color before naming the color. "One neutral, one accent" is a structural rule. "The accent goes where the claim is" is a semantic rule. Together they give the tool a decision procedure rather than an aesthetic preference to approximate. Second, the colorblind-safe pair is named explicitly because the tool will otherwise default to red-green, which is the most intuitive pair and the most common colorblindness failure mode. You have to name the exception.

---

## The design principle underneath

Cleveland and McGill, Mayer's Signaling Principle, WCAG contrast ratios, and the colorblindness statistics are four different research traditions all pointing at the same practical conclusion: color is a finite, fragile resource that only works when it is used sparingly, consistently, and with backup.

The finite part: working memory cannot attend to more signals than it has capacity for. Color that does not encode is spending capacity the reader cannot recoup.

The fragile part: color is the weakest quantitative channel. It depends on ambient light, projector quality, display calibration, and individual color vision — all of which vary. A chart that is readable only under ideal conditions is not a chart the designer can rely on.

The backup part: any encoding that uses color as its only channel fails for some fraction of readers. Pairing color with a label, a position, or a shape makes the encoding redundant in the engineering sense — if one channel fails, another carries the information through. That is what accessibility actually means in practice: not a special accommodation for a minority, but an architectural property that makes the signal robust to the conditions of the real world.

![Paired encoding (color + label + position) survives colorblindness. Color alone does not.](images/05-color-is-doing-nothing-or-harm-fig-05.png)
*Figure 5.5 — Colorblind simulation *

Tufte's phrase for this in *Envisioning Information* is "small effective differences" — the discipline of using the minimum visual variation needed to make the distinction, so that variation is available for the moments that matter. Loud color is usually a confession that the structure beneath it is not doing its job. Six saturated category colors usually mean the categories are not being separated by position, label, or hierarchy, and color is compensating for structural failures it cannot fix.

The elegant version of the principle is simple: if you cannot say what a color means in one word, it should not be on the slide.

---

## What two instructors might argue about

Two reasonable designers can read this chapter and disagree honestly about how austere a slide should be.

One position: color is one of the most powerful affective channels available to a designer. A deck that uses only dark gray and one accent is clinical, maybe joyless. A faculty member teaching a hundred first-year students at eight in the morning cannot afford to look austere. The argument is that a richer palette, used with deliberate restraint, is better than minimal palette. That four or five colors, even when not all semantically loaded, can signal energy, credibility, and care — things that matter for an audience's willingness to engage.

The other position: every color beyond the two doing semantic work is competing with the two doing semantic work. Austere is not the cost of precision — it is the form precision takes. The student who is confused about what red means has paid a cognitive cost that warmth and energy cannot reimburse.

The vocabulary for the disagreement is the question — *what does this color encode?* If the answer is a specific job — *this category*, *this method*, *this concept* — the color earns its place. If the answer is "it adds warmth" or "it matches the brand," the color is decoration. On that, the two positions converge: decoration on instructional slides is the failure mode both camps are trying to avoid. They disagree about whether some decorative color, deployed carefully, costs less than it buys. That is a defensible disagreement that will not be resolved by a single study.

One thing that is not a disagreement: the contrast standard. WCAG 2.2 was finalized in October 2023 and is the current normative version; the contrast requirements are unchanged from 2.1. APCA, an experimental successor algorithm under consideration for a future version of the standard, aims to better model how humans perceive contrast at different text sizes and weights. As of this writing, APCA is not normative and using it now is a forward bet, not a current best practice. The reader designing for the future should know it exists. The reader preparing this week's lecture should use WCAG 2.1/2.2 ratios and check them with a contrast tool before projecting.

---

## Exercises

**Warm-up**

1. A slide has five elements: a dark gray headline on white, a red callout box, a blue hyperlink in the body text, a green checkmark icon, and an orange footer. For each element, answer in one word: what does this color encode? If you cannot answer, classify the color as decorative. *Tests: ability to apply the "one-word encoding" diagnostic.*

2. A bar chart shows sales figures for four regions. The designer has used four distinct saturated colors — red, blue, green, orange — one per bar, with no axis labels and no text labels on the bars. According to the Cleveland-McGill hierarchy, what is the problem with using color as the primary encoding here, and what channel should replace it? *Tests: understanding of Cleveland-McGill and color's position in the accuracy ranking.*

3. A faculty member projects a slide with medium gray text (#888888) on a white background (#FFFFFF). Using the WCAG relative luminance formula — or a contrast checker tool — calculate the approximate contrast ratio and determine whether it meets AA for normal text (4.5:1) or large text (3:1). Does it meet the 7:1 projection target? *Tests: ability to apply WCAG contrast standards to a specific color pair.*

**Application**

4. A line chart in a climate science lecture shows two trajectories: "Pre-industrial baseline" encoded in green and "Current trend" encoded in red. The lines diverge sharply in the final third of the chart. Redesign the encoding so that: (a) the chart communicates correctly to a red-green colorblind reader, and (b) the chart uses a backup channel beyond color. Name the specific changes you would make and why each one addresses a different failure mode from this chapter. *Tests: applying paired-encoding principle and colorblind-safe palette choice.*

5. An AI-generated slide uses a teal-to-purple gradient background. The headline achieves 5.5:1 contrast at the lightest region of the gradient. Explain why this slide cannot pass a WCAG contrast audit regardless of the headline color chosen, and what architectural change is required to make verification possible. *Tests: understanding of gradient backgrounds as structurally incompatible with stable contrast.*

6. You inherit a six-color slide deck from a colleague. Before the next lecture, you have fifteen minutes to apply the two-color discipline from this chapter to one slide. Walk through the steps: what is the slide's claim, which color should become the accent, which elements revert to neutral, and what do you check before projecting? *Tests: ability to execute the two-color repair under time constraints.*

**Synthesis**

7. The chapter argues that "loud color is usually a confession that the structure beneath it is failing." Take a slide from a deck you have built that uses four or more colors. Audit it: is the color density compensating for missing labels, missing sort order, or missing categorical hierarchy? If yes, fix the structure first, then reapply the color rule. Describe what changed and why fixing the structure made the color question easier. *Tests: ability to see color as a symptom of structural failure, not the failure itself.*

8. A colleague pushes back: "My students need visual engagement — two colors looks like a government memo." Using the vocabulary from "What two instructors might argue about," construct the strongest version of your colleague's argument, then construct the strongest rebuttal. Where exactly do the two positions converge, and where do they genuinely diverge? *Tests: ability to use the chapter's disagreement vocabulary precisely and distinguish the genuine dispute from the apparent one.*

**Challenge**

9. WCAG 2.2 (current) and APCA (proposed for a future version) give different contrast recommendations for the same text-background pair at small sizes. Research the specific difference in how the two algorithms handle light text on dark backgrounds at 14pt. Which algorithm would you use for a slide deck today, and what would change about your recommendation if APCA becomes normative? *Tests: ability to reason about forward-looking standards decisions under current uncertainty; requires research beyond the chapter.*

---

## Prompts

Use these prompts with Claude to generate interactive D3 v7 versions of the
figures in this chapter. Each produces a standalone HTML file you can open
in a browser and modify freely.

**Prerequisites:** Load `brutalist/CLAUDE.md` and `brutalist/DESIGN.md` into
your Claude project context before using these prompts. They define the stack,
naming conventions, color system, and typography the figures use.

---

### Figure 5.1 — Horizontal ranked bar chart of Cleveland-McGill perceptual accuracy

Create a standalone D3 v7 HTML file for Figure Horizontal ranked bar chart of Cleveland-McGill perceptual accuracy. Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: horizontal ranked bar chart of Cleveland-McGill perceptual accuracy hierarchy — bars from top (most accurate) to bottom (least): Position on common scale, Position on non-aligned scale, Length, Angle/slope, Area, Volume/density, Color saturation/hue; the "Color saturation/hue" bar highlighted in accent color; caption: "Color saturation ranks near the bottom. Most slide designers use it as their primary encoding channel.". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variables and the required serif/mono font split.

> Reference implementation: `d3/05-color-is-doing-nothing-or-harm-fig-01.html`

---

### Figure 5.2 — Showing same headline text ("Q3 Results") rendered at

Create a standalone D3 v7 HTML file for Figure Showing same headline text ("Q3 Results") rendered at. Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: side-by-side showing same headline text ("Q3 Results") rendered at three points across a teal-to-purple gradient background — left point contrast 6.1:1 labeled "AA pass", middle point 3.8:1 labeled "AA fail", right point 2.1:1 labeled "severe fail"; below it, the same headline on a solid near-white background showing a single stable ratio of 12:1 labeled "AAA pass, everywhere"; caption: "A gradient is not one contrast ratio. It is hundreds. You cannot pass them all.". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variables and the required serif/mono font split.

> Reference implementation: `d3/05-color-is-doing-nothing-or-harm-fig-02.html`

---

### Figure 5.3 — Mockup of the failing slide 

Create a standalone D3 v7 HTML file for Figure Mockup of the failing slide . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: rendered mockup of the failing slide — teal-to-purple gradient background; navy headline "Q3 Results: Three Initiatives"; four colored bullets (red: "Initiative A: on track", green: "Initiative B: ahead of plan", orange: "Initiative C: delayed", blue: "Initiative D: scope changed"); 3D perspective bar chart with four saturated bars matching bullet colors; yellow badge upper right reading "NEW" in white; six annotation callouts: (1) badge "contrast 1.07:1 — invisible", (2) headline "contrast 2.1:1–6:1 — unstable", (3) red bullet "red = 'on track' — inverts learned convention", (4) green bullet "green = 'ahead of plan' — also inverts convention", (5) orange bullet "the actual problem (delayed) is visually equal to all others", (6) chart "3D distorts bar lengths — volume encoding, lowest accuracy". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that

> Reference implementation: `d3/05-color-is-doing-nothing-or-harm-fig-03.html`

---

### Figure 5.4 — Mockup of the repaired slide 

Create a standalone D3 v7 HTML file for Figure Mockup of the repaired slide . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: rendered mockup of the repaired slide — solid near-white background; dark gray headline "Q3 Results: Three Initiatives" contrast callout 12:1; four bullets in dark gray body text, Initiative C line reading "Initiative C DELAYED" with "DELAYED" in red accent; horizontal bar chart below, four bars sorted by % complete, three in dark gray, one (Initiative C) in red accent, axis labeled "% complete" with values 0–100, no 3D; annotation callouts: (1) "two colors only: dark gray and one accent", (2) "accent used twice — same meaning both times", (3) "chart sorted by value: position on common scale is primary encoding", (4) "red + text label + bar position: encoding survives colorblindness". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, a

> Reference implementation: `d3/05-color-is-doing-nothing-or-harm-fig-04.html`

---

### Figure 5.5 — Colorblind simulation 

Create a standalone D3 v7 HTML file for Figure Colorblind simulation . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: two-panel colorblind simulation — left panel: the repaired slide rendered under deuteranopia simulation (red-green colorblindness); right panel: a red-green encoded chart with no labels rendered under same simulation; in the left panel, the "DELAYED" text label and bar position still clearly identify Initiative C; in the right panel, the two lines are indistinguishable; caption: "Paired encoding (color + label + position) survives colorblindness. Color alone does not.". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variables and the required serif/mono font split.

> Reference implementation: `d3/05-color-is-doing-nothing-or-harm-fig-05.html`
