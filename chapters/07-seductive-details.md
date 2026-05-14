# Chapter 7 — Seductive Details

> If you removed this from the slide, would the student still learn what they need to learn?

---

## 1. The feeling

You finish a deck on the Krebs cycle and step back. You like it. The first slide has a cute hand-drawn mascot of a cartoon mitochondrion smiling next to the title. Slide three has a pull quote from Hans Krebs himself — Nobel laureate, dignified, looks great in a serif font. Slide seven has a "fun fact" callout: *one molecule of glucose yields ~36 ATP — enough to power a single human heartbeat for about a second.* You like that one especially. The deck feels rich. Sourced. A little bit playful. The students will like it.

You teach the lecture. They laugh at the mascot. A hand goes up about the Hans Krebs quote — somebody had heard he'd been forced to flee Nazi Germany and wants to know more. You spend three minutes on that. The ATP-per-heartbeat fun fact gets a quiet *whoa*. The room is warm. You feel like the lecture landed.

Two weeks later you grade the unit test. The class mean on "describe the role of acetyl-CoA in the citric acid cycle" is 41%. On the multiple-choice item about the mascot's name — which you didn't ask, because of course you didn't — they'd have aced it. They remember the mascot. They remember the Nazi Germany detour. They remember the heartbeat number. They do not remember the cycle.

This is not a failure of effort. They were engaged. You were engaged. The deck was *good*. Something else happened. The interesting parts of the deck displaced the load-bearing parts in the students' memories. The very things you added to make the deck warm and rich are the things that ate the lecture.

That mechanism has a name, and it is older than you might think.

## 2. The two diagnostic questions

Ask both. In this order. Every slide, every image, every "by the way," every aside.

**From cognitive science:** *Is anything on this slide non-essential to the learning objective?* This is the Coherence Principle in Mayer's form ([Mayer, *Multimedia Learning*, 3rd ed., 2020](https://www.cambridge.org/core/books/multimedia-learning/E64FFFAB9D984ECCFEA38D63A9DAA4E5)). "Non-essential" here is a precise idea, not a polite one. Non-essential means: there is no learning objective for this lecture that the element advances. The mascot does not. The Hans Krebs biographical aside does not. The ATP-per-heartbeat fun fact does not. They are warm-up; they are not the work.

**From visual design:** *If I removed this, would the slide still communicate what it must?* This is the subtractive question. The default move in slide design is additive: another illustration, another quote, another callout box, another stock image. Coherence asks the opposite question. The slide gets better not by adding things but by removing things. If removing the element does not damage the slide's communication, the element was decoration.

The two questions converge on the same diagnostic. The first asks "what is this for, in terms of what the student is supposed to leave with?" The second asks "what would change if it weren't here?" If the answers are "nothing in particular" and "nothing important," the element is a seductive detail and it is hurting the lecture.

## 3. The principle named

Plain language first: **interesting content that is not essential to the learning objective makes the lecture worse, even though it feels like it makes the lecture better.** And: **a slide gets stronger by removing things, not by adding them.**

In framework vocabulary, the finding is called the *seductive details effect*. The phrase was coined by [Garner, Gillingham & White (1989)](https://www.tandfonline.com/doi/abs/10.1207/s1532690xci0601_2) in *Cognition and Instruction*, who added vivid but tangential sentences to expository passages and found that readers remembered the vivid sentences and forgot the main ideas. The seductive material *seduced* attention away from the structural content. Note the citation: **Garner, Gillingham, and White, 1989** — not "Garner and Brown," a misattribution that floats around in teaching-workshop slides. Brown enters the literature later, as a co-author of the [1992 follow-up paper](https://www.tandfonline.com/doi/abs/10.1080/00461529209368973) (Garner, Brown, Sanders & Menke). Worth getting right; the original effect is 1989 and the co-authors are Gillingham and White.

The finding generalized fast. [Harp & Mayer (1998)](https://psycnet.apa.org/record/1998-10717-006) took it to multimedia, running four experiments in which undergraduates received a lesson on how lightning forms either stripped to its structural content (the step-down leader meeting the upward streamer, charge separation in cumulonimbus clouds) or with added "interesting" material — anecdotes about lightning strike survivors, dramatic photographs, mortality statistics. The seductive-details group recalled fewer of the structural steps and did worse on a problem-solving transfer task. The seductive content was *related* to lightning — not random noise, not off-topic — and still damaged learning. The result is what makes the effect surprising. Relatedness is not the same as relevance to the learning objective.

[Rey's 2012 meta-analysis](https://www.sciencedirect.com/science/article/abs/pii/S1747938X12000413) in *Educational Research Review* synthesized 39 experimental effects and confirmed small-to-medium negative effects on retention and medium negative effects on transfer. The effect replicates. It is one of the better-supported findings in multimedia learning research. It is also one of the most counterintuitive, which is why it is so consistently ignored in practice.

The mechanism most cleanly named by Harp & Mayer is *diversion*: the seductive detail captures attention and primes a schema that is the wrong scaffolding for the target content. The lightning-survivor anecdote primes *lightning-as-danger*. The target content is *lightning-as-electrostatic-process*. The student integrates the new material under the wrong heading and the structural content lands poorly. Two later mechanisms — disruption of local coherence between connected sentences, and pure schema-interference even when local coherence is preserved ([Eitel et al., 2023](https://link.springer.com/article/10.1007/s11251-023-09632-w)) — co-contribute. The effect is robust to mechanism; you do not have to pick one to take the finding seriously.

The design-level expression of all this is Mayer's **Coherence Principle**: *people learn better when extraneous material is excluded rather than included.* It is one of three "reduce extraneous load" principles, alongside Signaling and Redundancy. Coherence is the one stated *negatively* — exclude — because the failure mode it corrects is additive. The default error in slide design is putting more things on the slide. The corrective is the opposite move.

## 4. Bad example

Here is the second slide of a unit on cellular respiration. It is the Krebs-cycle slide you would generate by typing the topic into Gamma or Beautiful.ai. It is also approximately the slide a well-meaning instructor produces when they want the lecture to feel "engaging."

```html
<!-- BAD: every element except the cycle diagram is a seductive detail.
     The slide feels rich. The slide damages retention of its own content. -->
<section class="slide">
  <h1>The Krebs Cycle</h1>
  <!-- Topic label, not a claim. Doesn't hand the student anything to remember
       except the name of the unit. Worse: it sets up the slide as "about" the
       cycle rather than asserting what happens in it. -->

  <aside class="mascot">
    <img src="cartoon-mitochondrion.png" alt="Smiling mitochondrion mascot named 'Mito'">
    <!-- Decorative cartoon. Encodes no biochemical content. Primes a schema
         (cute-character / friendly-introduction) that is wrong for the target
         schema (oxidation reactions in a metabolic cycle). Seductive picture
         under the Coherence Principle. -->
  </aside>

  <blockquote class="quote">
    "I have always been fascinated by intermediary metabolism."
    <cite>— Hans Krebs, 1953 Nobel Lecture</cite>
    <!-- True quote, real person, legitimately sourced. Also a seductive detail:
         encodes no step of the cycle, no enzyme, no substrate. The slide spends
         layout, attention, and visual weight on a sentence that holds no
         testable content. -->
  </blockquote>

  <figure class="cycle-diagram">
    <!-- The actual content: an eight-step cycle showing citrate → isocitrate →
         α-ketoglutarate → succinyl-CoA → succinate → fumarate → malate →
         oxaloacetate, with enzyme names and where CO2 / NADH / FADH2 exit. -->
    <!-- Rendered at ~30% of slide area, because the mascot, quote, and
         callout are taking the other 70%. The cycle — which is the entire
         point of the slide — is the smallest element on it. -->
  </figure>

  <div class="fun-fact-callout">
    <strong>Fun fact:</strong> One glucose molecule generates enough ATP
    (~36) to power a single human heartbeat for about a second.
    <!-- Mixed numerical/anecdotal callout. Activates the schema
         "biochemistry-as-bodily-magic." The actual relationship between the
         Krebs cycle and ATP yield is structural (2 ATP / cycle, 3 NADH and 1
         FADH2 feeding oxidative phosphorylation), not "heartbeats per glucose."
         The fun fact reads as illumination; it teaches the wrong thing. -->
  </div>
</section>
```

Four elements share the slide. One of them — the diagram — encodes the learning objective. The other three are seductive details by the diagnostic question: removing them does not damage the slide's communication of what the Krebs cycle *is*. Removing them improves it, because the cycle diagram is freed to occupy the visual real estate it should have been occupying all along.

The trap is that each individual element has a defense. The mascot "warms the slide up." The Krebs quote "shows the human side of science." The fun fact "makes the chemistry feel relevant." These are defenses about *the lecture's affective experience*. They are not defenses about the learning objective. The diagnostic question forces the distinction.

A further uncomfortable feature: the AI slide tool produced two of the three seductive elements on its own. Gamma offered the mitochondrion mascot from its illustration library. Beautiful.ai auto-suggested the Krebs portrait quote. You wrote the fun fact yourself, because that one is on you. The point is that *the tool's defaults are seductive-detail-generating*. Stock illustration, quote callouts, fact boxes — these are the engagement-optimized grammar of consumer slide decks, imported wholesale into the lecture deck whether they belong there or not. The instructor is fighting the tool's defaults every time.

## 5. Good example

Same source content. Three elements gone.

```html
<!-- GOOD: the diagram is the slide. The headline asserts what the diagram
     shows. The student's working memory has nowhere to go except the cycle. -->
<section class="slide">
  <h1>Each turn of the cycle releases 2 CO<sub>2</sub>, captures 3 NADH and 1 FADH<sub>2</sub>, and yields 1 ATP.</h1>
  <!-- Assertion headline. Full sentence, claims the structural fact, the one
       sentence the student should leave the slide saying out loud. -->

  <figure class="cycle-diagram">
    <!-- Same eight-step diagram, now rendered at slide scale.
         Enzymes labeled at the last-row-readable size.
         Exits for CO2, NADH, FADH2 visually distinguished by position and color.
         Acetyl-CoA entry and oxaloacetate regeneration marked as the cycle's
         closure. No mascot. No quote. No callout. The slide is the cycle. -->
  </figure>

  <div class="notes" style="display:none">
    <!-- Notes field carries what the speaker says aloud:
         "The cycle was named for Hans Krebs, who described it in 1937
         and got the Nobel for it in 1953. The number students should
         remember is *per turn*: 2 CO2 out, 3 NADH and 1 FADH2 captured
         (the electron carriers that drive oxidative phosphorylation in
         the next chapter), 1 ATP directly. Two turns per glucose —
         because glycolysis produces two pyruvates. So per glucose: 6
         CO2 total, 6 NADH and 2 FADH2 from the cycle, plus 2 ATP." -->
    <!-- Krebs biographical detail relocated, not deleted. Students who
         want it can read it; students learning the cycle aren't asked
         to integrate it during the load-bearing moment. -->
  </div>
</section>
```

What changed: the mascot is gone, the quote is gone, the fun fact is gone, the cycle diagram occupies the slide instead of competing for one quadrant of it, and the headline asserts the structural fact rather than labeling the topic. The Hans Krebs biographical detail did not disappear — it moved to the notes field, which is the other channel. If the slide is in *live* mode, the speaker can mention Krebs in 10 seconds during the verbal narration. If the slide is in *study* mode (Chapter 9), the notes appear as a sidebar paragraph the student can read.

The slide will look more austere than the bad version. That austerity is what teaching a hard concept looks like. The Coherence Principle says aesthetics is not the criterion; learning is. The slide that respects coherence often looks emptier and teaches better.

## 6. The prompt

The Brutalist prompt for this fix is a content audit followed by a removal, and the same prompt template ports to any AI slide tool. The principle is what matters; the system name is interchangeable.

```
Audit this slide. For every visible element — title, image, quote,
callout, fact box, decorative graphic — answer this question:

  Which specific learning objective for this lecture does this element
  advance?

If the answer is "it's interesting," "it provides context," "it
motivates students," "it warms up the slide," or "the tool added it" —
the element is a seductive detail. Remove it.

For elements that pass the test, keep them. For elements that are
load-bearing but currently decorative (e.g., a diagram rendered too
small), promote them: increase their visual weight, give them more
slide area, treat them as the slide.

Then rewrite the headline as a full-sentence assertion of the
structural claim the slide is communicating. Not "The Krebs Cycle" —
"Each turn of the Krebs cycle releases 2 CO2, captures 3 NADH and
1 FADH2, and yields 1 ATP."

Relocate any seductive detail that earns a relocation to the notes
field. If it does not earn the notes field, delete it.
```

The prompt is doing two things at once. It is forcing the instructor to articulate the learning objective for the slide — which most slide-design failures begin by skipping. And it is naming the failure mode of the AI slide tool's defaults, so the instructor knows what to look for when the system auto-suggests an image.

## 7. The DESIGN.md change

The DESIGN.md variable that operationalizes this chapter is a strict default for content slides:

```yaml
# DESIGN.md — seductive details enforcement
decorative_imagery_per_content_slide_max: 0
# Every visual element must encode learning content. Decorative
# imagery, stock photographs, mood backgrounds, mascots, and "fun
# fact" callouts are forbidden on content slides by default.
#
# Title slides and section dividers may have decorative imagery
# under decorative_imagery_per_divider_slide_max (default: 1).
# These are not content-bearing slides and the rule does not apply.

notes_field_relocation: enabled
# Seductive detail material that the author considers valuable can
# be relocated to the slide's notes field. Material that does not
# earn the notes field is deleted, not retained "for the record."
```

The variable is set to 0, not "minimize" or "reduce." The default is hard. The reasoning is that "reduce" defaults invite negotiation back up — one mascot becomes two — and the empirical evidence on seductive details supports a hard floor more cleanly than a soft one. The instructor who has a defensible exception (a diagram that is *both* decorative and informative, an image that is the actual subject of the discussion) raises the value in their own DESIGN.md and writes the reason in a comment. That is the Brutalist move: defaults are conservative, departures are documented.

## 8. The diagnostic questions to keep

For any slide, any element, any "wouldn't it be nice if I added —":

1. **Which specific learning objective for this lecture does this element advance?** If the answer is general ("it provides context," "it's interesting"), the element is seductive.
2. **If I removed this, would the slide still communicate what it must?** If yes, removing it is not a loss; it is a correction.
3. **Did the AI slide tool propose this, or did I?** Tool-proposed images are seductive-detail candidates by default. The tool's training signal is engagement and aesthetic conformity, not student retention.
4. **Where is the cycle / process / claim / number that is the slide's actual content?** If it is smaller on the slide than a decorative element, you are signaling to the student that the decoration is the point.
5. **Is this element warming up the slide, or teaching from the slide?** Warming-up is a defensible choice on a title slide or a section divider. It is the wrong choice on the slide where the work happens.

Run these on every content slide. You will cut a lot. The deck will look sparser. The students will do better.

## 9. What two people might disagree about

Two reasonable instructors can disagree about where the boundary between *essential context* and *seductive detail* falls. Take the bond duration example from the research notes: a finance lecture opens with the 2022 UK gilt crisis — pension funds margin-called when Liz Truss's mini-budget crashed long-dated gilt prices. The story is dramatic, current, true. Is it a seductive detail or load-bearing context?

The answer is *it depends on the learning objective*. If the objective is "compute the duration of a coupon bond," the story is seductive — students will remember the political drama and not the math. If the objective is "explain why duration matters for portfolio risk," the story is load-bearing — it shows duration becoming materially consequential, which is the *reason* the math matters. Same story. Opposite verdicts. The disagreement between two instructors is usually not about the story; it is about what they think the slide is for. Naming the objective resolves it.

A second genuine disagreement: whether motivation is itself a learning objective. Some instructors argue that engagement is a prerequisite — a student who has disengaged learns nothing — so a seductive detail that re-engages a tired room is net positive even if it dilutes recall. The defense is structurally honest but empirically narrow. In the experiments the research tested, the seductive-details students were *more engaged* (rated the material more interesting) and *less learned*. Engagement did not transfer to retention; the trade was a real loss. The honest faculty move is to treat engagement and comprehension as separable design problems and design for both independently — opening with a real problem (which is engaging *and* on-objective) rather than with a decorative image (engaging and off-objective).

The vocabulary for the disagreement is sharper than "I like it more / I like it less." Two instructors who disagree about whether to cut the Hans Krebs quote can converge by asking: *which specific learning objective does this quote advance, and is there evidence that students retain the cycle better when the quote is present versus absent?* The first question can usually be answered. The second is empirical and, for any specific instructor's specific class, almost never tested. Where the empirical answer is missing, the diagnostic question is the next best instrument. Use it.

---

Bridge to Chapter 8. This chapter taught the cut at the element level: the mascot on the slide, the quote in the callout, the fun fact in the corner. The next chapter takes the same finding — *more is often less when "more" is not in service of an objective* — and applies it to the deck as a whole. A 60-slide deck that covers every term in the week's reading is the deck-scaled version of a slide cluttered with decorative imagery. The diagnostic question is the same. The unit of analysis is different.

---

**What would change my mind:** A direct experimental comparison showing that decks designed under the Coherence Principle (no decorative imagery, assertion headlines, content-only slides) produce *equal or lower* retention than decks with conventional engagement-optimized defaults (mascots, fun facts, mood images) when matched for instructor and content. The component evidence (Harp & Mayer, Rey 2012, the broader Coherence Principle literature) supports the design move. A head-to-head deck-level comparison would settle it. I haven't found one, and that is the seam in the argument I am most uncomfortable about.

**Still puzzling:** Why a small number of seductive-detail-rich lectures genuinely seem to produce strong learning — the Feynman lectures, for example, which include digressions, jokes, and asides that the Coherence Principle would predict to be costly. My current best guess is that Feynman's "seductive details" are usually doing structural work disguised as digression — they prime a schema the next concept will plug into — and that the apparent decoration is actually load-bearing once you trace where the analogy lands. But that is a guess about specific cases, not a defense of the practice in general. I do not yet have a clean account of when an apparent seductive detail is doing schema-work and when it is just diverting attention.

**Tags:** seductive-details, coherence-principle, harp-and-mayer-1998, garner-gillingham-white-1989, slide-design-diagnostics
