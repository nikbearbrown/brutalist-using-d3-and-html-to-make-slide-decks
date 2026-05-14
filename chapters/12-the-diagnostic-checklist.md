# Chapter 12 — The Diagnostic Checklist

*One reference page. Use it before every deck ships.*

---

On October 30, 1935, the prototype Boeing Model 299 crashed during a demonstration flight at Wright Field. Two of the five crew died. The investigation was short. The pilots had forgotten to release a control lock before takeoff. The aircraft was not too difficult to fly — one of the country's most experienced test pilots was at the controls. It was too complex to fly from memory alone, under the pressure of a demonstration, without any external scaffold for the steps that had to happen in order.

Boeing's response was the pre-flight checklist. A short, ordered list of items printed on a single card. With the checklist, the Model 299 went on to fly 1.8 million miles without an accident attributable to pilot oversight. Some thirteen thousand were built.

Atul Gawande, who spent a decade studying checklists in medicine and aviation before writing *The Checklist Manifesto*, is precise about what the checklist actually does. The pilots did not crash because they did not know to release the control lock. They knew. They crashed because the knowledge was not retrievable at the right moment, under pressure, when attention was elsewhere. The checklist offloads retrieval from working memory to a stable external artifact. The working memory is freed for the parts of the job that actually require judgment.

The clinical evidence runs the same argument. Pronovost and colleagues implemented a five-item central-venous-catheter checklist across 103 Michigan ICUs. Items as simple as: wash hands, use full sterile barriers, clean skin with chlorhexidine, avoid femoral insertion, remove unnecessary catheters. The median rate of catheter-related bloodstream infections fell from 2.7 per 1,000 catheter-days at baseline to zero within three months, sustained at 66% below baseline at 16 to 18 months. The Haynes WHO Surgical Safety Checklist study, run across eight hospitals in high-income and low-income settings, found in-hospital mortality dropped from 1.5% to 0.8% — a 47% reduction — and inpatient complications dropped from 11% to 7%.

<!-- → [CHART: two paired bar charts showing the Pronovost and Haynes results side by side — left pair: catheter infection rate before (2.7/1,000 days) and after (near 0) checklist implementation; right pair: surgical mortality before (1.5%) and after (0.8%); both charts labeled with the study name and the single intervention (checklist); caption: "The intervention was a card with five to nineteen items. The mechanism was working-memory offload, not new knowledge."] -->

The honest critique of this evidence arrived three months after Haynes. Bosk, Dixon-Woods, Goeschel, and Pronovost wrote in *The Lancet* that the checklists worked because they sat inside broader organizational change — empowered nurses, leadership commitment, data feedback loops. Deploy the checklist alone, without the surrounding work, and it becomes paperwork. "A technical solution to a cultural problem is likely to fail or to be resented." This matters here. The checklist in this chapter works for a reader who has worked through Chapters 1 through 11. Hand it to someone who has not read the book and it will read as forty arbitrary questions. The checklist is the visible artifact. The reading was the cultural change. Both are required.

---

## How the checklist works

Gawande names two checklist architectures. A *read-do* checklist is executed step by step: read the item, do the item, move to the next. A recipe is read-do. A *do-confirm* checklist runs after the task is complete: you build the thing, then run the checklist to confirm nothing was missed. A surgeon's pre-incision checklist is do-confirm. The choice depends on whether steps must occur in a fixed order (read-do) or whether the task is built fluently but mistakes creep in under cognitive load (do-confirm).

This checklist is do-confirm. Build the deck. Then run the checklist before shipping. The questions are framed as diagnostics — *is the headline a claim or a label?* — rather than instructions — *write a claim headline*. Running the checklist before each slide would be slower than building intuition. Running it after the deck exists catches the failures the intuition missed.

There is a familiarity gradient to expect. The first few times through, the checklist will feel slow. You are retrieving the vocabulary the chapters built and applying it deliberately to an artifact in front of you. By the tenth deck, most questions are answered before you finish reading them. The checklist has become the redundancy check it is meant to be — the thing that catches the slides you built at 11 p.m. when the defaults crept back in. The goal is internalization; the artifact is the safety net.

One discipline. If a question does not apply to a slide, the response is *this question does not apply to this slide because [reason in framework vocabulary]*, not *skip*. A reader who can articulate why a question does not apply is using the checklist correctly. A reader who skips without reflection is using it as paperwork, which is Bosk's failure mode at the individual level.

---

## The checklist

### Per-slide items

**Chapter 1 — Slideument**

Who is this slide for right now — me or the audience? A live-deck slide serves the speaker's anchor function. An async-study slide serves the document function. One slide, one job.

If I removed the speaker from the room, would this slide alone teach the content? If yes, it is a study artifact and is probably too dense to lecture from. If no, the notes field needs to carry what the slide cannot.

Is anything on this slide a sentence I am about to say out loud? If yes, cut it from the slide and move it to the notes field. Verbal-channel collision is a real cost, not an aesthetic preference.

Does the notes field contain what the slide cannot? An empty notes field on a sparse slide is half a deck.

---

**Chapter 2 — No Clear Hierarchy**

Where does my eye go first, and is that where it should go? If the eye lands on the wrong element, the size hierarchy is broken.

How many type sizes are on this slide, and can I name what each one is for? Title, primary message, supporting detail. If everything is the same size, there is no hierarchy. If everything is bold, nothing is.

Are elements that belong together physically close? Proximity is the signal that says *these are one thing*. Elements separated in space are perceived as unrelated.

Is whitespace grouping the right elements? White space is syntax, not wasted space.

---

**Chapter 3 — Too Much Text**

Which learning objective does each text element serve? If the answer is "general context" or "it's interesting," cut it.

Is any text repeating what the speaker will say aloud? Redundancy violation. Move it to the notes field.

Is any text interesting but not essential? Seductive detail. Coherence violation. Cut it or move it to notes.

Is the total word count above 50 for a live deck? A working ceiling. Above 75 words, the slide is a document in disguise.

---

**Chapter 4 — The Wrong Visual Form**

What is the relationship between the elements on this slide? Comparison? Process? Trend? Part-to-whole? Cause-effect? Name the relationship before choosing the form.

Is that relationship best shown as text, diagram, chart, or table? Most relationships are not best shown as a bulleted list. The bulleted list is the zero-decision form — what you get when you have not asked what the content is actually shaped like.

Would a reader understand the relationship faster with a visual? If yes, the visual is the right form. Text is the fallback, not the default.

Is this a 3D chart? Never. The depth axis adds visual complexity without information and distorts magnitude perception.

---

**Chapter 5 — Color Is Doing Nothing or Harm**

What does each color on this slide encode? Can I state it in one word? Brand. Emphasis. Primary series. Warning. If the answer is "decoration," remove it.

Does every text element pass 4.5:1 contrast against its background? WCAG 2.1 AA standard. In projection environments with ambient light, target 7:1 or higher.

Would a colorblind reader lose information? Eight percent of men have red-green color vision deficiency. A slide that relies on red and green alone fails for one in twelve male students.

Is any color present for aesthetics rather than meaning? The Signaling Principle requires color to mean the same thing every time it appears. A color that means nothing is a cue that misleads.

---

**Chapter 6 — The Textbook Figure on the Slide**

Was this figure designed for print or for projection? Print figures are studied at fourteen inches over several minutes. Slide figures are scanned at fifty feet in three seconds. Different media, different design requirements.

Can the student in the last row read every label? If the label cannot be read from the back of the room, the label does not exist for most of the class.

Is there a visual signal — accent color, arrow, callout — directing attention to the specific point this slide is making? The audience cannot study the figure. They can only follow where you point.

Have I removed labels that do not serve this slide's objective? A figure labeled for a whole textbook chapter is over-labeled for a single lecture slide.

Does any simplification I applied distort the relationships between the remaining elements? Simplification can cross into misrepresentation. Name the limit explicitly before shipping.

---

**Chapter 7 — Seductive Details**

Which learning objective does this element serve? If the answer is "it's interesting" or "it motivates students" or "it provides context," it is a seductive detail.

Is it interesting without being essential? Harp and Mayer's coherence violation. Cut it or move it to notes.

Would removing it make the core content clearer? Usually yes. The seductive-detail damage is asymmetric — they hurt more than they help.

Is it appearing early in the deck, where prior knowledge is lowest and the damage is highest? The effect is strongest in the opening slides, when the student has not yet built the schema that would let them file the interesting detail correctly.

---

### Per-deck items

**Chapter 8 — The Deck That Covers but Doesn't Teach**

What should the student be able to *do* after this lecture? State it with an action verb — explain, apply, analyze, compare, evaluate, produce. If the answer is "be familiar with," the deck has no destination.

Does the deck open with a problem or question, or with a definition? A deck that opens with definitions has skipped the hook.

Are concepts in dependency order — prerequisites before the ideas that depend on them?

Is there at least one consolidation moment before the 20-minute mark, and another before the deck closes? Working memory needs to discharge before it can take on more.

Is this deck organized around the textbook's structure, or around the build the learner needs? Coverage and teaching are different operations.

---

**Chapter 9 — Live Deck vs. Study Artifact**

What is this deck for — live delivery, async study, or hybrid? Design follows from this decision. A deck that has not answered it is a slideument waiting to happen.

If live: is the text minimal enough that students will listen instead of read? Roughly 30 to 50 words per slide as a working ceiling.

If async: does the slide carry enough explanation without a speaker? The slide is the whole instructional artifact. It must teach alone.

Is the notes field populated for whichever mode this deck is not? Either the slide carries the explanation (async) or the notes field does (live). Rarely both on the same slide.

---

**Chapter 10 — The Headline That Says Nothing**

Is the headline a claim or a label? A claim is a sentence with a verb that asserts something. A label is a noun phrase that names the subject. Different grammars do different jobs.

Could a student leave this slide with a specific thought in their head? If the only thought available is "the slide was about X," the headline did no teaching work.

Does the body provide visual evidence for the headline's claim? A diagram, a chart, a labeled image, an annotated comparison — not a vertical list of noun fragments.

Could I summarize this slide in one sentence to a colleague in the hallway? That sentence is the assertion. If you cannot produce it, the slide does not know what it is claiming.

Is this a teaching slide or a reference slide? Teaching slides default to assertions. Reference slides — agenda, glossary, section divider — correctly use labels. Name the type before challenging the headline.

---

**Chapter 11 — Owning Your DESIGN.md**

Can I explain every variable in my DESIGN.md in one sentence? The sentence is the decision. A variable without a one-sentence justification is still a default, still owned by the tool.

Is each decision traceable to a principle from cognitive science or visual design? A justification that lives outside the framework — "I like it better" — is not yet a decision.

Are reference-slide conventions named separately from teaching-slide conventions? A course with multiple slide types needs the DESIGN.md to acknowledge them.

When the system generated a slide I disliked, did I update DESIGN.md or did I tweak the slide? The slide tweak fixes one slide. The DESIGN.md update fixes the class of failure. Structural failures want structural fixes.

---

## The deck-level check

Run these once per deck, after the per-slide pass.

<!-- → [TABLE: the five deck-level checks as a quick-reference table — columns: "Item", "Question", "Pass condition", "Fail signal"; rows for D1 through D5; the table should be formatted so an instructor can run through it in under two minutes without re-reading the prose above] -->

**D1.** What is this deck for? Live delivery, async study, or hybrid with notes field populated. A deck that has not answered this is a slideument waiting to happen.

**D2.** Is the deck's arc legible from the headlines alone? Read just the headlines, top to bottom. Do they tell the argument of the lecture? If they read as a list of topics, the deck has labels rather than claims.

**D3.** Is there at least one consolidation moment before the 20-minute mark, and another before the deck closes? Working memory needs to discharge before it can receive more.

**D4.** Does any single slide carry the deck's central claim? The deck without a load-bearing slide has no spine. Find that slide. If you cannot find it, the deck does not have a thesis.

**D5.** If a colleague glanced through the deck cold, would they know the course it belongs to? If the deck reads as generic, the DESIGN.md has not been owned.

---

## What this checklist does not catch

The checklist is a diagnostic for the eleven failure modes this book has named. There are failures it cannot catch.

**Pedagogical misalignment.** The checklist catches whether the deck opens with a hook or a definition. It does not catch whether the learning objective for the lecture is the right objective for the course. That is a backward-design question — *what should the student be able to do at the end of this lecture?* — that no per-deck checklist can mechanize. Chapter 8 gestured at this without solving it. Solving it is the work of instructional design for an entire course.

**Audience misreads.** Some failures only show up in delivery. A slide that passes every checklist item can still fall flat with a particular audience — the analogy lands for engineers but not historians; the cultural reference dates the speaker. The checklist runs at the artifact level. The audience-level test is the lecture itself. There is no shortcut.

**Decks built without the prior reading.** This is Bosk's failure mode at the reader level. A faculty member who downloads this checklist without reading Chapters 1 through 11 will find the questions vague and unanswerable. *"Is the headline a claim or a label?"* requires the vocabulary built in Chapter 10. *"Does the body provide visual evidence?"* requires Chapter 4. The questions are killer items only for a reader who has the vocabulary. Without the vocabulary, the checklist is paperwork. The chapter is honest about this rather than pretending otherwise.

---

## When to stop using the checklist

Never. But what you do with it changes.

The first few decks: read each question, retrieve the relevant chapter vocabulary, apply it deliberately. The checklist is slow. You will find failures that surprise you — slides the eye missed because the eye was new. Each failure is the vocabulary being cashed out into actual seeing.

By the tenth deck: most items are answered before you finish reading the question. The eye does the assertion-or-label test reflexively. The hierarchy diagnostic fires without prompting. The checklist is no longer a process. It is the redundancy check that catches the slides built at 11 p.m. on a Sunday, when the defaults crept back in.

<!-- → [DIAGRAM: a timeline or arc showing the familiarity gradient — x-axis: number of decks audited (1 to ~10+); y-axis: time to complete checklist and proportion of items answered reflexively vs. deliberately; two curves: "time per audit" declining, "reflexive answers" rising; annotation at the right end: "checklist becomes safety net"; caption: "The goal is internalization. The artifact is the net you fall into when the eye is tired."] -->

The surgeons who have run the WHO checklist for years still run it. The argument is the same here. Internalization is the goal; the artifact is the safety net. The day you stop running the checklist because "I've got this" is the day the failures it caught return.

Eleven chapters built the eye. This page is the redundancy check.

Run it once per deck. Then ship.

---

**What would change my mind:** A study of self-administered diagnostic checklists in non-clinical, non-aviation skilled-professional contexts showing that the working-memory-offload argument does not generalize to artifact production — that the checklist either fails to improve outcomes or actively interferes with the development of the underlying judgment. The clinical and aviation evidence is strong; the inference to slide design is by structural analogy, not direct demonstration.

**Still puzzling:** The familiarity gradient — first read to reflexive — is consistent with the clinical evidence on sustained checklist use, but I do not have a study that calibrates how quickly internalization happens for self-administered diagnostic checklists applied to slide design, or under what conditions it stalls. The chapter argues from first principles and from analogy. A direct study would either confirm or revise the gradient.

---

## LLM Exercises

**Exercise 1 — Single-slide audit**
Choose any slide from your current deck. Paste its full content — title, body, any figure description — to an LLM with this prompt: *"Run this slide through the Brutalist per-slide diagnostic checklist. For each of the seven chapter categories (Slideument, Hierarchy, Too Much Text, Wrong Visual Form, Color, Textbook Figure, Seductive Details), assess: Pass, Fail, or N/A. Where N/A, state the reason. Where Fail, state which principle is violated and what the fix is. Do not fix the slide — only diagnose it."* Compare the LLM's findings to your own reading of the same slide.

**Exercise 2 — Deck-level arc check**
Extract just the slide headlines from an existing deck and paste them in sequence to an LLM with this prompt: *"Read these slide headlines in order. Answer the D2 deck-level check: do the headlines, read top to bottom, form a coherent argument — each claim following from or building on the previous? Or are they a sequence of independent topics with no visible logical thread? If the latter, identify where the argument breaks and name what connecting claim is missing between those two slides."* If the headlines do not form an argument, run the /write or /essay command on the deck's destination before rebuilding.

**Exercise 3 — Systematic failure diagnosis**
After running the full per-slide checklist on a deck of ten or more slides, paste the list of failures to an LLM with this prompt: *"Here are the checklist failures I found across this deck, organized by slide number and chapter category: [list]. Identify any patterns — failure categories that appear on more than three slides. For each pattern, propose a DESIGN.md update that would fix the class of failure rather than requiring per-slide fixes. For each proposed update, state: the variable name, the change (from / to), and a one-sentence rationale in framework vocabulary."* Use the proposed updates as candidates for your DESIGN.md, not automatic changes.

**Exercise 4 — Do-confirm practice**
Build a new slide on any topic without consulting the checklist during construction. When finished, run the per-slide items for Chapters 1 through 7 on the slide and record which items you passed and which you failed. Then ask an LLM: *"I built this slide without consulting any checklist. Here is the slide and here are my self-assessed checklist results: [results]. Do you agree with my self-assessment? For any item I marked Pass that you would mark Fail, explain what I missed."* Repeat on three consecutive slides and look for the items you consistently miss — those are the failure modes your intuition is not yet catching.

**Exercise 5 — Checklist calibration**
After using the checklist on ten or more decks, reflect on the familiarity gradient by asking an LLM: *"Here are the checklist items I find myself answering automatically (without reading the question) and the items that still require deliberate retrieval: [list both]. Based on this pattern, which failure modes have I internalized and which are still external to my intuition? For the items still requiring deliberate retrieval, suggest a one-sentence heuristic I could apply during slide construction — before the do-confirm pass — that would catch that failure mode earlier."* Use the heuristics as build-time prompts rather than only post-build diagnostics.

**Tags:** checklist-manifesto, Gawande, Pronovost, Haynes, do-confirm
