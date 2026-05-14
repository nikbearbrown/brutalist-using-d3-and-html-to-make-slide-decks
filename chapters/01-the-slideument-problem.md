# Chapter 1 — The Slideument Problem

> Is this deck a speaker's anchor or an audience's document — and what happens when it tries to be both?

---

## 1. The feeling

You finish the deck at 11 p.m. the night before lecture. Every slide is full sentences. Every claim is explained. Every reference is on the slide. The deck looks complete.

The next morning you lecture from it. You read the slide. Then you say roughly what the slide says. The students read along while you talk. Halfway through you notice them not looking at you. They are looking at the screen. So are you.

Two weeks later, a student emails: *I missed lecture three — can I just study from the slides?* You look at the slide for lecture three. You realize that without you in the room saying the connective tissue out loud, the slide is a stack of half-sentences and bullets that point at an explanation you didn't write down. You tell the student to read the textbook chapter instead.

Something failed at both ends. The slide was too dense to lecture from. It was too sparse to study from. It looked complete and was useless twice.

That feeling has a name.

## 2. The two diagnostic questions

Ask both, in this order, every time.

**From cognitive science:** *Is the verbal channel doing two jobs at once?* When the slide carries the same sentence you are saying out loud, your audience's working memory has to suppress one stream to follow the other. Usually they suppress you. You become the radio playing while they read.

**From visual design:** *Does this slide know what it's for — a speaker's anchor or an audience's document?* A slide can serve either. It cannot serve both without compromising both. A slide built to anchor your speaking is too sparse to read alone. A slide built to be readable alone is too dense to anchor speaking. If you have not decided which job this slide has, you have already lost the design fight.

## 3. The principle named

Plain language first: **when the slide says what you are saying, your students stop listening.** And: **a slide that tries to be a handout and a speaker's prompt at the same time fails at both.**

In framework vocabulary, those are two named ideas. The first is Mayer's Redundancy Principle — identical narration and on-screen text degrade learning, because both compete for the same verbal-channel bandwidth in working memory ([Mayer & Johnson, 2008](https://doi.org/10.1037/0022-0663.100.2.380); [Mayer, *Multimedia Learning*, 3rd ed., 2020](https://www.cambridge.org/core/books/multimedia-learning/E64FFFAB9D984ECCFEA38D63A9DAA4E5)). The second is Garr Reynolds' *slideument* — his contraction of "slide" and "document," named in [a 2005 Presentation Zen post](https://www.presentationzen.com/presentationzen/2005/09/the_slideument_.html) and developed across [*Presentation Zen*](https://www.presentationzen.com/) (Reynolds, 2008; 3rd ed. 2019) `[verify 2005 post URL resolves]`.

The two failures arrive together. Redundancy is the cognitive mechanism. Slideument is the structural cause. The slide is dense because the author hasn't decided what the slide is for, and the density violates Mayer's principle the moment you open your mouth.

This is the chapter's central claim: **the slideument is not the wordy slide. It is the slide whose author hasn't decided whose attention it is asking for, mine or my listeners'.** A 90-word slide delivered as a handout (no narration competing) is not a slideument. A 30-word slide whose 30 words are exactly what the speaker says is.

## 4. Bad example

Here is the slide the AI tool produced when you asked Gamma to make a deck on cellular respiration. The slide is the second one in the deck.

```html
<!-- BAD: slideument configuration. Title is a topic, not a claim.
     Body is a complete-sounding paragraph the speaker will also deliver verbatim.
     There is nothing for the speaker to *add*. The slide IS the lecture. -->
<section class="slide">
  <h1>Oxidative Phosphorylation</h1>
  <!-- Title is a label, not an assertion. Tells the student what the slide is "about"
       but hands them no claim to remember. -->

  <p>
    Oxidative phosphorylation is the metabolic pathway in which the
    mitochondrion uses enzymes to oxidize nutrients, thereby releasing
    chemical energy used to produce adenosine triphosphate (ATP).
    The proton gradient established across the inner mitochondrial
    membrane drives ATP synthase, generating approximately 32 ATP per
    glucose molecule. This process, discovered by Peter Mitchell in
    1961 (Nobel Prize, 1978), accounts for the majority of ATP
    produced during aerobic respiration in eukaryotic cells.
  </p>
  <!-- 87 words. Reading time: ~25 seconds.
       Problem 1 (Redundancy): the speaker is going to deliver these exact ideas
       in roughly these exact words. The verbal channel collides with itself.
       Problem 2 (Slideument): if a student studies from this slide alone two
       weeks later, the Peter Mitchell aside is half the slide and the
       structural fact (proton gradient → ATP synthase → ~32 ATP) is buried
       inside the prose. The structural claim is not visually load-bearing.
       Problem 3: the slide commits to neither use case. -->

  <div class="notes" style="display:none">
    <!-- empty -->
  </div>
  <!-- The notes field — the deck's second product — is empty. The slide is
       trying to do both jobs, and the field that exists to relieve it has
       nothing in it. -->
</section>
```

Here is what fails, point by point. The title is a topic label ("Oxidative Phosphorylation") rather than an assertion. The body is the explanation the speaker will deliver out loud, which violates redundancy the moment the lecture starts. Mitchell-1961 is a seductive detail riding along inside the prose where it cannot be cut without rewriting the paragraph. The notes field is empty, so the slide is forced to be both the speaker's prompt and the student's study text, and it is bad at both. A student studying from this slide gets a wall of prose with no structure. A student attending the lecture gets the wall plus an audio track of you saying the same thing.

The slide looks complete. That is the trap. Completeness is what slideument-style decks optimize for, because completeness is what the author can verify at midnight from their own desk. Pedagogical usefulness is harder to feel from there.

## 5. Good example

Same content. Two artifacts living in one file.

```html
<!-- GOOD: live-deck slide. The slide anchors the claim and the visual.
     The notes field carries the explanation. One source, two products. -->
<section class="slide">
  <h1>The proton gradient powers ATP synthase.</h1>
  <!-- Full-sentence assertion headline. Student leaves the slide with
       a *claim* in their head, not just a topic. -->

  <figure class="diagram">
    <!-- D3-rendered diagram of the inner mitochondrial membrane:
         H+ ions on one side, ATP synthase as a labeled rotor,
         arrow showing H+ flow, output labeled "ATP". -->
    <figcaption>~32 ATP per glucose</figcaption>
  </figure>
  <!-- Slide body is a diagram + one number. The visual channel carries the
       mechanism; the verbal channel (the speaker) carries the explanation;
       the two channels run in parallel rather than colliding. -->

  <div class="notes">
    Oxidative phosphorylation is the metabolic pathway in which the
    mitochondrion uses the proton gradient across the inner membrane to
    drive ATP synthase, generating ~32 ATP per glucose. The pathway was
    elaborated by Peter Mitchell (chemiosmosis, 1961; Nobel Prize 1978).
    For async study: this is the step in aerobic respiration where the
    bulk of ATP is produced.
  </div>
  <!-- Notes field carries the prose. Exported with the slide, the student
       who missed class gets the full explanation. During live delivery,
       only the speaker sees it. The deck is now two products, not a hybrid. -->
</section>
```

What changed: the title became a claim, not a label. The prose left the slide and moved to the notes field, where it serves study without competing with narration. A diagram replaced the paragraph, which lets the visual channel do work the verbal channel was doing alone. The Mitchell aside is in the notes — recoverable for a curious student, removed from the live-delivery competition.

Now the slide *anchors* the lecture. You can talk for ninety seconds about the diagram, the proton gradient, the ATP-per-glucose figure, why this is the high-yield step compared to glycolysis. The slide says *the proton gradient powers ATP synthase* and then gets out of your way. You are not competing with your own slide for the room's attention.

The structural move is the one Reynolds names: stop trying to ship one artifact for two jobs. The Brutalist convention — empty slide body, populated notes field — is the cheap version of his two-artifact prescription. The slide is the live deck. The slide-plus-notes export is the study artifact. Same source file. Different products.

## 6. The prompt

Paste this into the Brutalist system. The principle is portable to any AI slide tool — only the system name changes.

```
Rewrite this slide as a live-deck slide. Requirements:

1. The headline asserts the slide's claim in <= 10 words.
   It is a full sentence, not a topic label.

2. The slide body contains at most one visual element (diagram, labeled
   image, chart, or short equation) and no prose paragraph. No more than
   60 characters of text on the slide body, excluding the diagram labels.

3. Move the full explanation — every sentence I would say aloud — into
   the notes field. Expand the notes field so a student reading the slide
   without me present gets a complete explanation.

4. Identify any "interesting but not essential" details (dates of
   discovery, named researchers, asides) and either remove them or move
   them to the end of the notes field under "Background."

Return the slide as Brutalist HTML with the .slide and .notes structure
preserved.
```

Two things to notice about this prompt. First, it specifies *what each region of the slide is for*, not just "less text." That is the move that prevents the next generation of slideument from arriving the moment you say "shorter." Second, it identifies the seductive detail by name as a category to relocate, which forecloses the "but it's interesting" defense before it has somewhere to hide.

## 7. The DESIGN.md change

Update one variable. One sentence on why.

```
body_text_density_max: 60_chars   # was: unlimited
```
`[verify variable naming against Brutalist DESIGN.md conventions — if the
system already uses a different name for slide body density, substitute it
here. The principle is the cap, not the variable name.]`

Why: a hard cap on slide-body text forces the question *what is this slide for* to be answered before the slide can render. The notes field absorbs whatever the cap excludes, which converts the slideument's failure mode into the two-artifact solution by default.

If your Brutalist DESIGN.md already exposes a `slide_density` or `body_max_words` variable, set it to the equivalent of roughly 10 words / 60 characters and document the rationale in a comment. The number is not sacred; the cap is.

## 8. The diagnostic questions to keep

Run any slide through these. If any answer is *I don't know* or *both*, you have a slideument.

1. **Who is this slide for, right now — me or the audience?** Live-deck slides serve the speaker's anchor function. Async-study slides serve the document function. One slide, one job.
2. **If I removed the speaker from the room, would this slide alone teach the content?** If yes, it is a study artifact and is probably too dense to lecture from. If no, the notes field needs to carry what the slide can't.
3. **If I removed the slide and lectured from blank screen, would the lecture still teach the content?** If yes, the slide is decoration. If no, the slide is doing work — but is the work it does competing with my words or complementing them?
4. **Is anything on this slide a sentence I am about to say out loud?** If yes, cut it from the slide and move it to the notes field. Verbal-channel collision is a real cost, not an aesthetic preference.
5. **Does the notes field contain what the slide can't?** An empty notes field on a sparse slide is half a deck.

## 9. What two people might disagree about

Two faculty members can read this chapter and arrive at honest, defensible disagreements. Naming where matters more than picking a side.

**The crutch-versus-anchor split.** Some lecturers prepare by typing every sentence they intend to say into the slide. The slide becomes a teleprompter. They argue: *I lecture better when the words are in front of me. My students get the benefit of the full content. The deck is also their study aid.* Other lecturers treat the slide as an anchor for an explanation they hold in their head and deliver to the room. They argue: *the slide is where the audience looks; the explanation is what I bring; if I read the slide I am redundant with myself.*

Both are real positions held by working teachers. They produce different decks. The vocabulary that lets them argue precisely instead of past each other: **speaker's deck** (low text, high visual dominance, notes field carries explanation) vs. **audience's deck** (high text density, slide carries explanation, notes field may be empty). Neither is wrong as a *use case*. What is wrong is producing one deck and using it as both. The slideument is the hybrid neither camp endorses on reflection.

**The notes-field-is-enough question.** Reynolds endorses the populated notes field as the practical solution to the two-artifact problem. Tufte argues only a separate technical document — a proper handout, not slide notes — does the job, and points to [the Columbia accident slides analyzed in *The Cognitive Style of PowerPoint*](https://www.edwardtufte.com/tufte/powerpoint) as evidence of what happens when handout-density information is forced into slide format ([Columbia Accident Investigation Board, *Report Volume 1*, 2003, ch. 6](https://www.nasa.gov/columbia/home/CAIB_Vol1.html)) `[verify Tufte page range; common citations point to roughly pp. 8–12 of the 2nd ed.]`. Both are defensible. This book takes the notes-field path as default because the Brutalist system makes it cheap; the two-artifact path is the fallback when the notes field is not where students will actually look.

The disagreement vocabulary: *what specifically goes in the notes field, and will students read it?* Answer those, and the choice between Reynolds' and Tufte's prescription resolves itself for your specific class.

A slide can have too much text for a different reason than slideument failure — sometimes the hierarchy just isn't clear enough to show the reader what matters. That's Chapter 2.

---

**What would change my mind:** A controlled study of AI-generated decks measured against Mayer's Redundancy Principle in actual lectures, finding that the slideument configuration does *not* degrade learning compared to the sparse-slide-plus-notes configuration when speakers are matched. I am not aware of such a study; if one arrives, this chapter's prescription weakens.

**Still puzzling:** I do not have a clean rule for how much explanation a notes field needs to carry to substitute for a textbook chapter. Practitioner consensus says "enough that the student who missed class can follow the argument," which is qualitative. A density target for the notes field — words per slide, or a heuristic about which sentences must appear — is still missing from the literature I can name.

**Tags:** slideument, Reynolds, Mayer, redundancy-principle, live-deck-vs-study-artifact
