# Chapter 2 — No Clear Hierarchy

> When the eye doesn't know where to land first, the slide has already failed — what is it that makes hierarchy visible, and what destroys it?

---

## 1. The feeling

You open the deck. The first content slide loads. You look at it for a second and you cannot tell what it is asking you to read first.

There is a title at the top. The title is the same weight as the bullets below it. The bullets are slightly smaller — not enough smaller that the eye picks the title out as the entry point. One bullet is purple. Another is green. They are the same size as the regular bullets and you do not know what the color means. There is a callout box on the right. The callout box has its own heading in bold. The bold heading inside the callout is also the same weight as the slide's main title.

The slide is not ugly. The slide is not empty. Everything seems intentional. And yet, when you try to read it, you read it three times and you read it differently each time. Once you start with the bullets, once with the callout, once with the colored words. You have no path through it.

A student in row twelve has it worse. They look at the slide for the half-second you give them and they look at you and they have learned nothing. Not because the content was hard. Because the eye had no entry point.

## 2. The two diagnostic questions

Two questions, every time, in this order.

**From cognitive science:** *Where does the eye land first, and is that the most important thing on the slide?* If you ask a colleague to glance at your slide for one second and tell you what they read, the answer tells you what your visual hierarchy actually says — regardless of what you intended. When the answer doesn't match the priority you'd state in words, the slide's hierarchy is lying about the content.

**From visual design:** *Is the type hierarchy doing visible work, or is the slide using "title bigger than body" as a stand-in for hierarchy?* A 32pt title above 28pt body is not a hierarchy. It is two sizes inside a band the eye reads as one. Visible work means visible contrast — between sizes, between weights, between groupings. If the contrast is at the threshold of perception, the hierarchy is not doing work; it is doing politeness.

## 3. The principle named

Plain language: **a slide has hierarchy when the eye lands on the right thing first and finds the next thing without effort, and when elements that belong together sit together while elements that don't, don't.** Three forces — size, weight, and proximity — do that work. Random changes to any of them break it.

In framework vocabulary, two ideas meet here. From cognitive science: Mayer's Signaling Principle — learners perform better when visual cues direct attention to the load-bearing content, and signaling fails both when nothing is emphasized and when everything is ([Mayer, *Multimedia Learning*, 3rd ed., 2020](https://www.cambridge.org/core/books/multimedia-learning/E64FFFAB9D984ECCFEA38D63A9DAA4E5); [van Gog, 2014, in *The Cambridge Handbook of Multimedia Learning*](https://www.cambridge.org/core/books/cambridge-handbook-of-multimedia-learning/3A0464B788CB7EFD75A04E1F66ABEAB1)). From visual design: the Gestalt principles of proximity and similarity — the perceptual rules, named by Wertheimer in 1923 and confirmed by every vision science textbook since, by which the visual system groups elements automatically based on what is near what, and what looks like what ([Wertheimer, 1923, *Psychologische Forschung*](https://link.springer.com/article/10.1007/BF00410640) `[verify primary URL]`; [Palmer, *Vision Science*, 1999](https://mitpress.mit.edu/9780262161831/vision-science/)). The typographic prescription that operationalizes all of this lives in [Bringhurst, *The Elements of Typographic Style*, 4th ed., 2013](https://www.tug.org/store/hartleymarks/) `[verify URL]`: pick a scale and stay on it.

There is a third name worth knowing because the failure mode you most often produce is the one it predicts: Nancy Duarte's *one idea per slide* rule ([Duarte, *slide:ology*, 2008](https://www.duarte.com/books/slideology/)). If your slide has two ideas, no hierarchy can rank them. They are coordinate, not subordinate. The fix is not better hierarchy. The fix is two slides.

## 4. Bad example

The slide is titled "Three Causes of the 2008 Financial Crisis." Three bullets follow. A callout sits on the right. Here is the markup.

```html
<!-- BAD: hierarchy absent. Everything competes; nothing leads. -->
<section class="slide">
  <h1 style="font-size: 32px; font-weight: 600;">
    Three Causes of the 2008 Financial Crisis
  </h1>
  <!-- Title is 32px / semibold. Body bullets below are 28px / semibold.
       Ratio between levels: 1.14x. Below the threshold of perceptual
       contrast at projection distance — the eye reads this as one block. -->

  <ul style="font-size: 28px; font-weight: 600;">
    <li style="color: #6a1b9a;">Subprime mortgage origination</li>
    <!-- Purple. Why purple? Unknown. The color encodes nothing the slide
         declares. Mayer Signaling violation: a cue is present but the cue
         tells the reader nothing. -->

    <li>Mortgage-backed security leverage</li>
    <!-- The actual load-bearing cause. Looks identical to the other two.
         No size, weight, or color distinguishes it. The eye has no reason
         to read this one as the answer. -->

    <li style="color: #2e7d32;">Credit default swap exposure</li>
    <!-- Green. Again — encoding what? -->
  </ul>

  <aside style="font-size: 24px; font-weight: 700; border: 2px solid;">
    <h2 style="font-size: 26px; font-weight: 800;">Did you know?</h2>
    <p>Lehman Brothers was founded in 1850.</p>
  </aside>
  <!-- Callout box. Its heading is 26px / extra-bold — visually heavier than
       the slide's main title (32px / semibold). The slide has accidentally
       promoted "Did you know?" above the actual subject. Gestalt common-region
       (the box) plus high weight makes the aside compete with the title.
       The 1850 fact is a seductive detail (Ch 3 / Ch 7 territory) but it
       wins the hierarchy fight anyway because the slide handed it the win. -->
</section>
```

Where it fails, in order. The title is 32pt semibold; the bullets are 28pt semibold. Their ratio — roughly 1.14× — sits below the threshold at which the eye reads two sizes as two levels. At projection distance, this is one block, not two. The accent colors (purple, green) appear on two bullets but encode nothing; nothing on the slide tells the reader what purple means or why "MBS leverage" — the actual load-bearing cause — gets no color while the other two do. The signaling is present and meaningless, which is the failure mode van Gog (2014) names as *over-signaling that cancels out*. Worst of all, the callout heading "Did you know?" is in heavier weight than the slide's title. The slide has accidentally told the eye that "did you know" is more important than the slide's subject. Common-region (the box) plus weight wins the hierarchy fight against size alone. The eye lands on a 1850 trivia fact when it should be landing on the three causes the slide names.

The student looking at this for one second leaves with *something about 1850 and Lehman*. They do not leave with the answer to *which of the three causes was load-bearing*. The slide had a hierarchy. It was just the wrong one.

## 5. Good example

Same content. Three forces — size, weight, proximity — used on purpose. One signaling cue used once where it asserts emphasis.

```html
<!-- GOOD: hierarchy visible at a glance. One entry point, clear groupings,
     one purposeful emphasis. -->
<section class="slide">
  <h1 style="font-size: 44px; font-weight: 700;">
    MBS leverage was the load-bearing cause.
  </h1>
  <!-- Assertion headline. 44px / bold. The slide's primary message.
       Ratio against body: 44/22 = 2.0x. Unmissable at projection distance.
       Tells the student WHICH cause to focus on, not just that there were
       three. (Headline assertion: foreshadow of Chapter 10.) -->

  <p style="font-size: 22px; font-weight: 400; margin-top: 24px;">
    Three causes of the 2008 financial crisis:
  </p>

  <ul style="font-size: 22px; font-weight: 400; margin: 12px 0 12px 0;">
    <li>Subprime mortgage origination</li>
    <li style="font-weight: 700; color: #c0392b;">
      Mortgage-backed security leverage
    </li>
    <!-- One emphasis. Bold + accent color, used once on the slide,
       on the cause the headline names as load-bearing. The color is
       not decorative — it encodes "this is the one." Signaling
       Principle satisfied, because the cue answers a question the
       slide actually asks. -->
    <li>Credit default swap exposure</li>
  </ul>
  <!-- All three bullets at 22px / regular. They sit as a group (proximity).
       The bolded second item stands out because it is the ONLY emphasis
       on the slide. If all three were styled differently, none would. -->

  <div class="notes">
    Subprime origination expanded the borrower pool; CDS exposure
    amplified counterparty risk. Both were structurally important.
    But the leverage stack on MBS — Levin-Coburn senate report puts
    typical investment bank leverage at ~30:1 entering 2008 —
    converted a containable mortgage delinquency into a systemic
    collapse. That is the claim of this slide.
  </div>
  <!-- Notes field carries the supporting argument so the live slide can
       remain a hierarchy of size, weight, and one color. -->
</section>
```

What changed: the title became an assertion ("MBS leverage was the load-bearing cause") instead of a label ("Three Causes of the 2008 Financial Crisis"). The size ratio between title and body went from 1.14× to 2.0×, which is the difference between *technically larger* and *visibly larger*. The accent color appears once, on the bullet the headline names — color now encodes meaning ("this is the load-bearing one") rather than decorating arbitrarily. The callout box is gone; the trivia is in the notes if it's anywhere. Proximity does the grouping work: the three bullets sit together as a list; the headline sits apart as a claim.

Now the one-second test passes. Glance at the slide. You read *MBS leverage was the load-bearing cause* first. You see *three bullets, the middle one emphasized*. You know what to focus on before the speaker says a word. The hierarchy is doing the speaker's pointing for them.

Here is the trick worth naming. The biggest move was not making the title bigger. It was deciding **what the title was for**. Once the title became a claim, the question *which element of the body matters most* had an answer (the bullet the claim names), and the question *what should the accent color encode* had an answer (the bullet the claim names). The visual hierarchy fell out of the rhetorical hierarchy. Hierarchy in type is just the rhetorical structure made visible at the speed of perception.

## 6. The prompt

Paste this into the Brutalist system. Adapt the system name for any AI slide tool.

```
Restructure this slide so the visual hierarchy is unmistakable at a
glance. Requirements:

1. The headline is the entry point. Set it at 44pt bold (or whatever
   produces at least a 2.0x size ratio against body text). Rewrite the
   headline as a full-sentence claim if it is currently a topic label.

2. Body text sits at one weight lighter than the headline (regular,
   not bold) and at body size from DESIGN.md. There should be exactly
   two type sizes on this slide: headline and body. Reject any
   intermediate sizes.

3. Accent color appears at most twice on the slide and only on elements
   the headline's claim points to. If you cannot state in one phrase
   what the accent color encodes on this slide, remove the color.

4. Group elements by proximity. Things that belong together sit
   together with tight spacing; groups are separated by visible
   whitespace at least 1.5x the line-height between groups.

5. Move any callout box, sidebar, or "did you know" element to the
   notes field unless the headline's claim explicitly depends on it.

Return the slide as Brutalist HTML with the .slide and .notes structure
preserved.
```

The second requirement is the one most often resisted: "but I need three sizes for nuance." Three sizes is fine when each size does identifiable work. Three sizes that the eye reads as one band of sizes is two sizes too many. Reject intermediate sizes until each level earns its own meaning.

## 7. The DESIGN.md change

Two variables. One sentence each.

```
type_scale: [44, 22]              # was: [32, 30, 28, 26, 24]
accent_color_uses_per_slide: 2    # was: unlimited
```
`[verify variable naming against Brutalist DESIGN.md conventions. If your
system exposes typography_scale as a modular ratio (e.g., 1.5x or 1.618x)
rather than an explicit array, set the ratio to >= 1.5 and document the
two-level rule in a comment.]`

Why the type scale: a small set of well-spaced sizes forces every element to declare which level it belongs to, which makes contradictions visible. Why the accent cap: scarcity is what makes emphasis emphatic — if accent color can appear five times, none of those five appearances asserts anything.

A 1.5× ratio between levels (e.g., 22pt / 33pt / 44pt) is the floor at projection distance — anything subtler reads as one band. A 2.0× ratio is the safe default. Bringhurst's modular scales (1.125, 1.2, 1.25, 1.333, 1.5, 1.618, 2) are useful here as anchors `[verify Bringhurst's specific list; the principle of a modular scale is his, the exact ratios are widely repeated and worth checking against the 4th edition].`

## 8. The diagnostic questions to keep

Run any slide through these. They take ten seconds and they catch hierarchy failure before the slide ships.

1. **One-second test: where did my eye land?** If it didn't land on the most important element, the hierarchy is wrong. Not subtle — wrong.
2. **How many type sizes are on this slide, and can I name what each one is for?** If the answer is more than three sizes, or you cannot name a job for each, you have an accidental scale.
3. **What does the accent color encode on this slide?** If you cannot answer in one phrase ("the load-bearing cause," "the new term," "the warning"), the color is decoration and should come off.
4. **Are elements that belong together physically close, and are unrelated elements separated by visible whitespace?** Proximity is making a claim. Make sure it is the claim you want.
5. **If I removed all the text and looked only at the shapes, would I still see the structure?** Hierarchy that survives this test is doing visible work. Hierarchy that doesn't survive is hierarchy by label only.

## 9. What two people might disagree about

Two designers can read this chapter, agree on the diagnosis, and disagree honestly on how aggressive to be with the cure.

**The maximalist-versus-minimalist split.** One camp — closer to Reynolds and the [TED slide aesthetic](https://www.ted.com/about/our-organization/our-policies-terms/ted-talks-presentation-design-rules) `[verify URL]` — argues for dramatic size contrast (3×+ ratios, one or two type weights, generous whitespace) on the grounds that hierarchy invisible to the back row is hierarchy that didn't happen. Reynolds' worked examples in [*Presentation Zen*](https://www.presentationzen.com/) routinely run a single large element against tiny supporting text. The other camp — closer to Tufte — accepts subtler typographic hierarchy (1.5× ratios, multiple weights, small caps, indentation as a hierarchy cue) on the grounds that dense, technical content cannot be flattened to keynote sparseness without lying about the structure ([Tufte, *The Visual Display of Quantitative Information*, 2nd ed., 2001](https://www.edwardtufte.com/)). Both are defensible. Reynolds-style works for talks; Tufte-style works for technical documents projected.

The vocabulary the disagreement needs in order to be productive: *what is the contrast ratio between levels on this slide?* Not *do I like it more subtle?* If one designer's slides run 1.5× and another's run 2.5×, both can defend the choice — but they are now arguing about a number, not an aesthetic. The Brutalist convention this book leans toward (2.0× as the default) is closer to Reynolds because the audience is the live-lecture room, not the technical journal page.

**The "designed system" versus "tight system" disagreement.** A "designed system" uses multiple weights and intermediate sizes on purpose — light for captions, regular for body, semibold for sub-emphasis, bold for headline, black for the single most-emphatic word. Done with discipline, this reads as elegant. A "tight system" uses two weights and two sizes, full stop, on the grounds that more controls produce more chances to use them inconsistently. Both can produce hierarchy that works. The vocabulary: *how many levels does this slide actually need?* Most slides need two. Decks that need more should declare the system once and apply it consistently — including the "designed system" decks, which fail not from having four weights but from using four weights inconsistently across slides.

Once hierarchy is clear, the next question is whether there is too much content at any level of that hierarchy. That is Chapter 3.

---

**What would change my mind:** A controlled study showing that subtle typographic hierarchy (1.2× ratios, multiple weights) produces equivalent or better recall and comprehension to dramatic hierarchy (2×+ ratios, two weights) for projected lecture slides in actual classroom conditions. The literature I can name supports the Signaling Principle generally but does not finely partition by hierarchy-aggression. If a study lands on the subtle-hierarchy side, this chapter's default ratio should be revised downward.

**Still puzzling:** I do not have a clean rule for when an "intermediate" type size earns its place. Two sizes plus careful weight variation is enough for almost every slide I have seen. The case for a third size — a sub-headline, a caption tier — is intuitively real but the empirical work isolating its value is, to my reading, thin.

**Tags:** typographic-hierarchy, Mayer-signaling, Gestalt-proximity, Bringhurst-modular-scale, contrast-ratio
