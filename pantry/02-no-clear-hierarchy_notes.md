# Research Notes: Chapter 02 — No Clear Hierarchy

**Source:** TIKTOC.md chapter entry
**Notes file:** 02-no-clear-hierarchy_notes.md
**Corresponding chapter:** chapters/02-no-clear-hierarchy.md (not yet written)
**Generated:** 2026-05-13

---

## Chapter summary (from TIKTOC.md)

**One-line:** The reader learns to name hierarchy failure precisely — which elements are competing, which Gestalt principles are violated, and what a prompt must specify to establish clear visual order.

**The feeling:** A slide where the eye doesn't know where to go first. Everything feels equally important. Or nothing does.

**Cognitive science failure:** Extraneous cognitive load from absent signaling. The student's working memory is spent navigating the slide rather than processing its content. Mayer's Signaling Principle violated.

**Visual design failure:** No implicit grid, no size hierarchy, proximity groupings that don't match semantic groupings. Gestalt principles of proximity and similarity violated.

**Prompt category:** Typography scale + spacing + grouping.

**DESIGN.md variables:** Font size scale, font weight, spacing rhythm, layout grid.

**What two people disagree about:** How aggressive to be with size contrast.

**Bridge:** Once hierarchy is clear, the next question is whether there is too much content at any level of that hierarchy. That is Chapter 3.

---

## A. Conceptual foundations

### Typographic hierarchy — size, weight, position, and the scale

Typographic hierarchy is the system of visual differences that tells the eye which element to read first, second, and last. The dominant variables are size, weight (light/regular/bold/black), case (caps/lowercase), color/value, and position. A working hierarchy uses at most two or three of these at once and uses them consistently — the title is always the same way larger than body text; the emphasis is always the same way bolder than baseline.

Robert Bringhurst's *The Elements of Typographic Style* (1992, 4th ed. 2013) is the canonical treatment. Bringhurst's prescription for hierarchy: choose a modular scale (often based on musical ratios — 1.125, 1.2, 1.25, 1.333, 1.5, 1.618, 2) and stick to it. Random font sizes destroy hierarchy because the reader cannot tell what is structurally important from what is incidentally larger. A scale such as 16pt body / 20pt subhead / 28pt section / 40pt title gives the eye four reliable levels and no ambiguity.

On slides specifically, the size floor is the last-row rule: body text should be 24–28pt minimum so a student in the last row can read it. Title sizes of 36–48pt are typical. If everything sits in a narrow band (24, 28, 30, 32), no hierarchy emerges; the contrast ratio between levels is too small for the eye to read at projection distance.

**Common misconception:** That hierarchy is created by making the title bigger. Hierarchy is created by *contrast between levels*. A 30pt title above 28pt body has no hierarchy. A 44pt title above 24pt body has hierarchy. The ratio matters more than the absolute size.

**Worked example:** A slide titled "Three Causes of the 2008 Financial Crisis" at 32pt followed by three bullets at 28pt is visually one block — the eye reads them as a stack. The same slide with the title at 44pt and bullets at 22pt reads as title-plus-list — the eye finds the title first, then the list.

**Source(s):**
- Bringhurst, R. (2013). *The Elements of Typographic Style* (4th ed.). Hartley & Marks.
- Lupton, E. (2010). *Thinking with Type* (2nd ed.). Princeton Architectural Press. https://thinkingwithtype.com/

### Gestalt principles — proximity, similarity, common region, continuation

The Gestalt principles, formulated by Wertheimer, Koffka, and Köhler in the 1920s and refined by perception researchers since, describe how the visual system groups elements automatically. For slide design, four are load-bearing:

*Proximity:* Elements physically near each other are perceived as belonging together. A slide where related elements are scattered and unrelated elements are adjacent fights the viewer's perception. The standard failure mode: a caption that belongs to figure A sits closer to figure B because the layout software wrapped the text awkwardly.

*Similarity:* Elements that share visual properties (color, size, shape, font) are perceived as belonging to the same category. If three labels are the same blue and one is red, the red one is read as semantically distinct — whether or not the designer intended that.

*Common region:* Elements within the same enclosing boundary (a box, a colored panel, a frame) are read as a group. Common region overrides proximity when they conflict.

*Continuation:* The eye follows lines and curves. Elements aligned along an invisible line are perceived as related. This is why an implicit grid (halves, thirds, quarters) makes slides cohere even when the grid lines are not drawn.

The diagnostic move is to read a slide against these principles in order: are things that belong together close together? Are things that share meaning visually similar? Are groupings reinforced by enclosure or alignment? The failure mode the chapter names is when semantic grouping (what the content means) does not match perceptual grouping (what the eye sees).

**Common misconception:** That whitespace is empty space. Whitespace is the proximity signal — it tells the eye where one group ends and the next begins. Removing whitespace to fit more content destroys grouping.

**Worked example:** A slide with four bullets in a tight stack is read as four items in one group. The same four bullets with the first two paired tightly and the next two paired tightly, separated by extra space, is read as two groups of two — a different semantic claim. Spacing is the claim.

**Source(s):**
- Wertheimer, M. (1923). Untersuchungen zur Lehre von der Gestalt. *Psychologische Forschung*, 4, 301–350.
- Palmer, S.E. (1999). *Vision Science: Photons to Phenomenology*. MIT Press. (Modern synthesis of Gestalt.)
- Lidwell, W., Holden, K., & Butler, J. (2010). *Universal Principles of Design* (rev. ed.). Rockport. (Practitioner reference for Gestalt in design.)

### Mayer's Signaling Principle — visual cues directing attention

Mayer's Signaling Principle states that learners perform better when essential material is highlighted by visual or verbal cues that direct attention to it. The principle is one of the five "reducing extraneous processing" principles in Mayer's framework (alongside Coherence, Redundancy, Spatial Contiguity, Temporal Contiguity).

Signaling devices on slides include: bold weight on a key term, color used semantically (one color = "this is the new concept"), arrows or callout boxes directing the eye, headings that name the structure ahead, and position (top-left for the most important element in a left-to-right reading culture). The principle is established in Mayer's *Multimedia Learning* (2009, 2020) and reviewed meta-analytically by van Gog (2014) in the *Cambridge Handbook of Multimedia Learning*.

Signaling fails in two opposite ways. *Under-signaling*: nothing is emphasized, so the eye finds no point of entry and treats every element as equally important — extraneous load. *Over-signaling*: too many elements are emphasized (bold, colored, boxed), and the signals cancel each other out — "if everything is bold, nothing is bold." A slide with three colors of bold text and two callout boxes signals nothing because the cues compete.

The chapter's diagnostic: every signal on a slide should answer "what is this signal telling me?" If it tells you nothing — if it is decoration, not direction — it is noise.

**Common misconception:** That visual hierarchy and signaling are the same thing. Hierarchy organizes the levels of the slide (title, body, supporting). Signaling directs attention within a level to what matters most. A slide can have a clear hierarchy and still fail at signaling if the most important *body element* is not differentiated from the rest of the body.

**Worked example:** A slide titled "Three Causes of the 2008 Financial Crisis" with three equally-weighted bullets has hierarchy (title > bullets) but no signaling — no cue tells the student which of the three is the load-bearing cause. Bolding the second bullet, or using color on the key term within each bullet, restores the signal.

**Source(s):**
- Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.). Cambridge University Press.
- van Gog, T. (2014). The signaling (or cueing) principle in multimedia learning. In R.E. Mayer (Ed.), *The Cambridge Handbook of Multimedia Learning* (2nd ed., pp. 263–278). Cambridge University Press.

### Visual reading paths — F-pattern and Z-pattern, and what they actually predict

Eye-tracking research from the Nielsen Norman Group (Jakob Nielsen, Kara Pernice) on web reading found that users on text-heavy pages scan in an F-shaped pattern — heavy reading on the first line, lighter reading on the second, then vertical scanning down the left edge. The F-pattern has been over-extended in design folklore to claim every slide is read F-shape. That overgeneralizes. The F-pattern emerges in text-dense scrollable content; slides are different objects.

For slides, the more useful prediction is that without explicit signaling, the eye starts at the top-left in left-to-right reading cultures and follows whichever element has the highest visual weight (largest, boldest, highest contrast). The Z-pattern — top-left to top-right to bottom-left to bottom-right — is a useful rough model for sparse slides with a few elements but is similarly not a universal law. Both patterns are defaults the eye uses *in the absence of clear hierarchy and signaling*; the chapter's move is that good hierarchy overrides default scan patterns.

**Common misconception:** That designing for the F-pattern means placing the most important content at the top-left always. That confuses default scanning behavior with prescription. If the slide has clear signaling, the eye goes where you point it, not where the F-pattern would predict.

**Worked example:** A sparse slide with a single large diagram centered and a one-line caption beneath does not produce F-pattern scanning. The eye lands on the diagram (highest visual weight) and then reads the caption. The hierarchy did the work; the pattern is irrelevant.

**Source(s):**
- Pernice, K. (2017). F-Shaped Pattern of Reading on the Web: Misunderstood, But Still Relevant (Even on Mobile). Nielsen Norman Group. https://www.nngroup.com/articles/f-shaped-pattern-reading-web-content/
- Nielsen, J. (2006). F-Shaped Pattern for Reading Web Content. Nielsen Norman Group. https://www.nngroup.com/articles/f-shaped-pattern-reading-web-content-discovered/

### One idea per slide — the structural rule that makes hierarchy possible

Nancy Duarte (*slide:ology*, 2008) and Garr Reynolds (*Presentation Zen*) converge on "one idea per slide" as the structural rule that makes hierarchy meaningful. If a slide contains two ideas, no hierarchy can rank them — they are coordinate, not hierarchical, and any visual hierarchy you impose lies about the content. The fix is not better hierarchy; it is splitting the slide.

The chapter's diagnostic test (paraphrasing Duarte): "What is the single point of this slide?" If the answer requires "and" or "but," there are two slides hiding in one.

**Common misconception:** That "one idea" means "one word" or "one bullet." Duarte means one *teachable point* — which may require a headline, a diagram, a caption, and a callout to deliver. The unity is conceptual, not minimalist for its own sake.

**Worked example:** A slide titled "Causes and Consequences of the 2008 Crisis" contains two ideas (causes; consequences). Even with the best hierarchy, the slide is ambiguous about which to read first because the structure has two heads. Split into two slides, each with a clear hierarchy.

**Source(s):**
- Duarte, N. (2008). *slide:ology: The Art and Science of Creating Great Presentations*. O'Reilly Media. https://www.duarte.com/books/slideology/
- Reynolds, G. (2019). *Presentation Zen* (3rd ed.). New Riders.

---

## B. Domain examples and cases

### Case 1: The Apple keynote slide (Reynolds' canonical good example)

Reynolds' books and his blog use Steve Jobs' Apple keynote slides as the recurring example of slide hierarchy done well. The slides typically contained a single large image or word with a small caption or attribution, and the eye-path was forced by the asymmetry of visual weight. Jobs' decks were extreme in their sparseness, and Reynolds does not claim every academic deck should look like an Apple keynote — but the slides demonstrate that hierarchy is *visible* when there is real contrast between levels.

The case is useful in the chapter as the high-end of size-contrast aggression; the faculty member's slides will sit between Apple-sparse and textbook-dense, but the principle (visible contrast between levels) holds.

**Source:** Reynolds, G. (2019). *Presentation Zen* (3rd ed.), chapter on design. Multiple Jobs-keynote examples discussed; Reynolds' blog has running commentary at https://www.presentationzen.com/

### Case 2: Tufte's information graphics — hierarchy through density, not size

Edward Tufte's preferred slides (when he uses them at all) are paragraph-dense technical handouts where hierarchy is achieved through typographic detail (small caps, indentation, marginalia) rather than dramatic size contrast. The Tufte case is useful in the chapter as the *other* defensible aesthetic: dense, technical, no large titles, hierarchy through subtle typographic conventions. This is the "two people disagree" zone TIKTOC.md flags — aggressive vs. subtle size contrast, both defensible, the vocabulary for the disagreement is the contrast ratio between levels.

**Source:** Tufte, E.R. (2001). *The Visual Display of Quantitative Information* (2nd ed.). Graphics Press. https://www.edwardtufte.com/

### Failure case: The "academic poster on a slide" — hierarchy collapse from textbook transfer

The most common faculty failure mode is the slide produced by pasting a paragraph or section from a textbook and adding a title. The textbook paragraph already had hierarchy (within the textbook's typography: heading, paragraph, in-line emphasis), but that hierarchy was calibrated for reading at 18 inches in a book. Projected at 20 feet, the in-line emphasis is invisible and the paragraph is a wall. The slide has *imported* hierarchy, not *designed* hierarchy. The eye reads everything as equally important because the original signals — small caps, italic emphasis, indented subpoints — do not scale to projection.

This failure mode is the practical entry point for the chapter: the faculty member did not delete the hierarchy; the medium ate it.

**Source:** This is a synthesis of the lecture-slides-deep-research notes (lines 184–195) and Reynolds' general critique. No single primary source names "hierarchy collapse from textbook transfer" as a term — that's the book's coinage.

---

## C. Connections and dependencies

**Prerequisites (what reader must already know):**
- Chapter 1's distinction between live deck and study artifact (hierarchy choices differ for each).
- The basic Brutalist DESIGN.md variables for font size scale, weight, and spacing.
- That "the slide doesn't feel right" is a real signal worth diagnosing.

**Unlocks (what this chapter makes possible):**
- Diagnostic vocabulary for "what is competing on this slide" — used in Chapter 3 (text density), Chapter 4 (visual form), Chapter 5 (color), Chapter 6 (figures).
- The signaling-principle frame — central to Chapter 5 (semantic color) and Chapter 6 (figure callouts).
- The Gestalt-grouping move — recurs whenever a slide has multiple elements that should/shouldn't be perceived as related.

**Adjacent chapter connections:**
- Chapter 1 (Slideument): Hierarchy can't fix a slideument; the use-case bifurcation comes first. But once you've decided what the deck is for, hierarchy is the first design move.
- Chapter 3 (Too Much Text): Per TIKTOC.md bridge, "Once hierarchy is clear, the next question is whether there is too much content at any level of that hierarchy."
- Chapter 5 (Color): Signaling Principle reappears as semantic-vs-decorative color. Same diagnostic, different variable.
- Chapter 10 (Headline That Says Nothing): Hierarchy is what makes the assertion-headline visible as the load-bearing element.

---

## D. Current state of the field

**Settled:**
- Visual hierarchy reduces extraneous cognitive load — Sweller (1988, 2011), Mayer (2009, 2020). The mechanism is well-understood: the visual system uses hierarchy cues to allocate attention; absent cues, allocation is effortful.
- Gestalt principles describe how the visual system groups elements automatically — Wertheimer (1923) onward, replicated in modern vision science (Palmer, 1999).
- Signaling improves learning when used consistently — van Gog (2014) meta-analysis in the *Cambridge Handbook of Multimedia Learning*.
- The last-row rule (24pt+ body text) is industry standard for classroom projection — Reynolds, Duarte, Kosslyn all converge.

**Contested or emerging:**
- *How aggressive size contrast should be.* The Reynolds/Duarte camp endorses dramatic contrast; the Tufte camp prefers dense, subtle typographic hierarchy. Both are defensible for different audiences. TIKTOC.md flags this as the "what two people disagree about" of the chapter.
- *Whether F-pattern / Z-pattern reading models apply to slides.* The patterns were established for web reading. Extending them to slides is folklore as much as evidence. Nielsen Norman Group itself has walked back the strong version of the F-pattern claim (Pernice, 2017).
- *Whether digital natives have different scanning patterns than older readers.* Sparse empirical evidence; mostly assertion. Avoid in the chapter.

**Key references:**
1. Mayer, R.E. (2020). *Multimedia Learning* (3rd ed.). Cambridge University Press. — Signaling Principle and the cognitive-load frame.
2. Bringhurst, R. (2013). *The Elements of Typographic Style* (4th ed.). — Modular scale and the structural argument for hierarchy.
3. Reynolds, G. (2019). *Presentation Zen* (3rd ed.). — Slide-specific aesthetic with worked examples.
4. Duarte, N. (2008). *slide:ology*. — One-idea-per-slide and the structural prerequisite for hierarchy.
5. Lidwell, W., Holden, K., & Butler, J. (2010). *Universal Principles of Design*. — Practitioner-friendly Gestalt reference.

**Recent developments (last 3 years):**
- AI slide tools default to grid layouts that look hierarchical but use uniform font sizes within levels (e.g., Gamma's default templates). The visual hierarchy is in the *template*, not in the content. When the content varies in importance, the template doesn't adjust. [verify]
- Eye-tracking research on slide viewing specifically (rather than web reading) is sparse. Most empirical work on hierarchy is still extrapolated from print and web studies.
- The Web Content Accessibility Guidelines (WCAG) 2.2 (October 2023) refined contrast requirements; relevant for hierarchy via color but mostly covered in Chapter 5.

---

## E. Teaching considerations

**Where faculty get stuck:**
- *"My title is bigger — isn't that hierarchy?"* The most common stuck point. The faculty member made a title 32pt and body 28pt and believes they have hierarchy. The fix is the contrast-ratio vocabulary: hierarchy lives in the ratio between levels, not the absolute sizes. A 1.14× ratio (32/28) is invisible at projection. A 1.83× ratio (44/24) is unmissable.
- *"But the textbook does it this way."* The textbook's hierarchy works at print size. At projection size, it collapses. This connects to Chapter 6 (textbook figure transfer) but starts here.
- *"If I make the title huge, the slide looks unbalanced."* The faculty member is intuiting that visual weight matters. The fix is to introduce whitespace as the balancing element — a 44pt title with generous whitespace around it does not look unbalanced; a 44pt title crammed against a paragraph does.
- *"Everything on this slide is important."* The diagnostic move is to force ranking: if everything is important, you have not yet decided which is *most* important. The exercise of ranking is the teaching.

**Analogies and framings that work:**
- *Newspaper front page.* The eye knows what the lead story is before reading a word, because of size and position. The slide should pass the same test. (Common in design literature; cited in Reynolds.)
- *Orchestra dynamics.* Hierarchy is not "everyone plays louder" — it is "the melody plays louder than the accompaniment, every time, consistently." (Original framing for the book.)
- *Outline vs. essay.* An outline shows ranks (I, A, 1, a). A slide should show ranks the same way, visually. (Common framing.)

**Exercises that build the target skill:**
- *Before/after pair (the book's standard).* Take a Brutalist-generated content slide with three equally weighted elements. Run the prompt "Establish three levels of typographic hierarchy: title at 44pt, primary message at 28pt, supporting at 20pt. Use proximity to group the primary message with its supporting evidence." Compare.
- Diagnostic questions for any slide:
  1. Where does my eye go first? Is that where it should go?
  2. How many size levels are there? Can I name each one's role?
  3. Are elements that belong together physically close?
  4. Is whitespace grouping the right things?
  5. If I removed all the text and looked only at the shapes, would I still know what the structure was?

---

## F. Library files relevant to this chapter

- `lecture-slides-deep-research.md` — **Primary cross-reference.** Sections on typography rules (lines 136–153), layout and grid (lines 156–164), Mayer's Signaling Principle, and the last-row rule all feed this chapter directly.
- `_lib_EdTech.md` (plausibly) — May contain practitioner discussion of slide layout norms across instructional design programs.
- `_lib_How-to-Deliver-a-TED-Talk.md` (plausibly) — Gallo discusses TED's slide-design guidelines; TED's templates are a defensible hierarchy aesthetic worth referencing.
- `_lib_Teaching-for-Deeper-Learning.md` (plausibly) — Likely covers attention allocation in instruction; useful for the signaling frame.
- `_lib_Surfaces-and-Essences.md` (plausibly) — Hofstadter & Sander on analogy may surface as an analogy generator for the hierarchy-as-structure framing.
- `_lib_Thinking-Fast-and-Slow.md` (plausibly) — Kahneman's System 1 frame: hierarchy works because System 1 perceives it pre-attentively; failed hierarchy forces System 2 to navigate the slide.
- `_lib_Building-Thinking-Classrooms.md` and `_lib_The-Digital-Delusion-Horvath.md` — less directly relevant for Ch 2.

---

## G. Gaps and flags

- FLAG: The Bringhurst modular-scale recommendation (1.125, 1.2, 1.25, 1.333, 1.5, 1.618, 2 — sometimes called the "diatonic" scale or by other names) is widely repeated in design literature but Bringhurst's own treatment is more about the math of scales than a prescriptive list. Confirm against the source before citing specific ratios as "Bringhurst's recommendation."
- FLAG: The F-pattern eye-tracking research is real but has been over-cited in design folklore. Use carefully; the Nielsen Norman Group's own walk-back (Pernice 2017) is important context.
- FLAG: The Apple keynote / Steve Jobs slide examples are well-documented in Reynolds' books but the original slides themselves are Apple property. The chapter can describe them; reproducing them needs care (copyright covered in Appendix B).
- FLAG: There's a difference between the perceptual-grouping Gestalt principles (Wertheimer's original work) and the "design Gestalt" treatment in books like *Universal Principles of Design*. The former is empirical perceptual science; the latter is practitioner translation. The chapter should mostly use the practitioner translation but ground it once in the perceptual science.
- GAP: I do not have a single empirical study measuring the effect of *typographic hierarchy specifically* on slide-based learning outcomes. The Signaling Principle research (van Gog 2014) is general; signaling-via-typography vs. signaling-via-arrows-vs-signaling-via-color is not finely partitioned in the literature I can name. The chapter can rest on the general Signaling Principle without overclaiming a typography-specific empirical result.
- GAP: There's a real question — not addressed in TIKTOC.md — about how hierarchy interacts with the Brutalist system's HTML/D3 output. CSS hierarchy controls (font-size, font-weight, line-height, margin) are precise and inspectable, which is part of the book's argument for the medium. The chapter should probably acknowledge this advantage briefly without making it the point.
