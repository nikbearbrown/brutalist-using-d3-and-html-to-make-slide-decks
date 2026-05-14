# Chapter 1 — The Slideument Problem

*Is this deck a speaker's anchor or an audience's document — and what happens when it tries to be both?*

---

There is a peculiar thing that happens when you build a slide deck the night before a lecture.

You are alone at your desk. You are the only person in the room. And in that solitude, you are making a decision — mostly without realizing you are making it — about whose attention the slide is asking for. Is it asking for yours, up at the front of the room tomorrow morning, needing an anchor to keep the explanation on track? Or is it asking for the students', who will read whatever appears on the screen while you talk?

The trap is that from your desk at eleven at night, both jobs feel like the same job. You are writing the ideas down. The ideas are the ideas. What else is there to decide?

Here is what there is to decide. Those two audiences need different things from the same rectangle of light. And a slide that tries to give both audiences what they need ends up giving neither audience what they need. It looks complete — that is the deceptive part — but it fails at the moment of use, twice, in two different ways.

This failure has a name. Garr Reynolds coined it in 2005: the *slideument*. A slide that is also trying to be a document. The name is ugly on purpose. The thing it names is ugly on purpose too — a compromise that looks like a solution and isn't.

I want to explain exactly why this happens, because the word alone is not enough. You could memorize "slideument = bad" and still produce one every time, because the mechanism that creates it is invisible from the author's seat.

---

## The machinery

Start with something called working memory. This is not a metaphor — it is the actual cognitive bottleneck that governs how much information your brain can process at one time. Working memory is small. It holds somewhere between three and seven chunks of information in any given moment, and crucially, it is divided into channels. There is a verbal channel — the one processing language, whether spoken or read. There is a visual-spatial channel — the one processing images, diagrams, spatial relationships. The two channels are somewhat independent, which is genuinely useful: a diagram and a narration can run in parallel without each one degrading the other. That is the core insight behind good multimedia instruction, established through decades of experiments by Richard Mayer and summarized in *Multimedia Learning* (now in its third edition, 2020).

But here is the problem. Text on a screen is processed through the *verbal* channel. Your voice is processed through the *verbal* channel. Both are language. And when two streams of language arrive at the same channel at the same time, they don't helpfully combine — they compete. One stream wins, usually the one that doesn't require any effort to follow, which is the screen. You become the radio playing while someone reads. Mayer calls this the Redundancy Principle: identical information delivered through narration and on-screen text does not reinforce learning. It degrades it, because the student's verbal channel is spending resources suppressing the stream they're not attending to.

This is not an aesthetic preference. It is a measurable cognitive cost. Mayer and Johnson (2008) showed it in controlled experiments: students given animation plus narration outperformed students given animation plus narration *plus* on-screen text. Adding text to the slide — text that duplicates what the speaker says — made learning *worse*.

<!-- → [INFOGRAPHIC: two-lane diagram of working memory — left lane labeled "verbal channel" showing both a text-on-screen icon and a speaker icon competing for the same lane with a collision marker; right lane labeled "visual-spatial channel" showing a diagram icon flowing cleanly through; caption: "The redundancy problem: both text and narration enter the same channel. One must be suppressed."] -->

So that is the cognitive mechanism. Now here is the structural cause Reynolds identifies: the slide whose author never decided what it was for.

A speaker's anchor is a sparse artifact. It holds a claim, a diagram, a single striking number — just enough to tell the speaker what comes next and give the audience something to look at that doesn't compete with the explanation being delivered out loud. The explanation lives in the speaker's head and the notes field. The slide gets out of the way.

A study document is a dense artifact. It holds enough prose to reconstruct the argument without anyone speaking. It might look like a textbook page. That is fine — if it is deployed as a textbook page, viewed in silence, where there is no narration for the verbal channel to conflict with.

The slideument is what you get when the author builds the dense artifact and then lectures from it. The slide carries the full explanation because the author wanted it to be usable for study. But then the speaker delivers the same explanation out loud. The verbal channel gets hit twice. The students read the slide while you talk. Two weeks later a student who missed class emails asking if they can study from the slides, and you realize the notes field is empty, the slide body has the explanation but buried in prose without the visual structure a study document needs, and the student should probably just read the textbook.

Both jobs. Neither done well. The compromise that looked like thoroughness was actually the absence of a decision.

<!-- → [TABLE: two-column comparison of speaker's deck vs. study document — rows: artifact density, slide body content, notes field content, failure mode when misused, who benefits; helps reader see these as genuinely different artifacts before the slideument is named as the failed hybrid] -->

---

## What the failure looks like

Consider a slide on oxidative phosphorylation — the final stage of aerobic respiration, where the cell makes the bulk of its ATP. An AI-generated deck might produce something like this as slide two:

<!-- → [IMAGE: rendered mockup of the slideument slide — topic-label title "Oxidative Phosphorylation" in large heading font, 87-word paragraph below it in normal body text, empty speaker notes pane visible at bottom; overlaid annotation arrows pointing to: (1) the topic-label title with callout "label, not claim", (2) the prose block with callout "87 words — speaker will say this out loud", (3) the empty notes pane with callout "nothing here"] -->

> **Oxidative Phosphorylation**
>
> Oxidative phosphorylation is the metabolic pathway in which the mitochondrion uses enzymes to oxidize nutrients, thereby releasing chemical energy used to produce adenosine triphosphate (ATP). The proton gradient established across the inner mitochondrial membrane drives ATP synthase, generating approximately 32 ATP per glucose molecule. This process, discovered by Peter Mitchell in 1961 (Nobel Prize, 1978), accounts for the majority of ATP produced during aerobic respiration in eukaryotic cells.

Eighty-seven words. A complete paragraph. Reading time roughly twenty-five seconds.

Now you stand up to lecture. You are going to explain oxidative phosphorylation. You are going to talk about the proton gradient, the inner mitochondrial membrane, how ATP synthase works like a rotor being driven by ions flowing through it. You are going to mention Mitchell because 1961 and a Nobel Prize make the timeline vivid. You are going to say that this step produces most of the cell's ATP — that glycolysis earlier in the process is almost irrelevant by comparison, ATP-yield-wise.

Every sentence you are planning to say is already on the slide.

The verbal channel collision begins the moment you open your mouth. Students have already read the slide — it took them twenty-five seconds — and now they are waiting for you to say something it doesn't already say. If you just read it back to them, you are giving them information they have already processed. If you try to go deeper, you are departing from the slide without them knowing you've departed, because the slide still looks complete.

And note what else is missing. The slide title is a topic label — "Oxidative Phosphorylation" — not an assertion. A label tells a student what region of biology this is. An assertion tells them what to think. "The proton gradient powers ATP synthase" is a claim students can hold in their head and check their understanding against. "Oxidative Phosphorylation" is a filing system.

The notes field is empty. No student who missed class will get the explanation from this deck. The slide is too dense to lecture from cleanly and too badly structured to study from efficiently. It is the complete failure that looks like thoroughness.

---

## What the repair looks like

Same content. Different architecture.

<!-- → [IMAGE: rendered mockup of the repaired speaker's anchor slide — full-sentence headline "The proton gradient powers ATP synthase." in heading font; below it, a simple diagram of the inner mitochondrial membrane with labeled H⁺ ions, ATP synthase rotor, directional arrow, and "~32 ATP per glucose" callout; notes pane at bottom filled with prose explanation text; annotation arrows: (1) headline callout "assertion, not label", (2) diagram callout "visual channel carries mechanism", (3) notes callout "verbal explanation lives here, not on the slide"] -->

The slide body carries one assertion as the headline: *The proton gradient powers ATP synthase.* Under it, a diagram: the inner mitochondrial membrane drawn simply, H⁺ ions queued on one side, ATP synthase as a labeled rotor, an arrow showing the ion flow, output labeled "~32 ATP per glucose."

That is the entire slide. The visual channel gets the mechanism. The verbal channel gets the speaker's explanation. The two channels run in parallel rather than colliding.

The notes field carries the prose: the full explanation of chemiosmosis, the Mitchell reference, the context about why this step is the high-yield step in aerobic respiration, a note for async students explaining where this fits in the pathway.

Now the slide *anchors* the lecture without replacing it. You can talk for ninety seconds about the diagram. You can dwell on why the proton gradient works as a battery, why evolution stumbled onto a rotor as the mechanism for capturing that stored charge, why the number 32 is approximate and what it depends on. None of that is on the slide. The slide says one thing and then gets out of your way.

The structural move is exactly what Reynolds describes: one source file, two products. The slide is the live-deck artifact. The slide-plus-notes export is the study artifact. The same file produces both. But you had to make the decision — this slide is the speaker's anchor, and the notes field carries everything else — before the file could produce either product cleanly.

That decision is what the slideument author never made.

---

## The asymmetry of detection

Here is something worth sitting with. From the author's desk at eleven at night, the slideument *feels* more complete than the fixed version. The slide with eighty-seven words of prose looks finished. The slide with one sentence and a diagram looks sparse, maybe underprepared. The notes field is invisible in the normal slide-editing view. The decision to move the explanation there feels like hiding the work, not organizing it.

This is the asymmetry that produces slideuments at scale. The failure mode is invisible to the person creating it, because the evaluation condition — lecturing from the slide, a student trying to study from it alone — is not available at the authoring moment. You only discover the slide was wrong in the room, or two weeks later in an email.

AI tools that generate slide decks make this worse by optimizing for the wrong signal. The model has been trained on millions of slides and knows what a "complete" slide looks like. It looks like the eighty-seven-word version. The model produces slideuments not because it is bad at slides but because it is very good at producing what slideuments look like. It has learned the surface and not the function.

The repair is to tell the tool what function each region of the slide serves — not just "less text" but *the headline is a claim, the body is a visual, the notes field carries the explanation*. With those constraints, the model has something to optimize against other than "completeness."

The prompt that encodes this:

---

*Rewrite this slide as a live-deck slide.*

*1. The headline asserts the slide's claim in ten words or fewer. It is a full sentence, not a topic label.*

*2. The slide body contains at most one visual element — a diagram, labeled image, chart, or short equation — and no prose paragraph.*

*3. Move the full explanation into the notes field. Expand it so a student reading the slide without the speaker present gets a complete explanation.*

*4. Identify any "interesting but not essential" details — dates, named researchers, historical asides — and move them to the end of the notes field under "Background."*

---

Two things to notice. First, the prompt specifies *what each region is for*, not just *how much text to include*. "Less text" produces a sparse slideument. "The headline is a claim, the notes field carries the explanation" produces a different architecture. Second, the fourth instruction names the seductive detail as a category — the Mitchell-1961 aside, the Nobel Prize, the discovery date — and gives it somewhere to go rather than just cutting it. The detail doesn't disappear; it migrates to where it belongs.

---

## The design principle underneath

Reynolds' insight is not really about PowerPoint. It is about the difference between a speaker's artifact and a document, and the question of whether you have decided which you are making.

The same principle explains why Tufte's criticism of NASA's Columbia accident slides lands so hard. The engineers' risk assessment was formatted as PowerPoint bullets. The information it contained — the actual engineering analysis, the uncertainty ranges, the structural reasoning — required a technical document to convey correctly. Forced into slide format, the hierarchy collapsed, the quantitative nuance disappeared into bullet indentation, and the people reviewing the slides didn't have what they needed to assess the risk. The slide format was not the weapon; the failure to match artifact type to information type was. [(Columbia Accident Investigation Board, Report Volume 1, 2003, Chapter 6.)](https://www.nasa.gov/columbia/home/CAIB_Vol1.html)

That is a catastrophic version of the same failure that produces your eleven-pm slide deck. The author knew the content. The author put the content somewhere. The somewhere was wrong for what the recipient needed to do with it.

The Redundancy Principle gives you the cognitive mechanism: verbal-channel collision degrades learning. The slideument concept gives you the structural diagnosis: the author didn't decide whose attention the slide was asking for. Together they give you a test you can run on any slide in under a minute.

<!-- → [INFOGRAPHIC: flowchart of the three diagnostic questions — each question is a diamond decision node: (1) "Is anything on this slide a sentence I'll say out loud?" → Yes: move to notes field; (2) "Would this slide teach the content without a speaker?" → Yes: you have a study document, not a live-deck slide; (3) "Does the notes field contain what the slide can't?" → No: the deck is half-finished; all Yes paths converge on "you have a slideument"] -->

**Is anything on this slide a sentence I am about to say out loud?** If yes, move it to the notes field.

**If I removed the speaker from the room, would this slide alone teach the content?** If yes, the slide is a study document and is probably too dense to lecture from. The notes field is not what makes it a study document — the slide body is. Decide: is this a live-deck slide or a study artifact? One job, not both.

**Does the notes field contain what the slide can't?** An empty notes field on a sparse slide is half a deck.

The answers tell you whether you have a slide or a slideument. The decision to fix it is the same decision the author didn't make the night before: who is this for, right now?

---

## What two instructors might argue about

Two faculty members can read this and reach honest disagreement. The vocabulary for arguing precisely rather than past each other:

Some lecturers prepare by typing every sentence they plan to say into the slide. The slide becomes a teleprompter. They argue: I lecture better when the words are in front of me; the students get the full content; the deck is also their study aid. Other lecturers treat the slide as an anchor for an explanation held in their head. They argue: the slide is what the audience looks at; if I read the slide I am redundant with myself; the explanation is what I bring.

Both are real positions held by working teachers. They produce different decks. The term for each: **speaker's deck** (low text, visual-dominant, notes field carries explanation) versus **audience's deck** (high prose density, slide body carries explanation, notes field may be empty). Neither is wrong as a use case. What is wrong is producing one and using it as both.

The second place of genuine disagreement: whether the notes field is enough, or whether study requires a separate document entirely. Reynolds endorses the populated notes field as the practical solution — one source file, two products. Tufte argues the notes field is not a technical document and never will be; the slide format imposes a hierarchy and a density constraint that distorts the kind of information a student needs to reconstruct an argument. Both positions are defensible. The notes-field path is the default here because most teaching contexts make it cheap; Tufte's prescription is the fallback when what you need is actually a textbook chapter, and the distinction between "here is what the lecture covered" and "here is the argument you need to be able to reconstruct" is real and worth naming before you decide.

---

## LLM Exercise

Paste any slide from a deck you have already made into a language model with this prompt:

*Read this slide. Tell me: (1) Is the headline a claim or a topic label? (2) Does the slide body contain any sentence the speaker would also deliver verbally? (3) Is the notes field empty? Then rewrite the slide as a speaker's anchor: headline as a full-sentence assertion of ten words or fewer, body as a single visual element described in plain text, notes field carrying the full explanation a student would need without the speaker present.*

Compare the original and the rewrite. The question is not which looks more finished. The question is which one creates verbal-channel collision the moment you open your mouth, and which one gets out of your way.

---

**What would change my mind:** A controlled study measuring slideument configuration against sparse-slide-plus-notes in actual lectures, with learning outcomes measured two weeks later, finding no significant difference. I am not aware of such a study. If one arrives, this chapter's prescription weakens, and the efficiency argument for slideuments — they take less time to produce — becomes harder to dismiss.

**Still unresolved:** I do not have a clean rule for how much the notes field needs to carry. "Enough that the student who missed class can follow the argument" is qualitative. A density target — words per slide, a heuristic about which sentence types must appear — is still missing from the literature I can name.

---

*A slide can have too much text for a different reason than slideument failure — sometimes the hierarchy just isn't clear enough to show the reader what matters. That's Chapter 2.*
