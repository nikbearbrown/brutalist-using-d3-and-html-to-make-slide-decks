# Chapter 10 — The Headline That Says Nothing

*Is the headline a topic label, or does it state the slide's claim?*

---

There is a slide in almost every academic deck that looks exactly like this. The title is **Results**. Below the title are three graphs. The speaker says, *As you can see in the middle panel, infection rates dropped by sixty-six percent.* They could not see it. They were looking at the other two graphs. Not because they are inattentive, but because the slide gave them no reason to look at the middle panel before anywhere else. The word "Results" tells them what category of thing is happening. It does not tell them what to look for, or why it matters, or what the slide is asserting.

Twelve slides earlier, the deck opened with **Introduction**. Below the title were three bullets paraphrasing the syllabus. The presenter said, *Today we'll talk about working memory and slide design.* The slide did not disagree. The slide did not agree either. It held the topic at arm's length.

In between was **Methodology**. Three bullets: *Approach. Data. Analysis.* The audience waited for the speaker to tell them what the approach was, what the data was, what the analysis was. The bullets were placeholders for sentences the speaker was about to say. Once said, the bullets became redundant. Before said, they said nothing.

Three slides. The same failure. The slide tells you what it is *about*. It does not tell you what to *think*.

There is a name for this failure, and the literature on it is unusually clean.

---

## The grammar of a headline

The distinction is grammatical before it is anything else.

A **label** is a noun phrase. *Methodology. The Calvin Cycle. Q3 Performance. Results.* Labels name the subject. They tell you what room you are in. They are correct as the headings of book chapters and the tabs of filing systems, because book chapters and filing systems are navigated over time, with the reader moving through them at their own pace, looking for things.

A **claim** is a complete sentence with a verb that asserts something. *We replicated three classical findings on a corpus ten times larger. The Calvin Cycle fixes carbon in three stages, each requiring ATP. Q3 revenue grew 23%, driven entirely by enterprise renewals. Infection rates dropped by sixty-six percent in the treatment group.* Claims tell you what to think. They tell you not just what the slide is about but what the slide is saying about it.

Same content, different grammar, completely different cognitive effect.

<!-- → [TABLE: side-by-side comparison of label vs. claim headlines for the same five slide topics — columns: "Topic", "Label headline (wrong)", "Claim headline (right)"; rows: Introduction, Methodology, Results, Discussion, Conclusion; the claim column should show full-sentence assertions that could stand alone as the slide's argument; caption: "The grammar is the diagnostic. Same content, different commitment."] -->

When a student reads a label headline, they know the topic. They have to reconstruct the claim from whatever is below it — parsing the bullets, interpreting the graphs, extracting the meaning. That reconstruction is work, and it comes out of the same finite budget of working memory that should be processing the actual content. The label has handed the budget over to finding the point before any budget is available to engage with it.

When a student reads a claim headline, they receive the assertion before the evidence. The claim pre-activates a schema — a slot in working memory for this specific thought — and the evidence below fills that slot. The student does not have to hunt for the point. It was handed to them in the first two seconds.

Richard Mayer's Cognitive Theory of Multimedia Learning makes this precise. Learning happens when a student selects relevant information, organizes it into coherent mental representations, and integrates it with prior knowledge. The label headline disrupts the first step. The student has no basis for selecting which elements of the body are relevant until they have first reconstructed the claim — which they were never explicitly given. The assertion headline hands the student the organizing frame before the evidence arrives, which is the order working memory can actually use.

---

## The experiment that settled it

Michael Alley and Kathryn Neeley at Penn State formalized this as the **assertion-evidence structure** in a 2005 paper in *Technical Communication*. Two rules. The headline is a single declarative sentence stating the slide's main message — not a phrase, not a label, not a topic name. The body is visual evidence for that headline: a diagram, a chart, a photograph, an annotated image, an equation. Not a bulleted list of sub-points.

The rule is clean. The empirical case for it is cleaner than most findings in educational research.

Jennifer Garner and Michael Alley ran a controlled experiment comparing the assertion-evidence structure against the default topic-header-plus-bullets structure. One hundred and ten undergraduate engineering students. Parallel slide sets covering identical content. The only variable was the headline and body structure — assertion-evidence on one side, topic-label-plus-bullets on the other. The assertion-evidence group showed superior comprehension, fewer misconceptions, lower self-reported cognitive load, and stronger recall on both immediate and delayed post-tests. An earlier paper by Garner, Alley, and colleagues found the advantage was largest for complex conceptual material — exactly the case academic lectures face. More recent work by Wolfe and colleagues extended this across computer science, medical, and engineering student populations and found the effect generalizes.

<!-- → [INFOGRAPHIC: schematic of how the assertion-evidence structure processes in working memory vs. topic-label-plus-bullets — left path (label): eye reads "Results" → working memory searches for claim → parses bullets/graphs → maybe reconstructs claim; right path (assertion): eye reads "Infection rates dropped 66%" → schema activated immediately → evidence below fills the schema; label both paths with the cognitive cost at each step; caption: "The label makes finding the point the reader's job. The claim does it for them."] -->

The mechanism, in one sentence: the headline gives the student a schema before they see the evidence, so they encode the evidence into the schema rather than hunting for one.

Cliff Atkinson arrived at the same prescription independently, from the other end — working with management consultants rather than engineers, developing what he called "Beyond Bullet Points" for business presenters. The convergence matters. Engineering professors at Penn State, management consultants at McKinsey, journalists writing nut grafs — they all face the same constraint, which is that audience working memory is the bottleneck, and they all arrive at the same solution, which is to lead with the claim. The prescription is not a stylistic preference. It is the solution to a structural problem in how human working memory processes information under time pressure.

---

## Why topic labels are the default

If assertion headlines are demonstrably better, why does every AI slide generator produce topic labels?

The answer is that AI slide tools are trained on slide decks, and academic slide decks predominantly use topic labels. The tool has learned the default. The default is the failure mode. Canva, Gamma, Beautiful.ai — all of them parse the section headings of the source material and copy them onto slides as titles, because that is what the training data looks like. When you ask for a methodology slide, you get a slide titled "Methodology." The tool is reproducing what it was shown, not what works.

This is the same problem as bullets as the default form: the tool is optimizing for the visual rhythm of slides without evaluating the cognitive function of the specific elements. A slide with a title and bullets looks complete. Completeness is what the tool can verify. Pedagogical function is not something the tool's training signal captures.

But the deeper reason topic labels persist is that they are easier to write, in a specific sense. A label requires no commitment. *Methodology* can go on the slide before you have decided what your methodology *is*, before you have figured out what it *shows*, before you know what claim you are making about it. The label is a placeholder for a decision that hasn't been made yet. A claim, by contrast, requires you to know what the slide is for. *We sampled 10,000 participants across six countries using stratified randomization.* That is a decision. That commitment might be uncomfortable if you are not sure yet whether it is the most important thing about your methodology. The label lets you defer. The assertion forces you to decide.

This is actually useful diagnostic information. When you cannot write an assertion headline for a slide, it is often because the slide does not yet know what it is claiming. That is a signal about the slide's readiness, not about your ability to write headlines. A slide that cannot produce an assertion may not be ready to exist. It may be two slides that need to be separated. It may be a reference slide — agenda, glossary, term list — where a label is genuinely the right form. Or it may be a slide that should be cut, whose content either belongs in the notes field or does not belong in the deck at all.

The assertion test is, among other things, a curation tool.

---

## What assertion headlines do to the deck

The change happens at the headline level, but its effects propagate through the whole deck.

When the lecture-opening Introduction slide becomes an assertion — *"This lecture will show that working-memory limits explain three failure modes in slide design"* — it does several things at once. It gives the rest of the deck somewhere to land. Every subsequent slide either advances the claim or extends it. The student receives the organizing frame for the lecture in the first ten seconds of attention, when prior knowledge is unattached and schema formation is most plastic. The opening slide is the highest-leverage real estate in the deck; a topic label wastes it.

When the Results slide becomes *Infection rates dropped 66% in the treatment group*, the three graphs lose their ambiguity. The student does not need to scan all three looking for the finding. The claim directed them to the middle panel before the speaker said a word. The visual hierarchy follows from the rhetorical hierarchy, because the claim named what matters and the body can now support it instead of containing it.

When the Methodology slide becomes *We replicated three classical findings on a corpus ten times larger*, the three sub-elements — Stroop, Loftus and Palmer, Tversky and Kahneman — become evidence rather than bullet points. They are no longer indexing sub-topics; they are labeled blocks of visual evidence supporting a specific claim. The student reads each one knowing what claim it supports.

There is a compounding effect here that is easy to miss. When every slide states its claim in its headline, the deck becomes readable without the speaker. A student who missed class can read the deck and extract the argument — not just the topics, the argument — because the claims are all in the headlines, in sequence. The deck becomes a sequence of claims rather than a sequence of topic labels. The logical structure is visible.

<!-- → [IMAGE: two versions of the same five-slide deck shown as thumbnail strips — top strip: label headlines (Introduction, Methodology, Results, Discussion, Conclusion); bottom strip: same five slides with assertion headlines; annotation showing that the bottom strip reads as a connected argument when scanned left to right, while the top strip reads as a table of contents; caption: "A deck of assertion headlines is an argument. A deck of label headlines is a table of contents."] -->

This is different from what the notes field accomplishes. The notes field carries the explanation; the assertion headline carries the claim. Together they produce a deck that works as a live lecture aid (assertion gives the student the frame; explanation is delivered verbally) and as a study artifact (assertion in the headline, explanation in the notes, visual evidence in the body). The assertion headline is what makes the two-artifact solution work cleanly.

---

## The limit of the rule

Two limits are worth naming.

The first is reference slides. An agenda slide is a reference slide. A glossary is a reference slide. A key-terms recap is a reference slide. These slides serve a navigation or lookup function, not a teaching function. Forcing assertions onto them produces awkward fictions. *The agenda for today is six items long* is not a useful headline. The rule is: teaching slides default to assertions, reference slides correctly use labels, and the difference between the two should be an explicit decision rather than a per-slide guess. Most decks have three to five reference slides out of fifty. The default is assertion; the exception is label; the exception should be named.

The second limit is the length ceiling. An assertion that runs to twenty words usually contains either two claims — which want two slides — or an unnecessary clause — which wants cutting. The practical ceiling is around twelve words. Not because twelve is a magic number, but because a headline that exceeds it is usually telling you something. Either the claim is genuinely too complex to state simply, in which case the slide may be trying to do two things; or the author is hedging, adding qualifications that belong in the body or the notes. The ceiling is diagnostic, not prescriptive. When the headline runs long, the question is not *how do I shorten this?* — it is *is this one slide or two, and what qualification am I hiding in the hedge?*

Short complete sentences do most of the work most of the time. *The proton gradient powers ATP synthase.* Six words. *We replicated three classical findings on a corpus ten times larger.* Twelve words, at the ceiling, and earns every one of them.

---

## Two honest disagreements

Two faculty members who have read everything above can still disagree. Naming where matters more than picking a side.

The first disagreement is about bullets in the body. Alley's strict assertion-evidence structure excludes bulleted lists from the body entirely — the body is visual evidence, which means a diagram, a chart, a labeled image, not a vertical list of text fragments. A more relaxed reading says that the crucial move is the assertion headline, and the body can contain labeled blocks of evidence in whatever form fits the content. The defensible position is that bullets are usually a tell that the author has not chosen a visual form. When the content is genuinely enumerative, labeled evidence blocks typically outperform bullets because they name what each block evidences; a diagram or chart typically outperforms both. But the position you can defend in framework vocabulary is: bullets only when the relationship is genuinely flat-list-shaped and no better visual form exists. The position you cannot defend is: bullets because they are the default.

The second disagreement is whether academic slides and academic papers should share a headline grammar. The most common faculty objection is that papers use section labels — Introduction, Methods, Results — and asking slides to use full sentences feels inconsistent with the conventions of academic writing. The objection is real and resolves once the artifacts are distinguished. A paper is read over time — minutes per page, often re-read, with the section header serving as a navigational anchor for a reader who has been following an argument for ten pages. A slide is scanned in three seconds. The reader has no prior context with this slide, no opportunity to re-read, and no way to navigate. Different reading conditions, different headline grammars. The label is correct for the section header of a paper. It is not correct for the title of a slide. The moment you name the artifact — paper header versus slide title — the disagreement dissolves, because the two forms are not doing the same job.

<!-- → [TABLE: paper section header vs. slide title comparison — columns: "Dimension", "Paper section header", "Slide title"; rows: reading distance, dwell time, reader controls pace, re-reading available, navigational role, correct headline grammar; caption: "Same information, different artifact, different grammar. Naming the artifact resolves the disagreement."] -->

---

## The test

The chapter is a long argument for one short test.

*Is the headline a claim or a label?*

A claim has a verb and asserts something. A label is a noun phrase that names the subject. The grammar is the diagnostic. Apply it to the next deck. Find the slides with topic labels for headlines. For each one, ask: what is this slide claiming? If you can answer the question, write the answer as the headline. If you cannot answer it, the slide does not yet know what it is claiming, and the right response is to ask whether the slide should be cut or split before it is rewritten.

Most of the time, the slides that fail the test are not poorly executed — they are poorly specified. The author knows what the slide is about but has not committed to what the slide is saying. The assertion headline is not a design fix. It is a commitment. The commitment is to have figured out, before the slide goes to the audience, what the slide is for.

Once you have the claim in the headline, the body usually knows what to do. The evidence organizes itself around something it is evidencing. The visual form follows from the claim. The slide stops being a hat rack and starts being an argument.

---

**What would change my mind:** A replication of Garner and Alley's experiment in an asynchronous study-artifact condition — slides read without a speaker — that finds the assertion-evidence advantage does not hold when the slide is the only source of explanation. The existing evidence is from live or recorded-lecture conditions, which is the strongest case for assertion headlines. The asynchronous case is plausibly assertion-favorable but is empirically thinner. A strong null there would narrow the prescription to live-lecture decks.

**Still puzzling:** I do not have a clean rule for the length ceiling on an assertion. The chapter sets twelve words as a working maximum, but the number is a convention, not a finding. The assertion-evidence literature is mostly silent on length thresholds. A defensible benchmark would require an empirical study I have not found.

---

## LLM Exercises

**Exercise 1 — Label audit**
Take any deck you have built or received. Paste the slide titles — just the titles, nothing else — to an LLM with this prompt: *"For each of these slide titles, classify it as a label (noun phrase naming a topic) or a claim (complete sentence asserting something). Count how many are labels and how many are claims. For each label, ask: what is this slide likely claiming? If you can infer a claim, write it as an assertion headline. If you cannot, flag the slide as 'claim not recoverable.'"* Use the output as a deck-level audit before the lecture.

**Exercise 2 — Assertion rewrite**
Choose three slides from your deck that currently have label headlines. For each slide, paste the title and the body content to an LLM with this prompt: *"Rewrite this slide's headline as a single declarative sentence — a claim, not a topic label. The headline should state what the body substantiates. Maximum 12 words. If the body does not contain a recoverable claim, say so explicitly rather than inventing one."* If the LLM cannot recover a claim from the body, treat that slide as a candidate for cutting or splitting.

**Exercise 3 — Opening slide diagnosis**
Paste your deck's first content slide (after any title slide) to an LLM with this prompt: *"This is the opening content slide of a lecture deck. Does the headline state a claim the rest of the lecture will substantiate, or does it announce a topic? If it announces a topic, rewrite it as an assertion that gives the rest of the deck somewhere to land. The rewritten headline should make a student reading only this slide know what argument they are about to follow."* Use the rewritten opening as the frame the deck is organized around.

**Exercise 4 — Reference slide classification**
Paste your full deck's slide titles to an LLM with this prompt: *"Classify each slide title as: (a) a teaching slide that should have an assertion headline, (b) a reference slide (agenda, glossary, key-terms list, section divider) where a label headline is correct, or (c) ambiguous. For category (a) slides that currently have label headlines, write the assertion. For category (b) slides, confirm the label is appropriate. For category (c) slides, ask: what is this slide's function — teaching something new or providing something for lookup?"* Use the classification to distinguish where the assertion rule applies.

**Exercise 5 — Deck argument extraction**
After rewriting your deck's headlines as assertions, paste all the new assertion headlines in sequence to an LLM with this prompt: *"Read these slide headlines in order. Do they form a coherent argument — each claim following from or building on the previous? Or are they a sequence of independent claims with no visible logical connection? If the latter, identify where the argument breaks and what connecting claim is missing between those two slides."* A deck of assertion headlines should read as an argument. If it does not, the deck has a sequencing problem the assertion rewrite has now made visible.

**Tags:** assertion-evidence, Alley, Garner, headline-grammar, label-vs-claim
