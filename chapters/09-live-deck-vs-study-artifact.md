# Chapter 9 — Live Deck vs. Study Artifact


## TL;DR

- Is this deck a visual anchor for your spoken explanation, or is it the self-contained explanation itself — and could a student make sense of it without you?
- The chapter moves through Two channels, one bottleneck, What the failure looks like, What the repair looks like, The prompt that forces the declaration, and related ideas.
- Read it for the main argument, the vocabulary it introduces, and the practical judgment it asks you to develop.

*Is this deck a visual anchor for your spoken explanation, or is it the self-contained explanation itself — and could a student make sense of it without you?*

---

There is a constraint in the design of a lecture deck that most instructors never state out loud, and the failure to state it is responsible for a specific, recurring complaint from students. The complaint comes in two contradictory forms, and the contradiction is diagnostic.

One form: *the slides are so dense, I can't listen to you and read at the same time.* The other form: *I went back to the slides to study and they don't make sense without the lecture.* These two complaints are not made about different decks. They are made about the same deck, by different students, at different moments — the first during the lecture, the second three weeks later before the exam.

A single deck cannot be both a live anchor for spoken explanation and a self-contained study artifact. The two use cases impose opposite design constraints, for a reason rooted in how working memory processes information. Understanding that reason is what makes the constraint precise rather than just annoying.

---

## Two channels, one bottleneck

Working memory is divided. There is a verbal channel — the one that processes language, whether spoken or read. There is a visual-spatial channel — the one that processes images and spatial relationships. The two channels are largely independent, which is why a spoken narration and a diagram can run in parallel without degrading each other. That parallel processing is the core design insight behind good multimedia instruction.

The constraint arrives when both inputs to working memory are *language*. Text on a slide is processed through the verbal channel. The speaker's voice is also processed through the verbal channel. When a speaker narrates content that is already on the screen in text form, both inputs arrive at the same channel at the same time and compete. One wins; the other is suppressed. Usually the screen wins, because it is stable and effortless to read. The speaker becomes an audio track competing with printed text for the same limited resource.

Richard Mayer calls this the Redundancy Principle, and the experimental evidence behind it is substantial: students given animation plus narration outperform students given animation plus narration plus on-screen text that duplicates the narration. The extra text made learning worse. Not neutral — worse. Both channels were flooded with the same content, and the collision cost was real.

Now here is where it gets interesting. The Modality Principle, which Mayer also established, says something that seems to point in the opposite direction: people learn more deeply from pictures plus spoken words than from pictures plus printed words. The spoken narration uses the verbal channel while the visual uses the visual-spatial channel — two parallel streams, no bottleneck. A live lecture with sparse slides and a speaking instructor is the optimal configuration by this principle.

But Mayer specifies the boundary conditions under which the modality advantage holds: it is strongest for live, novel, instructor-paced instruction. It weakens or disappears when the material is learner-paced, when the content is highly technical and needs re-reading, when the learner is non-native, or when there is no narration available. Those boundary conditions describe *study mode* almost exactly. The principle that argues for sparse slides in live use is the same principle that argues against sparse slides in async study — because the principle depends on the narrator being present, and in study mode the narrator is gone.

This is the asymmetry. In live delivery, you have a narrator. The verbal channel is occupied by speech; the visual channel can carry images cleanly; on-screen text becomes redundant and harmful. In async study without a narrator, the verbal channel is silent: the slide must carry text, because nothing else carries the verbal content. The same design move that respects the modality principle in one mode violates it in the other.

A single deck cannot satisfy both constraints simultaneously. Either it is sparse — designed for the presence of a speaker — or it is annotated — designed for the absence of one. The features that make a slide good for live use are exactly the features that make it bad for study use, and vice versa.

| Item | Meaning |
| --- | --- |
| verbal channel source (speaker's voice | on-screen text |
| visual channel source (diagrams, minimal labels | annotated visuals with captions |
| slide body word count (0–20 words | 60–150 words |
| notes field role (full speaker script | optional references |
| retrieval mechanism (speaker-enforced verbal prompt | artifact-embedded attempt-then-reveal |

---

## What the failure looks like

The slide I want to examine is on the Central Limit Theorem, from an introductory statistics course. An instructor needs this slide both for Monday's live lecture and for the async section that watches a recording later in the week. One deck. Both uses.

The slide in slideument form has a topic-label headline — "The Central Limit Theorem" — followed by five bullets running to about seventy-five words. The bullets describe the theorem, its conditions, its conclusions. Reading time is roughly twenty seconds.

In live use, the instructor advances to the slide and begins to explain the CLT verbally. The students have already started reading the bullets — they are text, they are present, the verbal channel cannot resist processing them. By the time the instructor is two sentences into the explanation, half the room is still on bullet three. The verbal channel is split between reading and listening. The instructor is narrating content that is already on the screen, which is the redundancy violation in real time.

In study use, three weeks later, a student pulls up the slide to review before the midterm. The five bullets are there. They are correct. They do not contain a worked example, a diagram of the sampling distribution narrowing as n grows, a derivation of the standard error formula, or a retrieval prompt to test understanding. They are five statements of fact arranged in a list. The student can read them and verify that they have seen the CLT described. They cannot, from this slide alone, reconstruct what the CLT *does* or why it works. The slide "stands alone" in the sense that the words are present. It does not stand alone in the sense that the words explain.

Both complaints are valid. The deck is too dense for the live moment and too sparse for the study moment. The instructor is not at fault for trying to make one deck serve two purposes — that is the obvious, efficient choice. The fault is in not naming the constraint that makes the obvious choice structurally impossible.

![Mockup of the slideument CLT slide ](images/09-live-deck-vs-study-artifact-fig-01.png)
*Figure 9.1 — Mockup of the slideument CLT slide *

---

## What the repair looks like

The repair is to produce two artifacts from one source.

The live deck carries a single assertion as the headline: *The sampling distribution narrows toward normality as n grows.* The body is an animation — the skewed source distribution at the top, sampling distributions for n of 2, 10, 30, and 100 rendered below it, each progressively narrower and more bell-shaped. That is the entire slide. The visual channel carries the mechanism. The verbal channel carries the speaker's explanation. The notes field holds the full speaker script: the derivation of the standard error, the worked example of halving the standard error by quadrupling the sample size, the connection to why inference methods work on non-normal populations. The notes are what the speaker reads, not what the audience sees.

The study artifact carries the same headline. The animation now has full labels — the standard error formula at each n, the population mean marked, the four distributions annotated with their standard errors. Below the animation: two paragraphs of prose that explain, in the absence of a speaker, why the sampling distribution narrows, what the formula σ/√n means, and why the result holds regardless of the population's shape. After the explanation: an embedded retrieval prompt — *A population has σ = 20 and you are sampling n = 100. You want to halve your standard error. How large does n need to be?* — followed by a reveal of the answer.

The content is identical across both artifacts. The assembly is different in five specific places: word count on the slide body, labels on the visual, presence of a prose explanation, presence of a caption, and the form of the retrieval moment. The live deck assumes a speaker; the study artifact cannot.

![Mockup of the two CLT artifacts ](images/09-live-deck-vs-study-artifact-fig-02.png)
*Figure 9.2 — Mockup of the two CLT artifacts *

Notice what this requires. It requires the instructor to declare, before designing the slide, which artifact they are making. That declaration is the design decision most slide failures begin by skipping. The decision feels unnecessary — "it's the CLT slide, it's the same either way" — but it is not the same either way, and the students feel the difference even when the instructor does not name it.

---

## The prompt that forces the declaration

When working with AI slide tools, the structural move is to give the tool a `deck_mode` directive before it generates. Not "make this a lecture slide" — a mode flag that commits the output to a specific use case and makes a hybrid unacceptable.

---

*From this content source, produce two outputs.*

*Output 1 — live-lecture deck: each slide is a sparse anchor for spoken explanation. Headlines are full-sentence assertions. Body text is minimal — one image, one diagram, or one phrase. The slide does not stand alone; the speaker carries the explanation. The notes field is populated with the full speaker script for each slide.*

*Output 2 — study artifact deck: each slide is a self-contained explanation. Headlines are the same full-sentence assertions as in the live deck. The slide body contains the prose explanation as on-screen text. Visuals are captioned. Every three to five slides includes an embedded retrieval prompt the student attempts before revealing the answer.*

*Do not produce a hybrid. A hybrid is a slideument — text-heavy enough that the live audience reads instead of listens, but not detailed enough to study from when the speaker is absent. The hybrid serves neither use case.*

---

Two things to notice. First, the assertion headline is the same across both outputs. That is the one convention that ports: a full-sentence claim rather than a topic label. The student in the live lecture and the student studying alone both need to leave with an assertion in their head rather than a filing category. The assertion-evidence structure — full-sentence headline, visual evidence in the body — is the shared grammar. What differs is how much the slide body carries and whether the notes field is the speaker's script or the student's study text.

Second, the explicit refusal of the hybrid is not aggressive. It is a constraint that protects both artifacts. The tool's default, without the directive, is to produce something that looks professional and complete — which, as the chapters before this one have established, is the failure mode disguised as thoroughness.

---

## Where retrieval lives in each mode

One thing the two-artifact split makes visible is how differently retrieval moments must be handled across the two use cases.

In a live lecture, retrieval is something the speaker manages. A question posed out loud. A moment of paired discussion. A clicker question on screen where the audience attempts before the instructor reveals the answer. The instructor enforces the attempt — the room waits, the timer runs, students cannot skip the effort. The slide may show the question; it does not need to show the mechanism for attempt-then-reveal, because the speaker is the mechanism.

In a study artifact, no speaker is present to enforce the attempt. A student who wants to skip the retrieval prompt and scroll to the answer will scroll to the answer, unless the artifact resists. The embedded reveal — the question visible, the answer hidden behind a click — is the study artifact's only leverage. It is a weak mechanism compared to a live instructor, but it is the best available. Slides that contain only declarative statements, with no retrieval structure embedded, produce passive re-reading rather than active recall. Active recall is what produces durable memory; passive re-reading produces the feeling of knowledge without its substance.

This distinction — retrieval enforced by speaker in live mode, retrieval enforced by artifact in study mode — is another place where the two artifacts diverge in ways a single deck cannot bridge. A deck built for live use has no embedded retrieval because the speaker handles it. Posted as a study artifact after the lecture, the same deck invites passive re-reading. A deck built for study with embedded reveals and annotated visuals is disruptive in a live lecture, because the attempt-and-reveal sequence requires time the live session does not have. Each mode needs its own retrieval architecture.

![The speaker is the retrieval mechanism in live mode. The artifact must be its own retrieval mechanism in study mode. A posted live deck provides neither.](images/09-live-deck-vs-study-artifact-fig-03.png)
*Figure 9.3 — Two-column diagram showing retrieval architecture *

---

## The asymmetry of detection, one more time

The slideument failure for a full deck has the same invisibility property as the slideument failure for a single slide.

At the point of design, the instructor is working alone. The live use case is not present; the study use case is not present; only the content is present. The deck that tries to serve both feels more responsible than the deck that commits to one — it feels like covering all the bases. The two conflicting complaints are not yet available to be noticed. They only arrive after the deck has been used, at which point fixing it requires redesigning from scratch.

AI tools compound this in a specific way. The tool produces a deck that looks finished — professional, dense enough to seem complete, sparse enough to seem projectable. It has learned the aesthetic of the professional slide and has no way to measure what happens to the verbal channel in the room, or what a student's working memory does with the content in the absence of the speaker. The tool produces the slideument not because it is bad at design but because the slideument is what the training signal calls polished.

The fix is upstream of the design tool: declare the mode before generating. The instructor who opens a slide tool and starts building is already in the negotiation between live and study, and the negotiation produces the hybrid by default. The instructor who says "this build is the live deck; the study artifact is a separate build from the same source" has already made the only decision that matters.

---

## What two instructors might argue about

The genuine disagreement, once the two-artifact principle is accepted, is about the notes field.

One position: a well-populated notes field converts a live deck into a functional study artifact. The slide carries the visual anchor; the notes carry the explanation; the student who downloads the deck in notes-view gets a complete document. The two-artifact workflow is unnecessary — one source file, one deck, notes field populated, and the student can study from it.

The other position: students do not use the notes field. They download the PDF of the slides and study from that, in slide view, without ever opening the notes. The notes field is technically a study channel but its actual adoption rate is too close to zero to count on as a design commitment. The instructor who relies on the notes field as the study artifact is designing for behavior they believe students should exhibit, not behavior the evidence suggests they do.

Both positions are defensible. The empirical answer depends on the LMS configuration — some learning management systems show notes by default when a student opens the course materials; others hide them. The chapter's recommendation does not require resolving the disagreement. It only requires that the instructor know which configuration their students are actually using before deciding that the notes field is the study artifact.

| Students reliably access notes | Students download slide PDF only |
| --- | --- |
| "LMS shows notes by default" | "LMS hides notes by default" |
| columns: "Students reliably access notes" | "Students download slide PDF only" |
| cells: (show + access) → "Notes field is a viable study channel | A concrete checkpoint for applying the chapter concept. |
| one-deck workflow may be sufficient" | A concrete checkpoint for applying the chapter concept. |
| show + PDF) → "Notes field is visible but bypassed | A concrete checkpoint for applying the chapter concept. |
| study channel unused" | A concrete checkpoint for applying the chapter concept. |
| hide + access) → "Students actively seek notes | A concrete checkpoint for applying the chapter concept. |
| unusual but possible" | A concrete checkpoint for applying the chapter concept. |
| hide + PDF) → "Notes field is invisible to most students | A concrete checkpoint for applying the chapter concept. |
| two-artifact workflow required" | A concrete checkpoint for applying the chapter concept. |

There is also a question about recorded narrated decks — slidecasts with sparse slides and dense audio narration — which seem to function reasonably well as async study materials despite being live-deck configurations. If the recording is what the student studies, then the recording is the study artifact and the sparse slide is the visual outline. The two-artifact rule generalizes here to "one deck and one recording," where the recording substitutes for the annotated study deck. Whether the substitution is complete — whether a recorded narration provides everything a designed study artifact would — is something I do not have a clean answer to. My intuition is that the recording is better than a sparse slide without audio and worse than a designed study artifact with embedded retrieval, but that is a guess about a spectrum rather than a claim about a boundary.

The vocabulary that makes both disagreements productive: *which channel is carrying the verbal content in this specific artifact, under the conditions the student is actually using it?* Answer that question for the specific LMS, the specific student behavior, and the specific content, and the design decision follows.

---

**What would change my mind:** Empirical evidence that a single well-designed deck — one artifact — produces equal or better outcomes than a matched two-artifact pair on both the live-attendance retention measure and the post-lecture study-from-slides retention measure. The component evidence (Modality, Redundancy, assertion-evidence) supports the two-artifact split. A direct comparison of one-artifact versus two-artifact workflows on student outcomes is, as far as I have found, missing. That is the central empirical gap in this chapter's argument, and I hold the recommendation with appropriate tentativeness.

**Still puzzling:** The boundary between "this sparse live deck plus its recording" and "this designed study artifact" is not as clean as the chapter implies. Mayer's boundary conditions for when the modality advantage fades include learner-paced material, which a recording is — the student can pause and rewind. If pausing and rewinding closes the gap between a recorded lecture and a designed study artifact, the two-artifact workflow may matter less for institutions that systematically record. I have not worked through the cases carefully enough to know.

---

## Exercises

**Warm-up**

1. A faculty member teaches a Tuesday lecture and posts the same slide deck to the LMS for students who missed class. The deck has 60-word-per-slide bullets and a speaker who narrates most of what the bullets say. Name the two Mayer principles being violated simultaneously, explain which violation occurs in live use and which occurs in study use, and state why a single fix cannot resolve both. *Tests: ability to distinguish the Redundancy and Modality violations and see them as structurally opposed.*

2. The Modality Principle argues for sparse slides paired with spoken narration. List the four boundary conditions Mayer specifies under which the modality advantage weakens or disappears. Then state which of those conditions apply to an async student studying from posted slides at midnight before an exam. *Tests: understanding that the Modality Principle is conditioned, not universal, and that study mode meets the conditions that invert it.*

3. An instructor posts lecture slides as the study artifact. A student emails: "the slides have everything on them but I can't tell what mattered." A second student emails: "the slides don't make sense without the lecture." Both complaints are about the same deck. Explain how one deck can produce both complaints simultaneously, using the channel-asymmetry argument from this chapter. *Tests: ability to trace the two-complaint failure to a single structural cause.*

**Application**

4. Take a deck you currently use for a live lecture that you also post to students for study. Audit it: count the average words per slide, check whether the notes field is populated, and ask whether a student who missed class could reconstruct the argument from the slides alone. Classify it honestly: live deck, study artifact, or slideument. If it is a slideument, identify which five slides would require the most significant redesign to split into two proper artifacts. *Tests: ability to apply the audit to one's own work and identify the high-cost redesign points.*

5. Design the live-deck version of a CLT slide for a different statistics concept of your choosing — confidence intervals, say, or p-values. Write the assertion headline, describe the visual, and write the notes field speaker script. Then describe what changes in the study-artifact version: what labels are added, what prose is written, and what retrieval prompt is embedded. You do not need to build both; describe both. *Tests: ability to generate the two-artifact split from scratch on new content.*

6. An instructor argues: "I populate my notes field with the full script. Students who want the explanation can read it there. I only need one deck." What is the strongest version of the rebuttal? What empirical fact about student behavior does the instructor need to verify before their argument holds? What LMS configuration question do they need to answer? *Tests: ability to identify what makes the notes-field argument conditionally valid and what would falsify it.*

**Synthesis**

7. Mayer's boundary conditions for the modality advantage include "learner-paced." A slidecast — sparse slides plus recorded narration — is learner-paced because the student can pause and rewind. Does this mean a slidecast functions as a study artifact? Argue both sides: what does the recording provide that a designed study artifact also provides, and what does an embedded-retrieval study artifact provide that a recording cannot? Where, if anywhere, is the recording a complete substitute? *Tests: ability to reason about the slidecast as a special case and identify what it can and cannot substitute.*

8. The chapter claims that "the features that make a slide good for live use are exactly the features that make it bad for study use." Construct the strongest argument *against* this claim — a case where a single design decision genuinely serves both modes without compromise. If you find one, name it; if you cannot, explain why the constraint is structural rather than just typical. *Tests: ability to stress-test the chapter's central claim by looking for genuine exceptions.*

**Challenge**

9. The chapter's "what would change my mind" admits that a direct comparison of one-artifact versus two-artifact workflows on student outcomes does not exist. Design that study. What is the independent variable (specify both conditions precisely), what are the dependent variables (specify at least two outcome measures at different timescales), how do you control for instructor, content, and prior knowledge, and what statistical result would constitute evidence that the two-artifact workflow is *not* worth the additional production cost? *Tests: ability to specify the missing study precisely enough to evaluate whether it would actually answer the question.*

---

*This chapter taught the live-versus-study decision and the two-artifact workflow that follows from it. The next chapter zooms back to the individual slide — specifically, to the headline — and asks the question that anchored both builds above: is this headline a claim or a label? The assertion-evidence structure is the slide-level expression of the live-deck philosophy, and it is where the chapters before it converge into a single practical commitment about what the top of every slide is for. That's Chapter 10.*

## Prompts

Use these prompts with Claude to generate interactive D3 v7 versions of the
figures in this chapter. Each produces a standalone HTML file you can open
in a browser and modify freely.

**Prerequisites:** Load `brutalist/CLAUDE.md` and `brutalist/DESIGN.md` into
your Claude project context before using these prompts. They define the stack,
naming conventions, color system, and typography the figures use.

---

### Figure 9.1 — Mockup of the slideument CLT slide 

Create a standalone D3 v7 HTML file for Figure Mockup of the slideument CLT slide . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: rendered mockup of the slideument CLT slide — topic-label headline "The Central Limit Theorem"; five bullet points running to ~75 words filling the slide body; empty notes pane at bottom; two annotation callouts: (1) pointing at the bullet text with "Live failure: student reads while speaker narrates — Redundancy violation"; (2) pointing at the empty notes pane with "Study failure: no worked example, no diagram, no retrieval prompt — slide describes but does not explain". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variables and the required serif/mono font split.

> Reference implementation: `d3/09-live-deck-vs-study-artifact-fig-01.html`

---

### Figure 9.2 — Mockup of the two CLT artifacts 

Create a standalone D3 v7 HTML file for Figure Mockup of the two CLT artifacts . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: side-by-side mockup of the two CLT artifacts — left panel "Live Deck": assertion headline "The sampling distribution narrows toward normality as n grows.", animation of sampling distributions at n=2/10/30/100 with minimal axis labels, notes pane filled with speaker script text; right panel "Study Artifact": same headline, same animation but fully labeled with σ/√n at each n, two paragraphs of prose explanation below the animation, retrieval prompt "A population has σ = 20, n = 100. You want to halve your standard error. What n is required?" with hidden reveal; annotation arrows pointing to the five specific differences between the panels. Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only 

> Reference implementation: `d3/09-live-deck-vs-study-artifact-fig-02.html`

---

### Figure 9.3 — Two-column diagram showing retrieval architecture 

Create a standalone D3 v7 HTML file for Figure Two-column diagram showing retrieval architecture . Use the CDN https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js, inline CSS, ResizeObserver redraw, SVG role="img", aria-labelledby, title, and desc. Build the figure from this structural brief: two-column diagram showing retrieval architecture — left column "Live Mode": speaker icon → poses question verbally → room waits → timer → reveal; right column "Study Mode": embedded question on slide → student attempts → click to reveal → answer appears; below both columns: "Passive re-reading (no retrieval structure) → feeling of knowledge without its substance"; caption: "The speaker is the retrieval mechanism in live mode. The artifact must be its own retrieval mechanism in study mode. A posted live deck provides neither.". Use the described data shape and labels; when exact values are not supplied, use plausible illustrative values that preserve the relationships in the brief. Use a zero baseline for bars or areas, direct labels where possible, and annotations named in the brief. Use only DESIGN.md color variables and the required serif/mono font split.

> Reference implementation: `d3/09-live-deck-vs-study-artifact-fig-03.html`
