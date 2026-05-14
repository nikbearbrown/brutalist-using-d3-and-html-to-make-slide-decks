# Research Notes: Chapter 5 — Color Is Doing Nothing (or Harm)

**Source:** TIKTOC.md chapter entry
**Notes file:** 05-color-is-doing-nothing-or-harm_notes.md
**Corresponding chapter:** chapters/05-color-is-doing-nothing-or-harm.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns to distinguish semantic color (encodes meaning) from decorative color (adds noise), apply the contrast ratio test, and check for colorblind failure — then update DESIGN.md with precision.

**The feeling:** A slide that looks colorful but where the color doesn't seem to mean anything. Or a slide where something is hard to read without knowing why.

**Three failure modes:**

*Failure 1 — Decorative color:* Color used for aesthetics, not information. "If everything is colorful, nothing stands out." The signaling principle requires that color means the same thing every time it appears. Random color use destroys the signal.

*Failure 2 — Contrast failure:* Text or marks that fail the WCAG 2.1 AA standard (4.5:1 for text, 3:1 for graphical elements). In projection environments with ambient light, target 7:1+. The reader cannot see it. This is an accessibility failure and a design failure simultaneously.

*Failure 3 — Colorblind inaccessibility:* 8% of men, 0.5% of women have red-green color vision deficiency. A slide that uses red and green alone to encode distinctions fails for 1 in 12 male students before the first word is spoken.

**The Brutalist palette rule:** DESIGN.md specifies six variables. Red is brand and primary series — never danger or negative. Ochre is decorative accent only — never body text. Gray scale for everything else. This is not arbitrary — it is colorblind-safe and contrast-tested.

**The test:**
1. Does each color encode something specific and consistent?
2. Does every text element pass 4.5:1 contrast against its background?
3. Would a colorblind reader lose any information?

**Prompt category:** DESIGN.md color variable update with contrast ratio and semantic role specified.

**DESIGN.md variables:** All six color variables, with roles and contrast ratios documented.

**What two people disagree about:** How much personality color can carry before it becomes noise. The vocabulary for this disagreement: "what is this color encoding?" — if the answer is "nothing," the disagreement is settled.

**Bridge:** The eye is now trained on individual slides. The next category of failure is the textbook figure that arrived on the slide without redesign. That is Chapter 6.

---

## A. Conceptual foundations

### 1. Signaling: color as encoding, not decoration

Mayer's Signaling Principle (sometimes called the Cueing Principle) states that people learn better from a multimedia message when cues are added that highlight the organization of the essential material. Color is one of the most powerful signaling channels available — and one of the most commonly squandered. The principle's force is not "use color." The force is "color must mean the same thing every time it appears, and that meaning must serve the structure of the content." Color used inconsistently is not a weak signal. It is anti-signal — actively misleading the reader into searching for a pattern that isn't there.

The diagnostic question for Chapter 5 is therefore: "What does this color encode?" If the faculty member can answer in one word ("error," "this method," "the new term"), the color is doing work. If the answer is "it looks nice" or "for emphasis" or — most commonly — silence, the color is decoration. Decoration competes with signal. The signaling channel is finite. Color spent on decoration is color not available for encoding.

**Common misconception:** Color makes slides "more engaging" or "more lively." Engagement bought at the cost of meaning is the seductive-details failure mode applied to the visual channel. Engagement is not free; it is paid for in attention to the wrong thing.

**Worked example:** A slide where four bullets are colored red, blue, green, and orange. Asked why, the instructor says "just to make it readable." The reader's brain searches for what red means — categories? severity? — and finds nothing. The color was supposed to help. It hurt. The same slide with all four bullets in neutral text and one phrase highlighted (the one phrase that *is* the takeaway) has a working signal: the highlight means "this is what matters."

**Source:** Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press, ch. 6 on Signaling. Summary at https://pmc.ncbi.nlm.nih.gov/articles/PMC10845804/

### 2. WCAG 2.1 AA contrast ratios

The Web Content Accessibility Guidelines (WCAG) 2.1 specify a contrast ratio of at least 4.5:1 for normal-size text against its background to meet Level AA conformance. For large text (18pt regular or 14pt bold and above) the threshold drops to 3:1. For graphical elements and user interface components, the threshold is 3:1. AAA conformance — the higher tier — is 7:1 for normal text and 4.5:1 for large text. The W3C's official Understanding document explains that 4.5:1 was chosen to compensate for the loss of contrast sensitivity experienced by users with vision equivalent to approximately 20/40 (around the threshold of typical age-related vision loss).

For slide design, two things matter. First: WCAG is a digital-display standard developed for screens viewed at arm's length under controlled lighting. Projection in a classroom is harder — ambient light from windows, fluorescents, or projectors with imperfect color reproduction degrades perceived contrast. Practitioners (including Tufte and Reynolds) recommend targeting 7:1 or higher in projection contexts as a margin against degradation. Second: contrast is a computable property. The faculty member does not have to eyeball it. WebAIM's contrast checker (webaim.org/resources/contrastchecker/) takes two hex codes and returns the ratio. The chapter's prompt should include a contrast-check step.

**Common misconception:** "If I can read it on my laptop, it's fine." The laptop is a high-contrast OLED panel six inches from the user's face. The classroom projector at the back of a 60-foot room is not the same medium. Contrast ratios are not opinions about taste; they are floor specifications for legibility.

**Worked example:** A slide with a light-gray subtitle (#999999) on a white background. Contrast ratio: 2.85:1. Fails WCAG AA for normal text. The subtitle is invisible from the third row. The fix: darken to #595959 (ratio 7.0:1) — now AAA-compliant and visible in any classroom.

**Source:** W3C WAI, Understanding Success Criterion 1.4.3: Contrast (Minimum). https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum — WebAIM Contrast Checker: https://webaim.org/resources/contrastchecker/

### 3. Color-blindness prevalence and the red-green default failure

Approximately 8% of men and 0.5% of women of Northern European ancestry have some form of red-green color vision deficiency. The condition is inherited via the X chromosome, which is why men — with only one X — are far more affected than women. The most common subtype is deuteranomaly (reduced green sensitivity), followed by protanomaly (reduced red sensitivity) and the rarer full dichromacies (deuteranopia, protanopia). Worldwide prevalence varies by population but the 8%-of-men figure is stable for European-descended populations and widely cited in the visualization literature. In a classroom of 24 men, two will typically have some form of red-green deficit.

The practical consequence: a chart that encodes "this is good" vs. "this is bad" using green and red looks like one color to those students. Every chart in the deck that depends on red-green encoding is, for those students, an unencoded chart. They are not getting a hard signal; they are getting noise. This is not a hypothetical — it is the most common color-encoding failure in scientific and instructional graphics.

Two operational fixes the chapter should land. First: never encode meaning in color alone. Pair color with shape, position, or a textual label so the encoding survives loss of one channel. Second: use a colorblind-safe palette. ColorBrewer (colorbrewer2.org, Cynthia Brewer and Mark Harrower, Penn State, launched 2002) provides palettes that have been screened for colorblind compatibility, broken down by sequential, diverging, and qualitative use cases. Blue-orange is the most reliably distinguishable two-color combination across all common color vision types — a far safer default than red-green.

**Common misconception:** "I'll just avoid red and green." The problem is not red and green per se; it is using red and green *as the only encoding*. A red bar next to a green bar fails. A red bar labeled "loss" next to a green bar labeled "gain" works for everyone — the colorblind student reads the labels.

**Worked example:** A confusion matrix slide showing classification errors. The textbook colors true positives green, false negatives red. For 8% of male students, the matrix is two indistinguishable cells. Fix: keep the colors (they aid the majority of students) but add explicit labels and a textured pattern or contrasting border so the encoding survives in the green-red-confused case.

**Sources:**
- Birch, J. (2012). Worldwide prevalence of red-green color deficiency. *Journal of the Optical Society of America A*. https://pubmed.ncbi.nlm.nih.gov/22472762/
- Colour Blind Awareness UK: https://www.colourblindawareness.org/colour-blindness/
- ColorBrewer: https://colorbrewer2.org/
- Color Oracle (free simulator for Mac/Windows/Linux): https://colororacle.org/

### 4. Tufte on "small effective differences"

In *Envisioning Information* (Graphics Press, 1990) Tufte argues that good design uses small effective differences — minimum visual variation sufficient to encode the distinction the reader needs. Loud color, in this framing, is a failure of design discipline. The instinct to make distinctions *bigger* — louder color, heavier weight, more contrast — usually betrays that the underlying structure isn't being shown clearly enough on its own. Strong design uses muted, well-chosen color and lets the structure do the talking; the color is just the last small differential that tips the eye to the right element.

Applied to slides: if the faculty member is using six saturated colors to distinguish six categories, the categories are probably failing to distinguish themselves through position, size, or label. The color is over-compensating for a structural problem upstream. The fix is rarely "use seven colors." It is usually "fix the structure so two muted colors plus position carry the distinction." This is also the connection back to Chapter 4: wrong visual form (a six-category pie chart) puts the burden on color that the form should carry.

**Common misconception:** "More color = more information." False. The eye discriminates color reliably up to about five to seven categories under ideal conditions and far fewer under projection. Beyond that, color becomes a guessing game. Cleveland & McGill (1984) place "color saturation" near the bottom of their perceptual-accuracy ranking — a high cognitive cost relative to the information delivered.

**Source:** Tufte, E. R. (1990). *Envisioning Information*. Graphics Press. https://www.edwardtufte.com/book/envisioning-information/

### 5. Heer & Stone on color naming and the "this color, that color" problem

Jeffrey Heer and Maureen Stone's 2012 CHI paper, "Color Naming Models for Color Selection, Image Editing and Palette Design," builds a probabilistic model of how humans verbally name colors and uses it to define two operational metrics: color saliency (how reliably a color is named the same thing by different people) and color name distance (whether two colors share a name). The teaching point for the chapter: when you want a reader to compare two marks across slides, they need to be able to remember which is which. If the two colors are different but both fall under "kind of teal," the reader cannot reliably distinguish them at recall. Color choice for instructional purposes is not "which colors look nice together" — it is "which colors will the student be able to *name* and therefore remember."

This connects to Stone's *A Field Guide to Digital Color* (A K Peters, 2003), a more comprehensive treatment of how digital color systems work and where they break down for display purposes. For a slide-design chapter the Heer-Stone paper is the more practically actionable single source.

**Source:** Heer, J. & Stone, M. (2012). Color Naming Models for Color Selection, Image Editing and Palette Design. *CHI '12 Proceedings*. DOI: 10.1145/2207676.2208547. http://vis.stanford.edu/papers/color-naming-models — PDF: http://vis.stanford.edu/files/2012-ColorNameModels-CHI.pdf

---

## B. Domain examples and cases

### Case 1: The "engagement" gradient background (failure case)

A faculty member uses a Canva template with a teal-to-purple gradient background across all slides "for visual interest." Three failures stack. (1) Body text on the gradient passes contrast at the light end and fails at the dark end — the same text is legible on slide 4 and invisible on slide 9. (2) The gradient changes meaning across slides for no reason — extraneous load, in CLT terms. (3) The gradient is decoration, not signal — every reader spends working memory parsing whether the color is encoding something, and is told no. Fix: solid neutral background, contrast-checked once, applied to every slide.

### Case 2: A red-green chart in a public-health course (failure case, accessibility)

A slide showing two outcome groups — "intervention" (green) and "control" (red) — across five time points. The instructor projects in a 200-seat lecture hall. Sixteen of the male students cannot reliably distinguish the two lines. They cannot tell which is the intervention. They are not engaging less; they are receiving an unencoded chart. The instructor never finds out because the failure is invisible to them. Fix: keep the colors (they help the rest) but add explicit labels at the end of each line, vary line style (solid vs. dashed), and run the slide through Color Oracle once before saving the deck. Time cost: under two minutes per chart.

### Case 3: The well-chosen accent (positive case)

A slide titled with one full-sentence assertion — "Working memory holds about four items" — in neutral dark gray on white. One word, "four," is in the brand red. The eye lands on "four" first; the rest of the sentence is the context that frames "four." Color used once. Meaning specific (the numeric claim). Contrast checked (red on white passes 4.5:1). Encoding survives colorblindness because "four" is also the salient word in the sentence. This is what color encoding looks like when it works — one clear job, done with one color, repeatable across the whole deck.

---

## C. Connections and dependencies

**Prerequisites:**
- Chapter 1 (Slideument) and Chapter 3 (Too Much Text): reducing text density makes color choices visible. Color can't signal anything when the slide is wall-to-wall words.
- Chapter 2 (Hierarchy): hierarchy is usually carried by size and weight; color is the third signal, used sparingly. Trying to use color *before* size/weight hierarchy is in place puts too much load on the weakest channel.
- Chapter 4 (Wrong Visual Form): correct form often makes color unnecessary. A clear table needs almost no color. A clear flowchart needs one accent. A messy slide reaches for color to compensate.

**Unlocks:**
- Chapter 6 (Textbook Figure): figure redesign uses color as a signaling overlay — the chapter teaches what signaling does *to* a figure, but Chapter 5 establishes what counts as good color use in the first place.
- Chapter 10 (Headline That Says Nothing): the assertion-evidence structure often uses color in the headline ("four" red, "items" black) — depends on Chapter 5's encoding rules.
- Chapter 11 (Owning Your DESIGN.md): six color variables, each with a role and a contrast ratio documented. The DESIGN.md cannot be defended without Chapter 5's vocabulary.

**Adjacent chapters:** Chapter 5 closes Act One (the slide-level eye is built) and immediately precedes Chapter 6, which uses color as the primary instrument for retrofitting textbook figures. The connection should be made explicit at the chapter close — "now you know what color is for; let's apply it to the hardest case."

---

## D. Current state of the field

**Settled:**
- The Signaling Principle (Mayer) is empirically supported across dozens of studies.
- WCAG 2.1 AA's 4.5:1 ratio is the legal/practical accessibility floor for normal text; this is not contested.
- Red-green color vision deficiency affects ~8% of men in Northern-European-descended populations; not contested.
- Cleveland & McGill's perceptual-task ranking (color saturation near the bottom) is replicated.
- ColorBrewer palettes are colorblind-safe and the de facto standard for cartographic and data-visualization color selection.

**Contested:**
- Whether 7:1 (WCAG AAA) should be the *practical* slide standard, or whether 4.5:1 is sufficient in modern projector environments. Practitioners disagree; the safer recommendation for instructional slides is 7:1 when feasible.
- Whether dark-mode slides (light text on dark background) are more or less legible than light-mode slides in projection. The evidence cuts both ways; consistency within a deck matters more than the choice.
- Whether the Brutalist palette rule (red = brand only, never danger) is the right convention or whether it conflicts with established "red = warning" learned associations. The book takes a position; reasonable designers disagree.

**Key references (3–5):**
1. W3C WCAG 2.1, Understanding 1.4.3 Contrast (Minimum). https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum
2. Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press. (Signaling Principle, ch. 6)
3. Tufte, E. R. (1990). *Envisioning Information*. Graphics Press.
4. Heer, J. & Stone, M. (2012). Color Naming Models for Color Selection. *CHI '12*. http://vis.stanford.edu/papers/color-naming-models
5. ColorBrewer: Brewer, C., Harrower, M., Penn State (2002–). https://colorbrewer2.org/

**Recent developments (last 3 years):** WCAG 2.2 was finalized in October 2023 (current version as of 2026), keeping the 4.5:1 contrast requirement intact and adding new criteria around focus indicators and authentication that don't change slide-design practice. The APCA (Accessible Perceptual Contrast Algorithm) is an experimental successor to the WCAG contrast formula, designed to better reflect human perception of contrast at different sizes and weights; not yet a standard, but worth watching. [verify APCA status in 2026 — believed still draft/non-normative]

---

## E. Teaching considerations

**Where faculty stick:**
- Faculty defaulting to color "for visual interest" without naming what it encodes. The diagnostic question — "what does this color mean?" — is the unstick move. Make the faculty member answer in one word for each color used. If they can't, the color is decoration.
- Faculty distrust of their own taste. Many faculty say "I'm not a designer, I don't know which colors look good together." The chapter should reassure: this is not a taste question. Use ColorBrewer or Brutalist defaults. The taste judgments are made; the faculty member's job is encoding, not selection.
- Resistance to losing color. Faculty often experience the "use less color" rule as flattening, austere, joyless. The chapter should land: muted is not austere. Muted is precise. Color spent everywhere is color spent nowhere.

**Analogies that work:**
- *Color as currency.* You have a small budget of color attention to spend across the deck. Spending it on backgrounds and decorative accents leaves none for the moments when color needs to mean something. A deck that uses color sparingly has color available when it matters.
- *The fire alarm.* If a fire alarm sounded every five minutes, you would stop hearing it. If color is on everything, the eye stops parsing it. The signal needs the silence around it.
- *The brand-color-as-emphasis rule.* The Brutalist convention — red is brand and emphasis, never danger — is one consistent solution; faculty can adopt it or define their own, but the rule "one color, one job" is the principle.

**Exercises:**
- Take a current deck. List every color used. For each color, write the single word it encodes. Cross out any color whose answer is blank or "decoration." That's the cut list.
- Run a slide through Color Oracle (colororacle.org). What information disappears? Anything that disappears was encoded in color alone — that's a failure case to fix.
- Use WebAIM's contrast checker on every text-against-background pairing in a deck. Anything below 4.5:1 fails. Below 3:1 is illegible in projection. Fix list, ranked.
- For one slide, replace all color with grayscale plus one accent. Notice whether the slide is worse, better, or no different. The "no different" outcome is the diagnostic that the original colors were not encoding.

---

## F. Library files relevant to this chapter

- **`lecture-slides-deep-research.md`** — Section "Color for Instructional Contexts" is the direct precursor (contrast ratios, ColorBrewer, blue-orange as safe default). Section "Mayer's 15 Multimedia Learning Principles" — pull the Signaling Principle text. Section "Layout, Grid, and Whitespace" — references signaling as systematic use of cues.
- **`_lib_EdTech.md`** — plausibly relevant for accessibility framings in educational technology context.
- **`_lib_How-to-Deliver-a-TED-Talk.md`** — practitioner-level advice on slide aesthetics; flag for skim.
- **`_lib_Teaching-for-Deeper-Learning.md`** — likely contains signaling/cueing framing for K–12 instructional context; useful if Nik wants a cross-domain example.
- **`_lib_The-Digital-Delusion-Horvath.md`** — Horvath on edtech tools defaulting to decoration; plausibly relevant.
- **`_lib_Thinking-Fast-and-Slow.md`** — Kahneman on visual salience and attention; the "color as attention budget" argument has dual-process backing.
- **`_lib_Surfaces-and-Essences.md`** — possibly less directly relevant; flag plausibly.
- **`_lib_Building-Thinking-Classrooms.md`** — flag plausibly relevant; Liljedahl's framing of attention in classroom design may connect.

## G. Gaps and flags

- FLAG: The "8% of men" figure is reliable for Northern-European-descended populations. Prevalence varies by ethnic background (lower in many East Asian and sub-Saharan African populations). The chapter should cite the figure honestly and add one sentence acknowledging the variation, or phrase as "up to 8%" to remain defensible across populations.
- FLAG: The Brutalist palette rule (red = brand only) is a workshop convention, not a research finding. The chapter must present it as one defensible choice, not as a research-backed prescription. Two reasonable designers can disagree.
- FLAG: WCAG 2.2 superseded WCAG 2.1 in October 2023. TIKTOC.md cites WCAG 2.1; the chapter draft should update to 2.2 (the contrast requirements are unchanged but the version citation should be current). [verify which version Nik prefers — 2.1 was specified, 2.2 is current]
- GAP: No direct empirical study located that compares projection contrast degradation across modern (post-2020) projector technologies. The 7:1 recommendation is practitioner consensus, not a citable measured threshold.
- GAP: One sentence on AI-generated images as a Chapter 5 trigger (per TIKTOC.md Open Question 5) — AI-generated decorative images often have low-contrast text overlays, gradient backgrounds, and arbitrary color schemes that violate every diagnostic in this chapter. The failure is that the image looks polished and the violation is invisible to the untrained eye. The chapter draft should include this in "the feeling."
- GAP: APCA's current status in 2026 [verify] — believed still experimental, not part of WCAG 3 normative spec yet.
