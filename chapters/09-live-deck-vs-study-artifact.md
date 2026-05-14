# Chapter 9 — Live Deck vs. Study Artifact

> Is this deck a visual anchor for your spoken explanation, or is it the self-contained explanation itself — and could a student make sense of it without you?

---

## 1. The feeling

You teach the same statistics class twice: once live, once recorded for the async section. You make one deck and use it for both, because the content is the same and you're a working faculty member with a finite week.

The live section glazes over by minute twenty. The slides are dense with full sentences. You find yourself reading them aloud or, worse, paraphrasing what's already on the screen while the students read instead of listening. Halfway through the hour, the back row is on their phones. You are competing with your own slides for the room's attention, and the slides are winning.

You watch the recording for the async section a week later. Now the slides feel sparse. The student watching at home has the slides plus your voice, but the slides themselves don't carry the explanation — you do — and when the student tries to pause and study a single slide, there's nothing to study. They write in the course evaluation: *the slides don't make sense without the lecture*.

Then a third group: the students who attended live and then went back to the slides to review for the midterm. They report the opposite complaint: *the slides have everything on them but I can't tell what mattered*. The same artifact that was too dense for live use was, three weeks later, too sparse to study from. Or it was too dense for the moment of study but not detailed enough to substitute for the lecture they'd half-attended. Whichever direction the complaint runs, the artifact is failing the use case.

You made one deck for two products. It is bad at being either. This is the slideument problem from Chapter 1, scaled to the deck.

## 2. The two diagnostic questions

Ask both. Before the deck starts. Not after.

**From cognitive science:** *Is this deck the visual anchor for spoken explanation, or the self-contained explanation itself?* The cognitive science version is Mayer's Modality Principle ([Mayer, *Multimedia Learning*, 3rd ed., 2020](https://www.cambridge.org/core/books/multimedia-learning/E64FFFAB9D984ECCFEA38D63A9DAA4E5)): people learn more deeply from pictures plus spoken words than from pictures plus printed words, because spoken narration uses the verbal channel of working memory while visuals use the visual channel — two parallel channels, no bottleneck. When the slide shows text *and* the speaker reads it, both inputs land in the verbal channel and compete. Working memory chokes.

The principle's force is asymmetric across the live/async distinction. In live delivery, you have a narrator: the verbal channel is occupied by speech and the visual channel can carry images cleanly. On-screen text becomes redundant. In async delivery without a narrator, the verbal channel is silent: the slide *must* carry text, because nothing else carries the verbal content. The same design move that respects modality in one mode violates it in the other.

**From visual design:** *Could a student make sense of this without me?* The question is mechanical and ruthless. Imagine the student finds the slide three weeks from now, after they've forgotten the lecture, and the slide is the only artifact available. Can they reconstruct what the slide was teaching? If yes, the slide is a study artifact. If no, the slide is a live-deck anchor that needs a speaker. Both are legitimate. Neither is both. The mistake is not knowing which one you made.

The two questions converge: the cognitive-science question asks *which channels are available*, and the visual-design question asks *which artifact is being made*. Live delivery has both verbal and visual channels available; the slide can be sparse because the speaker fills the verbal channel. Async delivery has only the visual channel; the slide must carry the verbal content as on-screen text. The two use cases impose *opposite design constraints* because they have different audio channels available. A single deck cannot satisfy both.

## 3. The principle named

Plain language first: **one deck cannot be both a live anchor and a study artifact.** Either it is sparse — image-led, headline-only, designed to support spoken explanation — or it is annotated — sentence-headlines, full prose explanations, designed to stand alone. The features that make a slide good for live use are the features that make it bad for async use, and vice versa. Trying to do both produces a *slideument*: the deck that fails at both.

In framework vocabulary, this is the deck-level expression of three converging findings from multimedia learning research.

The first is **Mayer's Modality Principle**. Mayer reviews seventeen experimental tests in *Multimedia Learning* and consistently finds that pictures-plus-narration outperforms pictures-plus-on-screen-text on transfer measures, *under the boundary conditions of live, novel, fast-paced, instructor-paced instruction*. The boundary conditions matter. Mayer specifies that the modality advantage *weakens or disappears* when the text is long and technical, when the learner is non-native, when the material is paced by the learner (async), or when the content is highly familiar. Those boundary conditions describe study material almost exactly. The principle is most powerful for live use. Study use is where it fades.

The second is **Mayer's Redundancy Principle**, which goes further: do not narrate the same words shown on screen. When the speaker reads the bullets aloud while the audience reads the bullets silently, both verbal-channel and visual-channel processing collide on the same content twice. Learning is worse than either narration alone or silent reading alone. The slideument failure mode is structurally a redundancy failure: the deck is text-dense (because the author wanted it to stand alone) and is also being narrated by a speaker (because the author also wanted it to be used live). The two design choices, made out of separate worries, cancel each other out in the moment of use.

The third is **Atkinson's assertion-evidence structure** from *Beyond Bullet Points* ([Atkinson, 2005; 4th ed. 2018, Microsoft Press](https://www.beyondbulletpoints.com/)), empirically tested by [Garner & Alley (2013)](https://www.ijee.ie/) in engineering education. The assertion-evidence slide has a full-sentence assertion as the headline and a visual evidence as the body. Across multiple studies, this structure outperforms traditional topic-header-plus-bullets on retention. *In live use.* The assertion-evidence structure assumes a speaker; without one, the headline-plus-visual is a claim plus a graph with no machinery for understanding why the claim follows from the graph. The Chapter 10 chapter unpacks the assertion-evidence move at the slide level. Here, the relevant generalization is that the live-deck design philosophy *bakes in the speaker* and cannot survive the speaker's absence without redesign.

Add one more strand. [Means et al. (2010)](https://www.ed.gov/media/document/evaluation-of-evidence-based-practices-online-learning-meta-analysis-and-review-of-online-learning-studies-revised-september-2010-107159.pdf), in a U.S. Department of Education meta-analysis of 99 studies comparing online and face-to-face learning, found that online learning produced modest gains over F2F on average and blended learning produced the largest gains. The headline is debated and depends on what is being compared. The narrower takeaway, which is what matters for the chapter, is that *async learning can be effective when materials are designed for the absence of the speaker.* Sparse live decks repurposed as async study materials are not async materials. They are live materials with the speaker removed, and they fail predictably.

The Brutalist move is to refuse the slideument compromise. Either accept the live constraint (sparse, image-led, speaker carries the explanation, notes field populated with full speaker script) or accept the study constraint (dense, sentence-headlines, slide carries the explanation, embedded retrieval prompts). When the same content needs both, *produce two artifacts from one source* — same `lecture-04.md` source, two builds with different `deck_mode` flags. Not a hybrid. Two specialist artifacts.

## 4. Bad example

The bad example is one slide rendered as a slideument: dense enough to read, sparse enough that the lecturer is still talking over it. Succeeding at neither.

```html
<!-- BAD: slideument. The slide tries to be self-contained AND speakerable.
     It is text-heavy (because the author wants it to stand alone for study)
     and is also being narrated (because the author is using it in live
     lecture). Mayer's Redundancy violated by definition. Modality violated
     because text-on-screen-plus-narration overloads both channels at once. -->
<section class="slide">
  <h1>The Central Limit Theorem</h1>
  <!-- Topic label, not a claim. The slide is "about" the CLT.
       Neither a live anchor (which would assert what the CLT does)
       nor a study artifact (which would explain what the CLT does). -->

  <ul>
    <li>The CLT states that the sampling distribution of the sample
        mean approaches a normal distribution as sample size grows.</li>
    <li>This holds regardless of the shape of the underlying population
        distribution, provided the population has finite variance.</li>
    <li>The mean of the sampling distribution equals the population
        mean μ.</li>
    <li>The standard deviation of the sampling distribution (the
        "standard error") equals σ/√n, where σ is the population
        standard deviation and n is the sample size.</li>
    <li>The convergence to normality is faster for symmetric population
        distributions; for highly skewed populations, sample sizes of
        n > 30 are typically required.</li>
  </ul>
  <!-- Five bullets, ~75 words. Reading time: ~22 seconds.
       Problem 1 (Modality): all 75 words land in the visual channel
       as on-screen text, while the speaker is simultaneously
       narrating roughly the same content into the verbal channel.
       Both channels carry the same load. Redundancy.
       Problem 2 (Live failure): a student trying to listen to the
       speaker is also trying to read the bullets and is losing both.
       Problem 3 (Study failure): a student looking at this slide
       three weeks later sees five disconnected statements with no
       worked example, no diagram of the sampling distribution
       narrowing as n grows, no derivation, and no opportunity to
       attempt the idea. It "stands alone" in the sense that the
       words are present. It does not stand alone in the sense that
       the words explain. -->

  <div class="notes" style="display:none">
    <!-- empty -->
  </div>
  <!-- The notes field — the channel that would solve half the
       problem — is empty. -->
</section>
```

The failure is structural. The bullets are written to be readable on their own — that's the study-artifact pull — and the speaker is also delivering the same content in the live moment — that's the live-anchor pull. Both pulls are met halfway. The slide is too dense for the speaker (audience reads instead of listens) and too sparse to study from (no derivation, no diagram, no worked example, no retrieval prompt). The instructor at the front of the room senses something is off but cannot name it, because the slide individually looks fine. The slide is failing not as a slide but as a slideument — failing in the way slides fail when they have not been told which artifact they are.

## 5. Good example

Two outputs from one source. Same content. Two artifacts. Side by side.

**Source markdown (`lecture-04-clt.md`):** The content lives once, in a structured source file. Both builds read from it.

```markdown
# Slide: Central Limit Theorem

## Assertion
The sampling distribution of the mean narrows toward normality
as n grows, no matter what shape the population has.

## Visual
sampling-distribution-narrowing.svg
[D3-rendered animation: skewed source distribution at top;
sampling distributions for n=2, n=10, n=30, n=100 below;
each progressively narrower and more bell-shaped.]

## Speaker script (notes field)
The CLT is the reason inference works. Start with any population —
exponential, uniform, weirdly bimodal — and draw samples of size
n. Compute each sample's mean. Plot the distribution of those
means. As n grows, the distribution of means narrows and becomes
normal, regardless of the original shape. The narrowing follows
σ/√n. So to halve the standard error, you need four times as
many samples. The CLT is the bridge from "any distribution"
to "inference using the normal." It's why we can use t-tests
and confidence intervals on data we haven't proven is normal.

## Study explanation
Take any population distribution — call it P. Draw N independent
samples of size n from P. Compute the mean of each sample;
this gives N sample means. Plot the distribution of these N
sample means: this is the sampling distribution of the mean
for sample size n. The CLT states two things about this
sampling distribution: (1) its mean equals μ, the mean of P;
(2) its standard deviation equals σ/√n, where σ is the standard
deviation of P. As n grows, σ/√n shrinks — the sampling
distribution narrows — and the distribution's shape approaches
normality regardless of the shape of P. This is why inference
methods that assume normality (t-tests, z-tests, confidence
intervals) work for any underlying distribution, provided n is
large enough.

## Retrieval prompt
A population has σ = 20. You currently sample n = 100 and
observe a standard error of 2. You want to halve your standard
error to 1. How large does n need to be? (Answer: n = 400.
The standard error scales as 1/√n; halving SE requires
quadrupling n.)
```

Now the two builds.

**Live build (`deck_mode: live`):**

```html
<!-- GOOD: live deck. Sparse. The speaker carries the verbal content.
     Visual channel is occupied by a single dynamic diagram. Notes
     field carries the full speaker script. -->
<section class="slide" data-mode="live">
  <h1>The sampling distribution narrows toward normality as n grows.</h1>
  <!-- Full-sentence assertion headline. The student leaves the slide
       with a claim in their head, not a topic. -->

  <figure class="sampling-distribution">
    <!-- D3 animation: skewed population at top, sampling distributions
         at n=2, 10, 30, 100. Plays once when slide appears, can be
         replayed by the speaker. No labels except axes and n. -->
  </figure>

  <div class="notes">
    <!-- Full speaker script, drawn from the source's "Speaker script"
         block. The speaker reads notes, not the slide. The audience
         watches the animation while listening. Two channels, two
         contents, no collision. -->
    The CLT is the reason inference works. Start with any population —
    exponential, uniform, weirdly bimodal — and draw samples of size
    n. Compute each sample's mean. Plot the distribution of those means.
    As n grows, the distribution of means narrows and becomes normal,
    regardless of the original shape. The narrowing follows σ/√n. So
    to halve the standard error, you need four times as many samples.
    [continue speaker script through the worked-example moment;
    invite a paired discussion: "halve the standard error — how many
    more samples?"]
  </div>
</section>
```

**Study build (`deck_mode: study`):**

```html
<!-- GOOD: study artifact. Dense. The slide carries the verbal content.
     The speaker is not present; the explanation has to live on the slide.
     Modality Principle's boundary conditions apply: text is technical,
     learner-paced, no narration available — on-screen text is required.
     Embedded retrieval prompt produces forced practice. -->
<section class="slide" data-mode="study">
  <h1>The sampling distribution of the mean narrows toward normality as n grows — no matter what shape the underlying population has.</h1>
  <!-- Full-sentence assertion as in live mode. -->

  <figure class="sampling-distribution">
    <!-- Same D3 visual, but here labeled with σ/√n on the standard-error
         arrow at each n; population mean μ marked; the four sampling
         distributions annotated with their standard errors. -->
    <figcaption>
      As n grows from 2 to 100, the sampling distribution of the mean
      narrows (standard error σ/√n shrinks) and approaches a normal
      distribution. The result holds regardless of the population's
      shape, provided variance is finite.
    </figcaption>
  </figure>

  <div class="explanation">
    <p>
      Take any population P with mean μ and standard deviation σ.
      Draw N independent samples of size n from P. For each sample,
      compute the mean. The distribution of these N sample means is
      the <em>sampling distribution of the mean</em> for sample size n.
    </p>
    <p>
      The CLT states two things about the sampling distribution: its
      mean is μ (same as P), and its standard deviation is σ/√n. As n
      grows, σ/√n shrinks — the sampling distribution narrows — and
      its shape approaches normal regardless of the shape of P. This
      is why inference methods that assume normality (t-tests, z-tests,
      confidence intervals) work for non-normal populations when n
      is large enough.
    </p>
  </div>

  <div class="retrieval-prompt">
    <strong>Try this before continuing.</strong>
    A population has σ = 20. You currently sample n = 100 and observe
    a standard error of 2. You want to halve your standard error to 1.
    How large does n need to be?
    <details>
      <summary>Reveal the answer.</summary>
      n = 400. The standard error scales as 1/√n; halving SE requires
      quadrupling n.
    </details>
  </div>

  <div class="notes" style="display:none">
    <!-- Notes optional in study mode. The slide carries the content.
         Notes can hold pointers to the textbook section, related
         problem set, or further reading. -->
  </div>
</section>
```

Look at what changed across the two builds.

| Element | Live build | Study build |
|---|---|---|
| Headline | Assertion ("narrows toward normality as n grows") | Same assertion, extended to include "no matter what shape" |
| Visual | Animation; minimal labels | Same animation; full labels including σ/√n |
| Body text | None | Two paragraphs of self-contained explanation |
| Caption | None | Caption that summarizes the visual |
| Retrieval prompt | Verbal — speaker invites paired discussion | Embedded — student attempts before reveal |
| Notes field | Full speaker script | Optional; references the textbook section |

The content is identical. The *artifact* is different in five specific places. The instructor toggles `deck_mode: live` for the morning lecture and `deck_mode: study` for the post-lecture posting. The same `lecture-04-clt.md` source generates both. When the content changes — a clarification to the script, a new retrieval prompt — both rebuilds reflect the change. Two artifacts, one source of truth.

This is the central practical move of the chapter, and the practical move of the deck-level half of the book. The DESIGN.md toggle is what lets the reader stop negotiating between the two pulls and produce two artifacts each respecting its own constraint.

## 6. The prompt

The Brutalist prompt for converting a slideument source into two-mode artifacts:

```
From this content source, produce two outputs:

  1. A LIVE-LECTURE DECK where each slide is a sparse anchor for
     spoken explanation. Headlines are full-sentence assertions.
     Body text is minimal — one image, one diagram, or one phrase.
     The slide does not stand alone; the speaker carries the
     explanation. The NOTES FIELD is populated with the full
     speaker script for each slide.

  2. A STUDY ARTIFACT DECK where each slide is a self-contained
     explanation. Headlines are full-sentence assertions
     (the same as in live mode). The slide body contains the
     prose explanation — what the speaker would say, rendered
     as on-screen text. Visuals are captioned. Every 3–5 slides
     includes an embedded retrieval prompt the student attempts
     before revealing the answer.

Toggle DESIGN.md `deck_mode` between `live` and `study` to
switch which artifact is built. The source content remains
identical; the rendering differs.

Do not produce a hybrid. A hybrid is a slideument — text-heavy
enough that the live audience reads instead of listens, but
not detailed enough to study from when the speaker is absent.
The hybrid serves neither use case. Refuse it.
```

The prompt does two things at once. It forces the instructor to declare which artifact they are making in this build — a declaration most slide-design failures begin by skipping. And it specifies the difference between the two outputs precisely enough that the Brutalist system (or Gamma, or any LLM-driven slide tool) can act on it. The principle is portable; only the system name changes.

## 7. The DESIGN.md change

The `deck_mode` toggle is the central DESIGN.md change of the chapter. The same DESIGN.md variables — body text density, headline style, retrieval prompts, notes field conventions — take different values depending on the mode flag.

```yaml
# DESIGN.md — deck_mode toggle and the variables it controls

deck_mode: live   # or "study"
# The single most consequential variable in this DESIGN.md. Every
# variable below depends on it. Setting deck_mode commits the
# artifact to a use case. Do not produce hybrid artifacts.

# === LIVE MODE ===
# When deck_mode: live
body_text_density_target: 0-20-words-per-slide
# Sparse. The speaker carries the verbal content. The slide is
# an anchor, not an explanation.

headline_style: assertion-full-sentence
# Full-sentence assertion (Atkinson/Alley). Not a topic label.

slide_body_form: image-led-or-headline-only
# Body is a diagram, a chart, an image, a phrase, or a number.
# Not paragraphs. Not bullet lists longer than 3 items.

notes_field: full-speaker-script
# The full verbal content lives in the notes field. The speaker
# reads notes, not the slide.

retrieval_prompt_form: verbal-or-paired-discussion
# Retrieval moments are invited by the speaker — clicker
# questions, paired discussions, written attempts. The prompt
# may appear on the slide as a question; the answer does not.

# === STUDY MODE ===
# When deck_mode: study
body_text_density_target: 60-150-words-per-slide
# Higher. The slide carries the explanation in the absence of
# a speaker. Modality Principle's boundary conditions apply:
# learner-paced, no narration available, on-screen text required.

headline_style: assertion-full-sentence
# Same as live mode. The assertion structure is the one
# convention that ports across both artifacts.

slide_body_form: prose-with-captioned-visual
# Body is a self-contained explanation, with a visual that has
# a caption summarizing what the visual shows.

notes_field: optional-references-only
# Notes are optional and contain pointers to the textbook
# section, problem set, or further reading. The slide does not
# depend on the notes.

retrieval_prompt_form: embedded-with-reveal
# Every 3–5 slides, an embedded retrieval prompt the student
# attempts before clicking to reveal the answer. Forced
# practice without a speaker requires the artifact to enforce
# the attempt.
```

Two things to notice. First, `headline_style: assertion-full-sentence` ports across both modes. The assertion-headline move is the one convention that the live and study artifacts share, because in both cases the student should leave the slide with a *claim* rather than a topic label. (Chapter 10 picks up the assertion-evidence move at the slide level.) Second, `body_text_density_target` is the variable that does the most work in distinguishing the two modes. In live mode the target is near zero; in study mode it is closer to a paragraph. The same content source produces dramatically different word counts on the rendered slide depending on the mode flag.

## 8. The diagnostic questions to keep

For any deck, before opening the slide tool, and again at every dress rehearsal:

1. **Is this deck a live anchor or a study artifact?** State it out loud. If you cannot, the deck is going to drift into slideument by default.
2. **Could a student make sense of this slide without me?** If yes, the slide is a study slide. If no, the slide is a live slide. Most decks contain a mix; the mix is the slideument. Count the ratio and decide which the deck is for.
3. **What channel is carrying the verbal content?** If the speaker is carrying it, the slide should not also be carrying it (Redundancy). If no speaker is present, the slide must carry it (no choice).
4. **Where are the retrieval moments, and how are they enforced?** In live mode: verbal prompts the speaker invites. In study mode: embedded prompts the artifact enforces. "Q&A at the end" is not a retrieval moment in either mode.
5. **If a student emailed asking for the slides three days after the lecture, what would they receive — the live artifact, the study artifact, or a slideument?** The honest answer is the diagnostic. Most decks produce a slideument here, which is what creates the chronic complaint.

The questions are mostly about *which artifact you are making this time*. Get that declaration right at the start and the rest of the design choices follow. Get it wrong and every later choice negotiates against itself.

## 9. What two people might disagree about

The genuine disagreement is about a populated notes field. One position holds that a well-populated notes field can make a live deck functionally usable as a study artifact: the slide carries the visual anchor, the notes carry the explanation, the student studies from the notes-augmented deck and gets what they need. The other position holds that students do not, in practice, use the notes field — they download the PDF of the slides and study from that, never opening the notes view — so the notes field is technically a study channel but its adoption rate is too low to count on.

Both positions are defensible, and the empirical answer depends on the LMS and the workflow. Some LMS configurations show the notes by default when a student downloads the slides; in those contexts, the notes field is a real study channel. Other configurations hide the notes; in those contexts, the notes field is invisible to most students. The chapter's recommendation — produce two artifacts — does not require resolving the disagreement. It only requires accepting that the answer matters and that the instructor should *know* which configuration their students are using.

A second disagreement is about generative-AI auto-conversion. Tools like Gamma and Beautiful.ai increasingly offer a "presentation view" vs. "expanded view" toggle, where the same content renders sparse for live use and expanded for study use. This is the right direction, and it matches the Brutalist `deck_mode` move structurally. The disagreement is whether the auto-conversion is good enough yet. My current reading is: the toggle is real, the output is uneven, and the instructor who relies on auto-conversion without inspecting both artifacts is back in the slideument failure mode at the auto-tool's defaults rather than at their own.

The vocabulary for these disagreements is sharper than "I prefer one deck" vs. "I prefer two":

- *Which channel is carrying the verbal content in this artifact?* (Names the mode.)
- *What is the adoption rate of the notes field in this LMS configuration?* (Names the empirical fact that determines whether notes are a real study channel.)
- *What is the failure mode of the AI tool's auto-conversion, for my specific content?* (Names the test the instructor should run before trusting the toggle.)

A disagreement at the level of those three questions can converge. A disagreement at the level of "but students need to study from the lecture slides" misses the point: yes, they do — and what they study from should be designed for study, not inherited from a live deck. The same source content can produce both. One artifact cannot be both.

---

Bridge to Chapter 10. This chapter taught the live/study decision and the two-artifact workflow that follows from it. The next chapter zooms back to the individual slide — specifically, to the *headline* — and asks the question that anchored both the live and study builds above: *is this headline a claim or a label?* The assertion-evidence move is the slide-level expression of the live-deck philosophy, and it is where the seven chapters before it converge into a single practical commitment about what the top of every slide is for.

---

**What would change my mind:** Empirical evidence that a single well-designed deck — one artifact, not two — produces equal or better outcomes than a matched two-artifact pair (live deck + study artifact) on both the live-attendance retention measure *and* the post-lecture study-from-slides retention measure. The component evidence (Modality, Redundancy, assertion-evidence) supports the two-artifact split. A direct comparison of one-artifact vs. two-artifact workflows on student outcomes is, as far as I have found, missing. Acknowledged in the research notes as the central empirical gap of the chapter.

**Still puzzling:** Why some recorded narrated decks — "slidecasts" with sparse slides and dense narration — seem to function reasonably well as async study materials despite violating the chapter's stated rule that sparse decks don't stand alone. My best guess is that the recording is acting as the study artifact (the verbal content is preserved), with the deck functioning as a visual outline rather than the explanation itself. If true, the chapter's "two artifacts" rule generalizes to "one deck and one recording" as a special case, where the recording is the study artifact. I have not worked through the cases carefully enough to know whether this is a tidy generalization or a hand-wave. [verify whether there is empirical work on slidecast retention specifically — possibly Schroeder.]

**Tags:** modality-principle, redundancy-principle, slideument, assertion-evidence, two-artifact-workflow
