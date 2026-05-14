# Chapter 10 — The Headline That Says Nothing

> Is the headline a topic label, or does it state the slide's claim?

---

## 1. The feeling

The slide is titled **Introduction**. Below the title are three bullets. They paraphrase the syllabus. The presenter walks past the projector and says, *Today we'll talk about working memory and slide design.* The slide does not disagree. The slide does not agree either. It is a hat rack, not a claim.

Two slides later, the deck reaches **Methodology**. Three bullets: *Approach. Data. Analysis.* The audience reads the three words. They wait for the speaker to tell them what the approach is, what the data is, what the analysis is. The bullets do not advance them; the speaker does. The bullets are a placeholder for sentences the speaker is about to say. Once said, the bullets become redundant. Once redundant, they were never load-bearing.

Twelve slides later, the deck reaches **Results**. The slide shows three graphs and the word *Results*. The audience scans the three graphs trying to figure out which one carries the finding. The speaker says, *As you can see in the middle panel, infection rates dropped by sixty-six percent.* They could not see it. They were looking at the other two graphs.

Three slides, three different topics, the same failure. The slide tells you what it is *about*. It does not tell you what to *think*. You leave the deck having heard a list of topics that were covered. You leave with no claim in your head.

That feeling has a name, and the literature on it is unusually clean.

## 2. The two diagnostic questions

Ask both, in this order, every time.

**From cognitive science:** *Could a student walking past the projector for three seconds know what this slide asserts?* If the only thing they could pick up in three seconds is the topic name — "Methods," "Q3 Performance," "Cognitive Load Theory" — the slide has handed the working-memory budget over to *figuring out what the slide is about*. None of that budget is available to integrate the actual content. The signal-to-noise ratio at the headline level is zero.

**From visual design:** *Is the headline a topic label, or does it state the slide's claim?* This is the test that resolves the diagnostic. A label is a noun phrase that names the subject. *Mitochondrial Function. The Calvin Cycle. Q3 Performance.* A claim is a complete sentence that asserts what the slide will substantiate. *Mitochondria generate ATP through oxidative phosphorylation across the inner membrane. The Calvin Cycle fixes carbon in three stages, each requiring ATP. Q3 revenue grew 23%, driven entirely by enterprise renewals.* Same content, different headline grammar. The label tells you what room you are in. The claim tells you what is happening in it.

## 3. The principle named

Plain language first: **every teaching slide should state its claim in its headline, and the slide body should provide the evidence.**

In framework vocabulary, this is the **assertion-evidence (AE) structure**, formalized by Michael Alley and Kathryn Neeley at Penn State Engineering and articulated in [*Technical Communication* (Alley & Neeley, 2005)](http://writing.engr.psu.edu/2005_alley_neeley.pdf). It has two rules. First, the headline is a single declarative sentence stating the slide's main message — not a phrase, not a label, not a topic name. Second, the body is *visual evidence* for that headline — a diagram, a chart, a photograph, an annotated image, an equation — and not a bulleted list of sub-points.

The cognitive logic runs cleanly through Mayer's Cognitive Theory of Multimedia Learning ([*Multimedia Learning*, 3rd ed., Mayer 2020](https://www.cambridge.org/core/books/multimedia-learning/E64FFFAB9D984ECCFEA38D63A9DAA4E5)). The assertion pre-activates the schema the evidence will be integrated into. The student receives the claim first, then the evidence, in the order working memory can actually use. The traditional topic-header structure inverts this: the student receives a topic label, then a list of fragments, and has to reconstruct the assertion themselves from the body. That reconstruction comes out of the same finite working-memory budget that should be processing the content.

Cliff Atkinson's *Beyond Bullet Points* ([3rd ed., Microsoft Press, 2018](https://www.cliffatkinson.com/beyond-bullet-points)) is the popular-press version of the same idea, developed independently for business presenters. The convergence matters. Engineering professors at Penn State and management consultants at McKinsey and reporters writing nut grafs all face the same constraint — audience working memory is the bottleneck — and arrive at the same prescription. Lead with the claim. Then show the evidence.

The empirical case is also unusually clean. [Garner & Alley (2013)](https://writing.engr.psu.edu/ae_comprehension.pdf) compared the AE structure against the default topic-header-plus-bullets structure on 110 undergraduate engineering students with parallel slide sets covering identical content. The AE group showed superior comprehension, fewer misconceptions, lower self-reported cognitive load, and stronger delayed recall on both immediate and delayed post-tests `[verify exact effect size and p-value from PDF]`. The earlier [Garner et al. (2011)](https://peer.asee.org/assertion-evidence-slides-appear-to-lead-to-better-comprehension-and-recall-of-more-complex-concepts.pdf) ASEE paper found the AE advantage was *largest* for complex conceptual material — exactly the case academic lectures face. [Wolfe et al. (2024)](https://journals.sagepub.com/doi/10.1177/00472816231169433) `[verify DOI 10.1177/00472816231169433]` extends the work across computer science, medical, and engineering student populations and finds the effect generalizes.

The mechanism is one sentence: the headline gives the student a schema before they see the evidence, so they encode the evidence into the schema rather than hunting for one.

## 4. Bad example

Here is the slide an AI tool produced when you asked Gamma to make a deck on a research talk. The slide is the methodology slide, the second slide in.

```html
<!-- BAD: topic-label headline. Three bullet fragments that the speaker will
     paraphrase verbatim. No claim. No visual evidence. The slide is a hat rack. -->
<section class="slide">
  <h1>Methodology</h1>
  <!-- Topic label. Noun, no verb. The student sees "Methodology" and learns
       that the slide is about methodology. They learn nothing about *what*
       the methodology is or *why it matters*. -->

  <ul>
    <li>Approach</li>
    <li>Data</li>
    <li>Analysis</li>
  </ul>
  <!-- Three more noun fragments. Each fragment is a slot the speaker fills
       verbally. Once the speaker fills them, the bullets are redundant.
       Before the speaker fills them, the bullets say nothing. The slide is
       inert in both states. -->

  <div class="notes" style="display:none">
    <!-- empty -->
  </div>
</section>
```

What fails, point by point. The headline is a label — "Methodology" — that tells the audience the topic of the slide and nothing more. The three bullets are noun phrases that index sub-topics rather than claiming anything about them. The student who walks past the projector for three seconds learns that there is a methodology slide. They do not learn what the methodology *is* or what it *did*. The slide is structurally a slot for the speaker's narration; remove the speaker and the slide says nothing.

This is not a quirk of one bad deck. It is the default output of every AI slide generator on the market. Canva Magic Design, Gamma, Beautiful.ai, tome.app — they parse the section headings of the source material and copy them onto slides as titles. The pattern is consistent because the assumption is consistent (the section heading is the slide title), and the assumption is exactly what AE rejects. `[verify by running current tool comparison; outputs change quarterly]`

The slide *looks* complete. It has a title. It has bullets. It has the visual rhythm of an academic slide. That visual completeness is the trap. The bullets are filler. The title is a placeholder. The slide is a label pretending to be a claim, and academic readers — having seen ten thousand such slides — usually do not notice. The deck's central failure mode is that nothing about it stands out as broken.

## 5. Good example

Same content, rebuilt as an AE slide.

```html
<!-- GOOD: full-sentence assertion headline. Body is visual evidence —
     three short labeled facts the student can read and the speaker
     can elaborate. The student leaves with a *claim* in their head. -->
<section class="slide">
  <h1>We replicated three classical findings on a corpus ten times larger.</h1>
  <!-- Full-sentence assertion. Subject + verb + object. Declarative. The
       student who reads only this leaves with a specific thought:
       "they replicated three findings on a bigger dataset." That thought
       is the schema everything below will hang from. -->

  <div class="evidence-grid">
    <div class="evidence-cell">
      <h2>Stroop (1935)</h2>
      <p>Effect size 0.71 → 0.68 on 12,400 participants.</p>
    </div>
    <div class="evidence-cell">
      <h2>Loftus & Palmer (1974)</h2>
      <p>Wording effect held at 8,200 trials.</p>
    </div>
    <div class="evidence-cell">
      <h2>Tversky & Kahneman (1981)</h2>
      <p>Framing effect 67% → 64% at the larger N.</p>
    </div>
  </div>
  <!-- Three labeled facts, each visually separated. Not bullets — labeled
       blocks of visual evidence for the headline's claim. The student
       reads each block knowing what claim it supports.

       This *is* AE-compliant despite having short prose blocks: the
       blocks are visual evidence (labeled comparisons), not the
       fragmented-prose-with-leading-dots that the bullet ban exists to
       prevent. -->

  <div class="notes">
    For each of the three classical findings — Stroop, Loftus & Palmer,
    Tversky & Kahneman — we re-ran the original paradigm with the larger
    corpus. The effect sizes are within sampling error of the originals.
    The methodological point: when the original N was small (typically
    100–300 for these studies), the question was always whether a larger
    sample would shrink the effect. It did not.
  </div>
</section>
```

What changed: the headline became a claim, not a label. The student leaves the slide with *"they replicated three findings on a bigger dataset"* — a specific thought they can carry into the next slide. The three sub-elements are not bullets indexing topics; they are labeled blocks of visual evidence supporting the claim. The notes field carries the explanation the speaker will deliver, so the live deck does not also have to be a study artifact.

Notice what is *not* in the good example. There is no "we will discuss our methodology" announcement. There is no "approach / data / analysis" tripartition. There is no preamble about why replication matters. Every element on the slide either is the claim or supports it. The slide is doing one job, well.

The same surgery works at the deck's opening slide, where it carries the most leverage. The lecture-opening **Introduction** slide that lists three bullets paraphrasing the syllabus is the highest-attention real estate in the deck — students are alert, prior knowledge is unattached, the schema for the lecture is forming right now. Burning that slide on a topic label is the single most expensive mistake in academic deck design. The rewrite at the opening — *"This lecture will show that working-memory limits explain three failure modes in slide design"* — gives the rest of the deck somewhere to land. Every subsequent slide either advances the claim or extends it.

## 6. The prompt

Paste this into the Brutalist system. The principle is portable to any AI slide tool — only the system name changes.

```
Rewrite this slide's headline as the slide's claim, not the slide's topic.

Requirements:

1. The new headline is a complete declarative sentence (or sentence
   fragment that contains a verb and asserts something). It states what
   the body of the slide will substantiate. Max 12 words.

2. If I cannot tell you what the slide is claiming, the slide does not
   have a claim — flag this slide as a candidate for cutting, or rewrite
   the body so a claim is recoverable.

3. Reorganize the body as VISUAL EVIDENCE for the new headline. Replace
   bulleted lists of fragments with one of: a diagram, a chart, a
   labeled image, an annotated table, or labeled evidence blocks.
   No vertical lists of noun phrases.

4. If this slide is genuinely a reference slide — agenda, glossary,
   key-terms recap — say so explicitly and leave the label headline in
   place. Do not force assertions onto reference slides.

5. Return the slide in Brutalist HTML with .slide and .notes preserved.
   Move any prose I would say aloud into the notes field.
```

Two things to notice. First, the prompt has an explicit escape valve for reference slides — the case where a label is the correct headline. The diagnostic vocabulary lives in the prompt itself, which is what keeps the rewrite from over-correcting. Second, the prompt makes "I cannot find the claim" a *legitimate output*. If the model cannot recover a claim from the slide's body, the slide is probably not making one — and the right response is to flag it for the author, not to invent one. Many topic-label slides should be cut rather than rewritten. The prompt allows that finding to surface.

## 7. The DESIGN.md change

Two variables. One sentence each on why.

```
headline_must_assert: true
# Every teaching-slide headline is a complete declarative sentence stating
# the slide's claim. Reference slides (agenda, glossary, divider) are
# exempt — name them explicitly in the slide's class list.

headline_max_words: 12
# An assertion that exceeds 12 words usually contains either two claims
# (which want two slides) or an unnecessary clause (which wants cutting).
# 12 is the working ceiling — not a target.
```

The first variable is the principle. The second is the discipline that keeps the principle from producing wordy slides — *"Look at this trick, it's beautiful"* is a six-word assertion; *"The proton gradient powers ATP synthase"* is also six. Short complete sentences do most of the work most of the time. The 12-word ceiling exists to surface the slides where the author is stretching toward two claims. When the headline runs long, the question is not *"how do I shorten it?"* — it is *"is this one slide or two?"*

The reference-slide exemption is the part that prevents the rule from over-firing. In a fifty-slide lecture deck, three to five slides are genuinely reference: agenda, glossary, key-terms recap, the divider slides that mark section transitions. Forty-five are teaching slides where an assertion is the correct headline. The default is the assertion. The exception is the label. Naming the exception explicitly in DESIGN.md prevents the next generation of slides from drifting back into label-headlines under the cover of "but the agenda needs a label too."

## 8. The diagnostic questions to keep

Run any slide through these. If any answer is *I don't know* or *it's just a topic*, the slide has a label, not a claim.

1. **Is the headline a claim or a label?** A claim is a sentence with a verb that asserts something. A label is a noun phrase that names the subject. Different grammars do different jobs.
2. **Could a student leave this slide with a specific thought in their head?** If the only thought they could leave with is "the slide was about X," the headline has done no teaching work.
3. **Does the body provide visual evidence for the headline's claim?** A diagram, a chart, a labeled image, an annotated comparison — visual evidence for the claim the headline made. Not a vertical list of fragments.
4. **Could I summarize this slide in one sentence to a colleague in the hallway?** That sentence is the assertion. If you cannot summarize it in a sentence, the slide does not know what it is claiming.
5. **Is this a teaching slide or a reference slide?** Teaching slides default to assertions. Reference slides (agenda, glossary, key terms) correctly use labels. Name the type before fighting the headline.

## 9. What two people might disagree about

Two faculty members can read this chapter and arrive at honest, defensible disagreements. Naming where matters more than picking a side.

**How strictly to enforce the no-bullets rule.** Alley's strict version excludes bulleted lists from the body of an AE slide entirely; Atkinson's *Beyond Bullet Points* is less doctrinaire about bullets per se and more focused on the assertion headline. Wolfe et al. (2024) does not isolate the bullet question. The defensible disagreement: *when is a bulleted list a fragmented prose dump (bad) versus a labeled enumeration of genuinely list-shaped content (acceptable)?* My reading is that bullets are usually a tell that the author has not chosen a visual form. When the content is genuinely enumerative — three classical findings, four operations on a figure, five color rules — labeled evidence blocks usually beat bullets, and a diagram or chart usually beats both. But the position you can defend in framework vocabulary is: *bullets allowed only when the relationship is genuinely a flat list and no better visual form exists.* The position you cannot defend is: *bullets because Word lets you make them quickly.*

**Whether assertion headlines work for every slide type.** The strict AE position is yes — every teaching slide makes a claim, so every teaching slide can have an assertion headline. The relaxed position is that some slides are legitimately reference slides — definitions, term lists, agendas — and forcing assertions onto them produces awkward fictions. ("The agenda for today is six items long" is not a useful headline.) The vocabulary that lets these two positions argue precisely: *is this slide teaching something new (claim) or providing something for lookup (reference)?* Different jobs warrant different headline structures. The book's recommendation is to default to assertions for teaching slides, allow labels for reference slides, and document the rule in DESIGN.md as an explicit decision rather than a per-slide judgment.

**Whether academic papers and academic slides should share a grammar.** The most common faculty objection is that papers use section labels — "Introduction," "Methods," "Results" — and asking slides to use full sentences feels stylistically inconsistent with academic writing. The objection is real and resolves once the artifacts are specified. Papers and slides are read in different conditions. A paper is read in time — minutes per page, often re-read, with the section header serving as a navigational anchor for a reader who is in the middle of an argument they have been following for ten pages. A slide is scanned in three seconds — the audience has no prior context with this slide, no opportunity to re-read, and no way to navigate. Different reading conditions, different headline grammars. The label is correct for the section header of a paper. It is not correct for the title of a slide. Naming the artifact resolves the disagreement.

---

The chapter has been a long argument for one short test. *Is the headline a claim or a label?* Apply it to the next deck the system generates. Find the slides with topic-label headlines. Rewrite the headlines as claims. Watch what the body of each slide does in response. Most of the time, the body discovers it does not have evidence for any claim, and the slide reveals itself as one that should be cut. That, by itself, is worth the chapter.

The next chapter is the one that asks who is running this whole machine. You have ten variables, ten vocabularies, ten places where AI slide tools fail and you now know why. The DESIGN.md is where those decisions live persistently. Whose decisions are they? That is Chapter 11.

---

**What would change my mind:** A replication of Garner & Alley (2013) or Wolfe et al. (2024) in an asynchronous study-artifact condition (slides read without a speaker) that finds the AE advantage *does not* hold when the slide is the only source of explanation. The empirical record is on live or recorded-lecture conditions; the async case is plausibly AE-favorable but is empirically thinner. If a strong null arrives, the assertion-headline prescription weakens for study-only decks. `[verify whether such a study has appeared 2024–2026]`

**Still puzzling:** I do not have a clean rule for the length ceiling on an assertion. The chapter sets twelve words as a working maximum, but the number is a Brutalist convention, not a finding. The AE literature is mostly silent on length thresholds, and practitioner rules of thumb range from "one line" to "two lines maximum." A defensible benchmark would require an empirical study I cannot find.

**Tags:** assertion-evidence, Alley, Garner, headline-grammar, label-vs-claim
