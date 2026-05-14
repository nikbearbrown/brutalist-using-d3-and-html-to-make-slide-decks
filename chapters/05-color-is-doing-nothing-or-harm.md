# Chapter 5 — Color Is Doing Nothing (or Harm)

> Every color on the slide is either encoding something or competing with what is. Find out which. Cut the rest.

---

## 1. The feeling

A slide opens up. The background is a soft teal-to-purple gradient. The headline is in deep navy. Below the headline, four bullets: one in red, one in green, one in orange, one in blue. The body copy under each bullet is in a pale gray — readable on the lighter part of the gradient, half-vanishing on the darker part. There is a brand-color stripe down the left side. Three icons in the corner are filled with three different colors. A circular badge in the upper right reads "Updated 2025" in white on yellow.

Nothing is wrong with any individual element. The slide looks polished. It came out of a Canva template, or a Gamma generation, or an AI image tool's "professional" preset.

But look at it for ten seconds. Where does your eye go first? Where does it want to land? What does the red bullet mean? What does the green one mean? Are they paired? Is one good and one bad? The brain is searching for a pattern the slide is not delivering. The search is invisible. The cost is not.

Or this: a slide showing two trajectories — "Intervention" in green, "Control" in red — across five time points. The lines cross. In the projection booth from the back row, the colors blur into a single muddy hue. The instructor talks about which group did better. Eight percent of the male students in the room cannot tell which line is which. They are not paying less attention. They are receiving an unencoded chart.

Or this: an AI-generated hero image at the top of the slide — a stylized illustration with a low-contrast text overlay in a thin sans-serif. The text is dark gray on a medium gray gradient. On a laptop at desk distance, it's legible. Projected, it is nearly invisible from the third row.

That is the feeling this chapter is about. Color that looks like decoration and acts like noise, or color that *is* encoding and fails for the readers who need it.

---

## 2. The two diagnostic questions

**Cognitive science question:** *Is each color carrying meaning, or is it decoration?*

This is Mayer's [Signaling Principle](https://pmc.ncbi.nlm.nih.gov/articles/PMC10845804/) reduced to a single test. Signaling means a cue that directs attention to the organization of essential material. The principle's force is not "use cues." It is "the cue must mean the same thing every time it appears, consistently across the deck, and that meaning must serve the structure of the content." Color used inconsistently is not a weak signal. It is anti-signal — the reader searches for a pattern that does not exist, and the search itself burns working memory you needed for the content.

**Visual design question:** *Does each color-on-color pairing meet WCAG contrast minimums, and is the palette colorblind-safe?*

The [W3C Web Content Accessibility Guidelines](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum) specify a contrast ratio of at least 4.5:1 for normal text against its background and 3:1 for large text (18pt regular or 14pt bold and above) to meet Level AA conformance. AAA, the higher tier, is 7:1 for normal text. The standard was originally developed for screens viewed at arm's length. Projection in a classroom is a harder problem. Ambient light from windows, fluorescents, and projector bulbs of variable quality degrades perceived contrast. Practitioner consensus — Tufte, Reynolds, the design literature broadly — is to target 7:1 or higher in projection contexts as a margin against degradation. And about 8% of men of Northern European ancestry have some form of red-green color vision deficiency ([Birch 2012](https://pubmed.ncbi.nlm.nih.gov/22472762/)). A chart encoded in red and green alone is, for those readers, an unencoded chart.

Always both questions. Always in that order. The encoding question is upstream; if the color is decorative, no contrast fix will save it. The contrast question is downstream; if the color is doing real signaling work, it has to be readable for everyone.

---

## 3. The principle named

Plain language first: **every color on the slide is either doing a specific job or it is making the slide worse.** There is no neutral color. Color that does not encode is competing with color that does.

If you cannot answer "what does this color mean?" in one word — *error*, *this category*, *this method*, *the new term* — the color is decoration. Decoration is not neutral on instructional slides. It draws attention you needed elsewhere. The Signaling Principle is finite-capacity: there are only so many cues the reader can attend to. Spending the capacity on decoration leaves none for encoding.

Framework vocabulary: this is the Signaling Principle being honest about its scarcity. It is also Tufte's "small effective differences," from [*Envisioning Information*](https://www.edwardtufte.com/book/envisioning-information/) — the discipline of using the minimum visual variation needed to make the distinction. Loud color is usually a confession that the structure beneath it is failing to distinguish itself. Six saturated category colors usually mean the categories are not being separated by position, size, or label, and color is over-compensating. Fix the structure first. The color question gets easier the moment the structure is right.

And it is Cleveland and McGill again. Their [1984 ranking](https://www.tandfonline.com/doi/abs/10.1080/01621459.1984.10478080) places color saturation near the bottom of perceptual-accuracy tasks. Color is one of the *weakest* channels for encoding quantitative information. Using it as the primary signal — without backing it with position, size, label, or shape — is asking the weakest channel to do the heaviest work.

---

## 4. Bad example

Slide title: **"Q3 Results: Three Initiatives"**

Here is what the AI tool produced — the kind of slide that wins on first impression and fails on third.

```
+----------------------------------------------------------+
|  [teal-to-purple gradient background, 100% coverage]    |
|                                                          |
|  Q3 Results: Three Initiatives          [yellow badge:   |
|  (navy on gradient — contrast varies)    "NEW" in white] |
|                                                          |
|  • Initiative A:  on track          [red bullet glyph]  |
|  • Initiative B:  ahead of plan     [green bullet glyph]|
|  • Initiative C:  delayed           [orange bullet glyph]|
|  • Initiative D:  scope changed     [blue bullet glyph] |
|                                                          |
|  [chart: 4 bars, each a different saturated color,       |
|   showing % complete, no axis labels, 3D perspective]    |
|                                                          |
|  Source: internal report                                 |
+----------------------------------------------------------+
```
<!-- annotation: gradient background changes the contrast of every element on the slide from top to bottom. Text legible at the top, fails at the bottom. -->
<!-- annotation: four bullet colors. Asked "what does red mean?" the maker says "it's just a different color for each bullet." That is decoration sold as signal. The reader's brain searches for what red encodes and finds nothing. -->
<!-- annotation: but red on bullet A — for "on track" — and green on bullet B — for "ahead of plan" — accidentally invert a deeply learned convention (red = warning, green = good). The accidental encoding contradicts the actual data. The signal is worse than absent; it is misleading. -->
<!-- annotation: yellow badge in upper right ("NEW"): white text on yellow background. WebAIM contrast checker: 1.07:1. Functionally invisible. -->
<!-- annotation: navy headline on teal-purple gradient: contrast ratio varies from approximately 6:1 at the lightest part to 2.1:1 at the darkest. The same headline is legible on one slide and unreadable on the next, depending on which part of the gradient sits behind it. -->
<!-- annotation: chart uses 3D perspective: bars closer to the viewer appear larger regardless of value. A reader cannot reliably compare magnitudes. Cleveland-McGill: volume is near the bottom of perceptual accuracy. -->
<!-- annotation: chart uses four saturated colors with no semantic role — color is the category label, but the category labels are also right there in text. Color is redundant and adds visual noise. -->
<!-- annotation: pale gray secondary text (Source) at the bottom: against the dark end of the gradient, contrast ratio approximately 1.8:1. Below AA, below AAA, below readable. -->

The slide has six colors doing decorative work and zero colors doing semantic work. The one place a color *could* have done a job — flagging "delayed" as a problem — is buried under three other decorative colors. The signaling channel is saturated with noise.

This is the most common slide failure mode in AI-generated decks. The tool optimizes for visual interest, which it measures by color variety and gradient sophistication. Visual interest measured that way is anti-correlated with comprehension. Canva's default templates frequently fail WCAG contrast on header overlays — not because the designers do not know, but because the templates have to look striking in the gallery, and striking is hard to do with high contrast.

---

## 5. Good example

Same slide title. Same content. Color discipline applied.

```
+----------------------------------------------------------+
|  [solid #FAFAFA background — light neutral, no gradient]|
|                                                          |
|  Q3 Results: Three Initiatives           [dark gray,    |
|                                            contrast 12:1]|
|  —————————————                                            |
|                                                          |
|  Initiative A   on track                                 |
|  Initiative B   ahead of plan                            |
|  Initiative C   DELAYED              ← red accent here   |
|  Initiative D   scope changed                            |
|                                                          |
|  [chart: 4 horizontal bars sorted by % complete.         |
|   Three bars in neutral dark gray. The C bar in red.     |
|   Axis labeled "% complete" with values 0, 50, 100.      |
|   No 3D. No perspective.]                                |
|                                                          |
|  Source: internal report Q3 2025  [secondary gray 7:1]   |
+----------------------------------------------------------+
```
<!-- annotation: background is one solid light neutral. Every element on the slide has a stable, known contrast relationship with the background. -->
<!-- annotation: two colors total on the slide. Dark gray (everything that is body text or chart neutral) and one red (the one place the slide is making a claim — Initiative C is the problem). -->
<!-- annotation: red is used exactly once in the text ("DELAYED") and exactly once in the chart (the C bar). The reader's eye lands on red without searching. The signal is consistent across the slide and would be consistent across the deck if the convention is maintained. -->
<!-- annotation: chart is sorted by value. Cleveland-McGill: position along a common scale is the highest-accuracy perceptual encoding. The reader compares the four bars by length and by ordering. -->
<!-- annotation: red is paired with a textual label ("DELAYED") and with bar position (last in the sort). Even a reader with red-green color deficiency reads the encoding correctly. -->
<!-- annotation: headline contrast: dark gray (#222) on near-white background, ratio 14:1. AAA-compliant by a wide margin. -->
<!-- annotation: secondary text (Source line) contrast: medium gray (#595959) on near-white, ratio 7.0:1. AAA-compliant. -->
<!-- annotation: total color budget on the slide: two functional colors. Color attention spent: one place. Signal-to-noise ratio: high. -->

What changed: the slide stopped using color to look interesting and started using color to mean one thing.

Red appears twice. Both times it means the same thing: "this is the thing the slide is calling out as a problem." A reader scanning the slide for half a second knows where to look. A reader reading carefully gets the rest of the context. The encoding survives colorblindness because red is paired with text ("DELAYED") and position (last in the sort). The encoding survives projection because red on near-white passes contrast at the back row.

The gradient is gone. Solid backgrounds are not a stylistic preference here. They are the only way to make contrast ratios stable across the slide. A gradient is a thousand different contrast ratios in one image, and you cannot pass them all.

The chart is two-dimensional and sorted by value. Three of the four bars are in a neutral; one is in the accent. The chart is doing the same work as the text — using one color, in one place, with one meaning.

---

## 6. The prompt

Paste this into the Brutalist system on any slide where the color feels off — or where it does not feel off but you have not actually checked.

> Restrict this slide to a two-color palette: one neutral (for backgrounds, body text, and chart marks) and one accent (for the element or elements that carry the slide's claim).
>
> Reserve the accent color for exactly the parts of the slide that the audience should look at first. Every other element uses the neutral.
>
> If color is encoding categories in a chart, pair the color with at least one other channel: shape, position in a sort, or a textual label. The encoding must survive loss of color discrimination.
>
> Ensure every text-against-background pairing meets WCAG AA contrast (4.5:1 for normal text, 3:1 for text 18pt or larger). For projection in a classroom, target 7:1 where feasible.
>
> Avoid gradient backgrounds. Use a single solid background per slide so contrast ratios are stable.
>
> Choose colors from a colorblind-safe palette ([ColorBrewer](https://colorbrewer2.org/) is the standard reference). The blue-orange pair is the most reliably distinguishable across the common color vision types and is a safe default when red-green would be intuitive.

The prompt is portable. The Brutalist system can implement it directly through DESIGN.md variables. In Canva or Gamma, the same prompt works as a design directive against the template — overriding the tool's default palette is harder there but possible.

---

## 7. The DESIGN.md change

Five variables, with roles and contrast ratios documented.

```yaml
# DESIGN.md
palette:
  background: "#FAFAFA"        # near-white neutral; AAA-safe with dark gray text
  text_primary: "#222222"      # 14:1 against background; AAA
  text_secondary: "#595959"    # 7:1 against background; AAA
  neutral_mark: "#595959"      # default chart and rule color
  accent: "#B81D24"            # brand red; signaling-only

accent_color_uses_per_slide_max: 2

contrast_minimum:
  text_normal: 4.5             # WCAG 2.1 AA
  text_large: 3.0              # WCAG 2.1 AA, 18pt+ or 14pt bold+
  projection_target: 7.0       # practitioner standard; not a WCAG level

palette_rule: "Accent color is reserved for elements that carry the slide's
               claim. Body text, headlines, and chart neutrals use the
               grayscale ramp. No color outside the palette without
               updating DESIGN.md and documenting what it encodes."

forbidden_palette_uses:
  - "gradient backgrounds"
  - "color as the only encoding channel in a chart"
  - "more than two accent colors anywhere in the deck"
```

One sentence why each variable matters:

- `accent_color_uses_per_slide_max: 2` — beyond two uses, the eye stops treating the accent as signal and starts treating it as another category. The whole encoding collapses.
- `contrast_minimum.text_normal: 4.5` — the accessibility floor for text; below this, readers with typical age-related vision loss cannot read the slide.
- `palette_rule` (red as brand-only, never danger) — this is a workshop convention, not a research finding. Two reasonable designers can disagree. The point is that *some* convention is documented, not that this particular one is uniquely correct.

The reader's DESIGN.md may end up with different specific values. The discipline is the point: every color in the palette has a role, every role has a contrast ratio, and every variable can be defended in one sentence. If you cannot say what a variable does, the variable is not yet a decision.

---

## 8. The diagnostic questions to keep

Run these on any slide. Under thirty seconds each.

1. **What does each color on this slide encode?** Answer in one word per color. If the answer is "decoration" or silence, the color is failing. Add it to the cut list.

2. **Does every text-against-background pairing pass 4.5:1?** Use [WebAIM's contrast checker](https://webaim.org/resources/contrastchecker/) — two hex codes in, ratio out. The check takes ten seconds per pairing. There is no excuse for not doing it.

3. **If I converted this slide to grayscale, would any information disappear?** Anything that vanishes was encoded in color alone. That is the colorblind-failure inventory. Either add a second encoding (label, position, shape) or accept that those readers will not get the information.

4. **Could I run this slide through [Color Oracle](https://colororacle.org/) once and be unsurprised by what I see?** The simulator runs on Mac, Windows, and Linux for free. Two minutes per deck.

5. **Have I spent my color budget where the slide is making its claim — or have I spent it on decoration that has nothing to claim?** Color is a finite attention resource across the deck. Spending it on backgrounds and accents that mean nothing leaves none for the moments where color needs to carry meaning.

---

## 9. What two people might disagree about

Two reasonable designers will disagree about how much personality color can carry before it becomes noise.

One position: color is one of the most powerful affective channels available to a designer. A deck that uses only dark gray and one accent reads as austere, clinical, joyless. A deck that uses a coordinated palette of four or five colors — even when not all of them are semantically loaded — feels alive. Faculty who teach in fields where engagement matters (a 100-person intro lecture at 8 a.m.) cannot afford austere. The recommendation: use a richer palette with deliberate restraint, not minimal palette.

The other position: every color beyond the two doing semantic work is competing with the two doing semantic work. The reader's attention is a finite resource and color spending is zero-sum across the deck. Austere is not the cost. Austere is the form precision takes. The recommendation: two colors, always, until the slide has earned a third.

The vocabulary for the disagreement is the question *what does this color encode?*. If the answer is a specific job — *this category*, *this method*, *this concept* — the color earns its place. If the answer is "it adds warmth" or "it matches the brand" or "it looks better," the color is decoration and the two positions converge: decoration on instructional slides is the failure mode.

There is also a real shift in the standard worth flagging. WCAG 2.2 [was finalized in October 2023](https://www.w3.org/TR/WCAG22/) and is the current normative version as of this draft; the contrast requirements are unchanged from 2.1. APCA (the Accessible Perceptual Contrast Algorithm) is an experimental successor under consideration for WCAG 3.0, which aims to better reflect human perception of contrast at different text sizes and weights. APCA is not yet a standard [verify — believed still draft/non-normative as of 2026] and using it now is a forward bet, not a current best practice. The reader designing for the next ten years should know it exists. The reader designing this week's lecture should use WCAG 2.1/2.2 contrast ratios and not wait.

One last note: AI-generated images on slides are a high-frequency failure mode for this chapter. The tools produce polished-looking decorative images with low-contrast text overlays, arbitrary color schemes, and gradient backgrounds that violate every diagnostic in this chapter — and the failure is invisible to the untrained eye precisely because the image looks designed. The fix is the same as it would be for any image: ask what each color encodes, run the contrast checker, and either accept the answer or replace the image. AI-generated images are not exempt from the rules. They just hide the violation more effectively.

---

The eye is now trained for individual slides. Color encoding is also the primary instrument for retrofitting one of the hardest cases on a slide: a complex figure that was designed for a textbook page and dropped, unedited, into a deck. That is Chapter 6.
