# Chapter 12 — The Diagnostic Checklist

> One reference page. Use it before every deck ships.

---

## 1. Why this chapter exists

On October 30, 1935, the prototype Boeing Model 299 — the aircraft that would become the B-17 — crashed during a demonstration flight at Wright Field. Two of the five crew died. The investigation was short. The pilots had forgotten to release a control lock before takeoff. The Model 299 was not too difficult for trained pilots; one of the country's most experienced test pilots was at the controls. It was too complex to fly without external scaffolding for memory. Boeing's response was the pre-flight checklist — a short, ordered list of items printed on a single card. With the checklist, the B-17 went on to fly 1.8 million miles without an accident attributable to pilot oversight. Some `13,000` were built. The case is the founding story of the modern professional checklist, recounted in [Atul Gawande's *The Checklist Manifesto* (Metropolitan Books, 2009)](https://www.atulgawande.com/book/the-checklist-manifesto/), ch. 2.

The case that matters for this book is not the airplane. It is the failure mode the checklist prevents. The pilots did not crash because they did not know to release the control lock. They knew. They crashed because, under the pressure of a demonstration flight, the knowledge was not retrievable at the right moment. The checklist offloads retrieval from working memory to a stable external artifact. The pilot's working memory is freed for the parts of the job that genuinely require judgment.

The clinical evidence is the next step in the argument. [Pronovost et al. (2006) in the *New England Journal of Medicine*](https://www.nejm.org/doi/full/10.1056/NEJMoa061115) `[verify DOI 10.1056/NEJMoa061115]` implemented a five-item central-venous-catheter checklist across 103 Michigan ICUs — the Keystone ICU project. Items as simple as *wash hands. Use full sterile barriers. Clean skin with chlorhexidine. Avoid femoral insertion. Remove unnecessary catheters.* The median rate of catheter-related bloodstream infections fell from 2.7 per 1,000 catheter-days at baseline to 0 within three months, sustained at 66% below baseline at 16–18 months. The [Haynes et al. (2009) NEJM paper](https://www.nejm.org/doi/full/10.1056/NEJMsa0810119) `[verify DOI 10.1056/NEJMsa0810119]` extended the case with the WHO Surgical Safety Checklist — a 19-item, single-page checklist run at three points in a surgical procedure, implemented in eight hospitals across high-income and low-income settings. In-hospital mortality dropped from 1.5% to 0.8% (a 47% reduction); inpatient complications dropped from 11% to 7%.

The honest critique arrived three months after Haynes. [Bosk, Dixon-Woods, Goeschel, and Pronovost (2009) in *The Lancet*](https://doi.org/10.1016/S0140-6736%2809%2961440-9) `[verify DOI 10.1016/S0140-6736(09)61440-9]` argued that the checklists worked only because they sat inside broader cultural and organizational change — empowered nurses, leadership commitment, data feedback. Deploy the checklist alone, without the surrounding work, and it becomes paperwork. *"A technical solution to a cultural problem,"* they called it, *"is likely to fail or to be resented."* This matters here. The Brutalist diagnostic checklist works for a reader who has built the diagnostic vocabulary in Chapters 1–11. Hand it to a faculty member who has not read the book and it will read as forty arbitrary questions. The checklist is the visible artifact. The reading was the cultural change. Both are required.

The slide-design case is structurally analogous and empirically thinner. There is no published study of whether a slide-design checklist improves slide quality or learning outcomes. The argument here is by structural analogy from the clinical and aviation literature, not by direct empirical demonstration. That is honest research extrapolation and worth flagging here rather than burying.

## 2. How to use this checklist

There are two architectures for a checklist, named in the aviation literature and recounted in Gawande. A *read-do* checklist is executed step by step as you read each item: read step one, do step one, read step two, do step two. A recipe is read-do. A *do-confirm* checklist is run after the task is complete: you build the thing, then run the checklist to confirm nothing was missed. A surgeon's pre-incision checklist is do-confirm. The right choice depends on whether the steps must occur in a specific order (read-do) or whether you can perform the task fluently and might omit a step under cognitive load (do-confirm).

**This checklist is do-confirm.** Build the deck. Then run the checklist to confirm before shipping. The questions are framed in the diagnostic mood ("Is the headline a claim or a label?") rather than the imperative ("Write a claim headline"). Reading the checklist before each slide would be slower than building intuition; running the checklist after the deck exists catches the failures the intuition missed.

There is also a familiarity gradient. The first three or four times you work through this checklist, expect it to feel slow. You are retrieving vocabulary the chapters built and applying it deliberately. By the tenth deck you have run it on, most items are habit; the checklist now functions as a redundancy check that catches the day when the eye is tired or the deck was built under pressure. Eventually, the questions are reflexive enough that the checklist becomes a safety net rather than a process. None of this means you should stop running it. [Pronovost et al. (2006)](https://www.nejm.org/doi/full/10.1056/NEJMoa061115) documented sustained improvement only as long as the checklist was sustained; populations that stopped using it after the eye was built returned to baseline rates. The checklist is for tired you, not present you.

One discipline. If a question does not apply to a slide, the response is *"this question does not apply to this slide because [reason in framework vocabulary]."* The response is not *"skip."* A reader who can articulate why a question does not apply is using the checklist correctly. A reader who skips a question without reflection is using it as paperwork. This is the move that prevents Bosk's failure mode at the individual-reader level.

---

## 3. The Brutalist Slide Diagnostic Checklist

### Slide check (run per slide)

#### Ch 1 — Slideument

- [ ] **Who is this slide for, right now — me or the audience?** Live-deck slides serve the speaker's anchor function. Async-study slides serve the document function. One slide, one job.
- [ ] **If I removed the speaker from the room, would this slide alone teach the content?** If yes, it is a study artifact and is probably too dense to lecture from. If no, the notes field needs to carry what the slide can't.
- [ ] **Is anything on this slide a sentence I am about to say out loud?** If yes, cut it from the slide and move it to the notes field. Verbal-channel collision is a real cost.
- [ ] **Does the notes field contain what the slide can't?** An empty notes field on a sparse slide is half a deck.
- **DESIGN.md variables to update if these fail:** `body_text_density_max`, `notes_required_when_live_deck`, `deck_mode`.

#### Ch 2 — No Clear Hierarchy

- [ ] **Where does my eye go first? Is that where it should go?** If the eye lands on the wrong element, the size hierarchy is off.
- [ ] **How many size levels are there? Can I name each one's role?** Title, primary message, supporting detail. Three levels usually. If everything is the same size, there is no hierarchy.
- [ ] **Are elements that belong together physically close?** Gestalt proximity. Elements separated in space are perceived as unrelated.
- [ ] **Is whitespace grouping the right things?** Whitespace is the signal that says *"this is one thing."* It is not wasted space.
- [ ] **Is bold doing work, or is everything bold?** If everything is bold, nothing is.
- **DESIGN.md variables to update if these fail:** `font_size_scale`, `font_weight`, `spacing_rhythm`, `layout_grid`.

#### Ch 3 — Too Much Text

- [ ] **Which learning objective does each text element serve?** If the answer is "general context" or "it's interesting" — cut it.
- [ ] **Is any text repeating what the speaker will say aloud?** Redundancy violation. Move to notes field.
- [ ] **Is any text interesting but not essential?** Seductive detail. Coherence violation. Cut or move to notes.
- [ ] **Is the total word count above 50 for a live deck?** A working ceiling. Above 75 words, the slide is a document, not a slide.
- **DESIGN.md variables to update if these fail:** `body_text_density_max`, `max_words_per_slide`.

#### Ch 4 — The Wrong Visual Form

- [ ] **What is the relationship between the elements on this slide?** Comparison? Process? Trend? Part-to-whole? Cause-effect? Name the relationship.
- [ ] **Is that relationship best shown as text, diagram, chart, or table?** The decision matrix from Ch 4. Most relationships are not best shown as a bulleted list.
- [ ] **Would a reader understand the relationship faster with a visual?** If yes, the visual is the right form. Text is the fallback, not the default.
- [ ] **Is this a 3D chart?** Never. The depth axis adds visual complexity without information and distorts perception of magnitudes.
- **DESIGN.md variables to update if these fail:** `visual_form_default`, `no_3d_charts`.

#### Ch 5 — Color Is Doing Nothing (or Harm)

- [ ] **What does each color encode? Can I state it in one word?** Brand. Emphasis. Primary series. Negative. If the answer is "decoration" — cut it.
- [ ] **Does every text element pass 4.5:1 contrast against its background?** WCAG 2.1 AA standard. In projection environments with ambient light, target 7:1+.
- [ ] **Would a colorblind reader lose any information?** 8% of men have red-green color vision deficiency. A slide that uses red and green alone fails for 1 in 12 male students.
- [ ] **Is any color decorative — present for aesthetics, not meaning?** The signaling principle requires color to mean the same thing every time it appears.
- **DESIGN.md variables to update if these fail:** the six color tokens (`--color-white`, `--color-ink`, `--color-red`, `--color-secondary`, `--color-border`, `--color-ochre`), each with role and contrast ratio documented.

#### Ch 6 — The Textbook Figure on the Slide

- [ ] **Was this figure designed for print or for projection?** Print figures are high-resolution and studied closely. Slide figures are scanned at distance. Different media, different design requirements.
- [ ] **Can the student in the last row read every label?** The last-row test. If the label cannot be read from the back of the room, the label does not exist.
- [ ] **Is there a visual signal directing attention to the specific point this slide is making?** Color, arrow, callout box. The audience cannot study the figure — they can only follow where you point.
- [ ] **Have I removed labels that don't serve this slide's objective?** A figure labeled for a whole textbook chapter is over-labeled for a single lecture slide.
- [ ] **Does simplification distort the relationship between the remaining elements?** Simplification can cross into misrepresentation. Name the limit explicitly.
- **DESIGN.md variables to update if these fail:** `figure_label_font_size`, `figure_signaling_color`.

#### Ch 7 — Seductive Details

- [ ] **Which learning objective does this element serve?** If the answer is "it's interesting" or "it motivates students" or "it provides context" — it is a seductive detail.
- [ ] **Is it interesting without being essential?** Harp & Mayer's coherence violation. Cut it or move it to notes.
- [ ] **Would removing it make the core content clearer?** Usually yes. The diversion mechanism is asymmetric — seductive details hurt more than they help.
- [ ] **Is it appearing early in the deck where damage is highest?** Effect is strongest when seductive details appear in the opening, when students have low prior knowledge.
- **DESIGN.md variables to update if these fail:** `notes_field_carries_background`, `opening_slide_constraints`.

### Deck check (run once per deck)

#### Ch 8 — The Deck That Covers but Doesn't Teach

- [ ] **Does the deck open with a problem or question — or with a definition?** A deck that opens with definitions has skipped the hook.
- [ ] **Are concepts in dependency order: prerequisites before complex ideas?** Each concept before the one that depends on it.
- [ ] **Is there a consolidation moment before the 20-minute mark?** Working memory saturates around 15–20 minutes. A 50-minute lecture needs at least two consolidation moments.
- [ ] **Is this deck organized around the textbook's structure or the learner's build?** Coverage and teaching are different operations.
- **DESIGN.md variables to update if these fail:** `deck_opening_convention`, `retrieval_prompt_template`, `chunk_size_minutes`.

#### Ch 9 — Live Deck vs. Study Artifact

- [ ] **What is this deck for: live delivery or async study?** This is a use question, not a design question. Design follows the decision.
- [ ] **If live: is the text minimal enough that students won't read instead of listen?** Roughly 30–50 words per slide; not more than 75.
- [ ] **If async: does the slide carry enough explanation without a speaker?** The slide is the whole instructional artifact; it must teach alone.
- [ ] **Is the notes field populated for whichever mode this isn't?** Either the slide carries the explanation (async) or the notes field does (live). Both rarely.
- **DESIGN.md variables to update if these fail:** `deck_mode` (live | async), `notes_field_role` (script | study | discussion).

#### Ch 10 — The Headline That Says Nothing

- [ ] **Is the headline a claim or a label?** A claim is a sentence with a verb that asserts something. A label is a noun phrase that names the subject.
- [ ] **Could a student leave this slide with a specific thought in their head?** If the only thought they could leave with is "the slide was about X," the headline has done no teaching work.
- [ ] **Does the body provide visual evidence for the headline's claim?** A diagram, chart, labeled image, annotated comparison — not a vertical list of fragments.
- [ ] **Could I summarize this slide in one sentence to a colleague in the hallway?** That sentence is the assertion. If you cannot summarize the slide in a sentence, the slide does not know what it is claiming.
- [ ] **Is this a teaching slide or a reference slide?** Teaching slides default to assertions. Reference slides (agenda, glossary, citation slide) correctly use labels.
- **DESIGN.md variables to update if these fail:** `headline_must_assert`, `headline_max_words`, `reference_slide_types`.

#### Ch 11 — Owning Your DESIGN.md

- [ ] **Can I explain every variable in my DESIGN.md in one sentence?** The sentence is the decision. A variable without a one-sentence justification is still a default.
- [ ] **Is each decision traceable to a principle from cognitive science or visual design?** A justification that lives outside the framework ("I like it better") is not yet a decision.
- [ ] **Are my reference-slide conventions named separately from my teaching-slide conventions?** A course with multiple slide types needs the DESIGN.md to acknowledge them.
- [ ] **When the system generated a slide I disliked, did I update DESIGN.md or did I tweak the slide?** The slide tweak is the per-slide fix. The DESIGN.md update is the rule.

---

## 4. The deck-level check

These are the questions that apply across the deck, not to individual slides. Run them once per deck after the per-slide pass.

- [ ] **D1. What is this deck for?** Live delivery, async study, or hybrid with notes field populated. A deck that has not answered this is a slideument waiting to happen.
- [ ] **D2. Is the deck's arc legible from the headlines alone?** Read just the headlines, top to bottom. Do they tell the argument of the lecture? If they read as a list of topics, the deck has labels rather than claims.
- [ ] **D3. Is there at least one consolidation moment before the 20-minute mark, and another before the deck closes?** Working memory needs to discharge before it can take on more.
- [ ] **D4. Does any single slide carry the deck's central claim?** The deck without a load-bearing slide has no spine. Find that slide. If you cannot find it, the deck does not have a thesis.
- [ ] **D5. If a faculty colleague glanced through the deck cold, would they know the course it belongs to?** If the deck reads as generic, the DESIGN.md has not been owned. Run Chapter 11's audit.

---

## 5. The Brutalist prompt for a full deck audit

Paste this into the Brutalist system. It runs the checklist against the current deck and reports failures by chapter category, proposing DESIGN.md updates where the same item fails on multiple slides.

```
Audit this deck against the Brutalist diagnostic checklist.

For each slide, check the per-slide items from Chapters 1 through 11 (the
"Slide check" sections of Chapter 12). For each item, report PASS, FAIL,
or N/A. Where N/A, state the reason in framework vocabulary.

For the deck overall, check items D1 through D5 from the "deck-level
check" section.

Group failures by chapter category. When the same item fails on more than
three slides, propose a DESIGN.md update that would fix the class of
failure rather than per-slide fixes.

For each proposed DESIGN.md update, include:
1. The variable name (or proposed name if it does not yet exist).
2. The change (from / to).
3. A one-sentence rationale in framework vocabulary.

Return the audit as a structured report: PER-SLIDE FAILURES, DECK-LEVEL
FAILURES, PROPOSED DESIGN.md UPDATES. Do not modify the deck or the
DESIGN.md without confirmation.
```

Two things to notice about this prompt. It does not ask the system to *fix* anything — it runs the diagnostic and proposes the systemic fix. The reader stays in the loop on whether the proposed DESIGN.md update is correct, which is the discipline of Chapter 11 applied to Chapter 12. And the threshold for proposing a DESIGN.md update is "more than three slides fail the same item." This is the killer-item heuristic from Gawande's checklist criteria: if the failure is one-off, fix the slide; if the failure is structural, fix the rule. The reader who tweaks the DESIGN.md for every per-slide failure produces a brittle file. The reader who tweaks the slide for every structural failure produces a brittle deck. The threshold separates these.

---

## 6. When to stop using the checklist

Never. But what you do with it changes.

The first three or four decks: read each question, retrieve the relevant chapter vocabulary, apply it deliberately. The checklist is slow. You will find failures that surprise you — items the eye missed because the eye was new. Each failure is the diagnostic vocabulary getting cashed out into actual seeing.

By the tenth deck or so: most questions are answered before you read them. You glance at the headline of each slide and your eye does the assertion-or-label test reflexively. The slide hierarchy fires the eye-flow question without prompting. The seductive-details diagnostic is already running in the background while you build. The checklist is no longer a process. It is the redundancy check that catches the slides you built at 11 p.m. on a Sunday, when the eye was tired and the defaults crept back in.

This is the familiarity gradient. It is not in the empirical literature for this specific case — I cannot point to a study calibrating it for self-administered diagnostic checklists — but it is consistent with the clinical evidence. Surgeons who have run the WHO checklist for years still run it ([Pronovost et al. 2006](https://www.nejm.org/doi/full/10.1056/NEJMoa061115); [Haynes et al. 2009](https://www.nejm.org/doi/full/10.1056/NEJMsa0810119)). The argument is the same. Internalization is the goal; the artifact is the safety net. The day you stop running the checklist because "I've got this" is the day the failures it caught return.

The position I take is this. The first read of the checklist proves the vocabulary was built. The hundredth read proves the vocabulary holds. Both are part of the practice. The book ends here, but the checklist does not.

## 7. What this checklist does not catch

The checklist is a diagnostic for the eleven failure modes the book has named. There are failures it cannot catch. Saying so is the discipline of [Bosk et al. (2009)](https://doi.org/10.1016/S0140-6736%2809%2961440-9) applied to this book — the visible artifact is not the whole intervention.

**Pedagogical misalignment.** The checklist catches whether the deck's opening is a hook or a definition (Ch 8). It does not catch whether the *learning objective* for the lecture is the right learning objective for the course. That is a backward-design question — *what should the student be able to do at the end of this lecture* — that no per-deck checklist can mechanize. The book has gestured at this in Chapter 8 without solving it, because solving it is the work of instructional design for an entire course, not a per-deck diagnostic.

**Voice mismatches with institutional brand and course identity.** Chapter 11 owns the question of whether the DESIGN.md reflects the faculty member's context. The checklist asks whether each variable is justified in framework vocabulary, but it cannot tell you whether the brown accent you chose actually fits your department's culture or whether your institution's brand committee will object to it. These are contextual judgments the checklist cannot substitute for.

**Audience misreads.** Some failures only show up in delivery. A slide that passes every per-slide item can still fall flat with a particular audience — maybe the analogy lands for engineers but not historians; maybe the cultural reference dates the speaker. The checklist runs at the artifact level. The audience-level test is the lecture itself. There is no shortcut.

**Decks built without the prior reading.** This is the Bosk failure mode. A faculty member who downloads this checklist without working through Chapters 1–11 will read the questions as vague and unanswerable. *"Is the headline a claim or a label?"* requires the vocabulary built in Chapter 10. *"Does the body provide visual evidence?"* requires Chapter 4. The questions are killer items only for a reader who has the vocabulary. Without the vocabulary, the checklist is paperwork. The chapter is honest about this and refuses to pretend otherwise. The slide-design checklist works as the tip of the iceberg. The iceberg is the book.

---

Eleven chapters built the eye. This page is the redundancy check.

Run it once per deck. Then ship.

---

**What would change my mind:** A study of self-administered diagnostic checklists in non-clinical, non-aviation skilled-professional contexts showing that the working-memory-offload argument does not generalize to artifact production — that the checklist either fails to improve outcomes or actively interferes with the development of the underlying judgment. The clinical and aviation evidence is strong; the inference to slide design is by structural analogy, not direct demonstration.

**Still puzzling:** The familiarity gradient (first read → tenth read → reflexive) is the chapter's pedagogical contribution and is consistent with the clinical evidence on sustained checklist use, but I do not have a study that calibrates how quickly internalization happens for self-administered diagnostic checklists or under what conditions it stalls. The chapter argues from first principles and from analogy. A direct study would either confirm or revise the gradient.

**Tags:** checklist-manifesto, Gawande, Pronovost, Haynes, do-confirm
