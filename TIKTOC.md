# Brutalist: Using D3 and HTML to Make Slide Decks
## TicTOC.md — Full Planning Document

**Author:** Nik Bear Brown
**Series:** Brutalist D3
**Version:** 1.0
**Status:** Pre-draft — chapter list confirmed, ready for chapter specification

*Phase 1–2 output from Tic TOC. Built through interactive intake /i1–/i4 and /l1–/l3.*

---

## PART 1 — VISION AND POSITIONING

### Book Concept Summary

This book teaches **diagnostic visual literacy** — the trained eye that
knows what to tell the Brutalist system to change — to faculty and
educators who are producing mediocre slides with AI tools (Canva, Gamma,
Beautiful.ai) they cannot improve because they lack the vocabulary to say
what is wrong.

It delivers that literacy **through examples**: every principle is
demonstrated in a before/after slide pair, and every fix is a prompt the
reader can run immediately in the Brutalist system. Theory is never
assigned — it is built inductively through repeated, precise exposure to
the same diagnostic questions applied to real slide problems.

**The book succeeds if the reader can look at a Brutalist-generated slide
deck, name specifically what is wrong with any slide, and give the system
an instruction precise enough to fix it.**

One-sentence logline:
*You can't prompt precisely if you can't see precisely — this book builds
the seeing.*

---

### Book Type and Deployment Specification

**Primary type:** Practitioner handbook — read cover to cover once to
build the eye, then used as a diagnostic reference when something feels
wrong with a deck.

**Not:** A course textbook (chapters are not week-sized units), a
field-defining monograph (not an argument cover to cover), a Brutalist
system manual (the system is the medium, not the subject).

**Primary reader:** Faculty member. Has taught for years. Makes slides by
transcribing textbook content into bullets. Has used Canva, Gamma, or
Beautiful.ai and found the output "OK but not what I want." Has never
read a design book. Not trained in instructional design. Comfortable
enough with code to be in the Brutalist series, or willing to learn.

**Coding floor:** The reader can use the Brutalist system. CLAUDE.md,
DESIGN.md, and PROJECT.md are known or learnable. No prior D3 expertise
required — the system handles generation.

**Prior Brutalist knowledge required:** None. Independent entry point.
The Brutalist D3 graphicacy book is complementary (better charts in
slides if read) but not prerequisite.

**Secondary readers:** Anyone making slide decks with AI tools who is
frustrated that the output is "OK but not what I want" and cannot say
why.

**What this book is NOT:**
- Not "Slide Design for Dummies"
- Not a theory textbook — Mayer and Tufte are infrastructure, not content
- Not a Brutalist system manual
- Not a comprehensive treatment of cognitive science as academic subject

---

### Central Argument and Thesis

> "This book argues that AI slide tools (Canva, Gamma, Beautiful.ai)
> produce output the user cannot improve because they have no diagnostic
> vocabulary — this book builds that vocabulary across two frameworks
> (cognitive science and visual design) using a medium (D3/HTML) that
> makes every fix cheap and visible, and this matters because imprecise
> prompting produces imprecise slides regardless of how good the
> underlying system is."

**The DESIGN.md as artifact:** Each chapter hands the reader a new
variable they can control — and the confidence to know *why* they are
changing it. The reader's DESIGN.md may end up different from the
Brutalist defaults. That is a feature, not a bug. The book is
prescriptive about the diagnostic questions and vocabulary. It is not
prescriptive about the right answer.

**The meta-principle:** This book teaches instructional design principles
by demonstrating instructional design principles in its own pedagogy.
Theory through examples is itself the application of Mayer's Multimedia
Principle, the Coherence Principle, and the Segmenting Principle. The
book is an instance of what it teaches. Named once in the introduction,
then modeled throughout without labeling it.

---

### Theoretical Framework (invisible infrastructure)

Two frameworks. Never assigned as reading. Always operating as the
engine behind every diagnostic example.

**Framework 1 — Cognitive Science / Instructional Design**
- Cognitive Load Theory (Sweller): intrinsic, extraneous, germane load
- Mayer's Multimedia Learning Principles (12): coherence, signaling,
  redundancy, spatial contiguity, temporal contiguity, segmenting,
  pre-training, modality, multimedia, personalization
- The Seductive Details Effect (Harp & Mayer 1997–98; Rey meta-analysis
  2012): interesting but irrelevant content actively harms retention
- Assertion-Evidence model (Alley): full-sentence headline + visual
  evidence outperforms topic header + bullets
- Chunking and working memory limits (~4 ± 1 items)
- Slideument problem (Reynolds): the hybrid that serves neither live
  delivery nor study artifact

**Framework 2 — Visual & UX Design**
- Tufte: data-ink ratio, cognitive style of PowerPoint, chartjunk,
  the Columbia disaster as a slide failure
- Reynolds (Presentation Zen): signal vs. noise, simplicity as removal
- Duarte (slide:ology): the glance test, one idea per slide
- Typography for projection: sans-serif, size hierarchy, the last-row rule
- Layout and whitespace: grid, gestalt proximity, alignment
- Color for instructional contexts: contrast ratios (WCAG AA 4.5:1),
  colorblind-safe palettes, semantic vs. decorative color use
- Visual form selection: when text, when diagram, when chart, when table

**Key sources loaded as pantry research:**
- Four deep research documents covering both frameworks in full
- DESIGN.md, CLAUDE.md, PROJECT.md from the Brutalist stack
- The Causal Reasoning TOC as structural model for chapter specification

---

### Field Positioning

**The gap:** No book teaches slide design diagnostics through live,
runnable examples in a code-based system. Existing design books
(Reynolds, Duarte, Tufte) teach principles. They do not teach the
reader to translate a principle into a precise prompt that fixes the
slide. Canva and Gamma teach nothing — they just produce.

**Comparable texts:**

*Presentation Zen* (Reynolds):
Teaches the aesthetic of simplicity through inspiration and philosophy.
Beautiful book. Does not teach diagnostic vocabulary. Does not give the
reader a prompt. This book: same sensibility, different delivery — every
principle is a before/after pair and a runnable fix.

*The Cognitive Style of PowerPoint* (Tufte):
The definitive critique. Explains why slides fail analytically. Does
not build the eye incrementally or give the reader control mechanisms.
This book: Tufte's diagnosis as one input among many, delivered through
examples rather than polemic.

*slide:ology* (Duarte):
Practical and visual. Organized around slide types rather than failure
modes. Assumes the reader is building from scratch, not fixing AI output.
This book: problem-first, AI-tool-aware, DESIGN.md as the artifact.

**Positioning statement:**
"Unlike existing slide design books, which teach principles for readers
building decks from scratch, this book teaches diagnostic vocabulary for
readers who already have AI-generated output and need to know precisely
what to change — and how to say it."

---

## PART 2 — LEARNING ARCHITECTURE

### Sequencing Model

**Primary model:** Problem → Solution (Concrete → Abstract embedded
within each chapter)

**Justification against learner profile:** The faculty member's entry
point is always "this slide doesn't feel right." They do not arrive
asking "what is the coherence principle?" They arrive with a deck that
is producing a feeling of wrongness they cannot name. Every chapter
must begin with that feeling and build toward the vocabulary that names
it. Theory that arrives before the problem it solves will be ignored
by this reader — they have never read a design book and will not start
now unless the design problem is already on the table.

**Within each chapter:** Concrete before abstract. The bad slide comes
first. The principle is named after the reader has felt the problem.
The fix — a prompt — is the application. The DESIGN.md change is the
integration.

**Most likely breakdown chapter:** The sequencing vs. live/async
distinction (Chapter 9 candidate) — because it requires the reader to
think about their deck as two different objects simultaneously, which
is a more abstract move than the earlier visual diagnostic chapters.

**Transition point:** After Chapter 5 (roughly). The first five chapters
build the eye for individual slide problems. From Chapter 6 onward, the
problems become deck-level (sequence, arc, live vs. async). The
transition requires the reader to shift unit of analysis from slide to
deck. This must be named explicitly at the transition.

---

### Three-Act Learning Arc

**Arc statement:**
"This book takes the reader from *frustrated user of AI slide tools who
can feel but not name what is wrong* to *practitioner who can diagnose
any slide problem in precise vocabulary and give any AI slide system an
instruction that fixes it* by first building the eye for individual slide
failures (Act One), then building the eye for deck-level failures (Act
Two), then integrating both frameworks into a DESIGN.md the reader owns
and can defend (Act Three), leaving them with a one-page diagnostic
checklist they can use on any slide, in any system, forever."

**Prompt portability (decided):** Every prompt in the book is written
as a principle first, with Brutalist as the reference implementation.
The reader using Canva, Gamma, or any other AI slide tool gets the same
diagnostic vocabulary and the same prompt structure — only the system
name changes. Brutalist is the demonstration, not the prerequisite.

**Act One — Build the Eye for the Slide (Chapters 1–5)**
*Unit of analysis: the individual slide*

Starting state: The reader can feel that a slide is wrong but cannot
name why. They know "I don't like this" and cannot say more.

Ending state: The reader can look at any slide and apply both
frameworks — cognitive science and visual design — to name the specific
failure. They have vocabulary. They can form a prompt.

Inciting question per chapter: "What exactly is wrong here?"

Act One → Act Two transition: The reader can diagnose individual slides.
The next question is whether the deck as a whole is working — which
requires a different unit of analysis.

**Act Two — Build the Eye for the Deck (Chapters 6–9)**
*Unit of analysis: the deck as a sequence and artifact*

Starting state: The reader can fix individual slides but cannot yet see
how the deck fails as a whole — in sequence, in arc, in its dual life
as live delivery and study artifact.

Ending state: The reader can evaluate a full deck against both the
cognitive science arc (hook, build, consolidate) and the live/async
split. They know what the deck is *for* and can make structural changes.

Hardest conceptual moment: The live vs. async split (Chapter 8
candidate) — because it requires accepting that one deck cannot do both
jobs, which conflicts with how most faculty currently work.

Act Two → Act Three transition: The reader has the full diagnostic
vocabulary. The final question is: how do you own your design decisions
instead of accepting the system's defaults?

**Act Three — Own Your DESIGN.md (Chapters 10–11)**
*Unit of analysis: the DESIGN.md file as design philosophy*

Starting state: The reader understands what to change and why but
has not yet integrated the two frameworks into their own coherent
design philosophy.

Ending state: The reader can read their DESIGN.md, explain every
decision in it in the vocabulary of both frameworks, and update it
with confidence when they encounter a new slide problem. Their
DESIGN.md is theirs — not the Brutalist default, not a copy of
anyone else's.

---

### Learning Outcomes (by chapter)

*Practitioner handbook format: outcomes stated as diagnostic and
production capabilities, not academic competencies.*

**Chapter 1 — The Slideument Problem**
1. (Analyze) Distinguish a slideument from a slide deck: name the
   structural difference and predict the failure mode of each for
   a given use case.
2. (Apply) Identify slideument characteristics in a Brutalist-generated
   deck and produce a prompt that begins separating them.

**Chapter 2 — No Clear Hierarchy**
1. (Analyze) Diagnose hierarchy failure in a slide: name which
   Gestalt and cognitive load principles are violated and where.
2. (Apply) Produce a prompt that establishes a clear visual hierarchy
   using DESIGN.md typography and spacing variables.
3. (Evaluate) Assess whether a proposed hierarchy change serves the
   slide's communication goal or merely imposes order.

**Chapter 3 — Too Much Text**
1. (Analyze) Identify text density failure using the redundancy
   principle and the slideument diagnostic.
2. (Apply) Produce a prompt that reduces text to the minimum required
   for the slide's communication goal.
3. (Evaluate) Distinguish text that is load-bearing from text that
   is seductive detail — and defend the distinction.

**Chapter 4 — The Wrong Visual Form**
1. (Analyze) Match content type to visual form using the
   text/diagram/chart/table decision framework.
2. (Apply) Produce a prompt that replaces an inappropriate visual
   form with the correct one for the content type.
3. (Evaluate) Justify the visual form choice in vocabulary from
   both the cognitive science and visual design frameworks.

**Chapter 5 — Color Is Doing Nothing (or Harm)**
1. (Analyze) Diagnose color failure in a slide: decorative vs.
   semantic use, contrast ratio failure, colorblind accessibility.
2. (Apply) Produce a DESIGN.md update that fixes the color failure
   with a precise, principled rationale.
3. (Evaluate) Assess whether a color choice serves the signaling
   principle or creates extraneous load.

**Chapter 6 — The Textbook Figure on the Slide**
1. (Analyze) Identify why a direct textbook-to-slide figure transfer
   fails: resolution, label density, missing signaling.
2. (Apply) Produce a prompt that redesigns the figure for projection:
   cropped, labeled for the last row, signaled for the specific point.
3. (Evaluate) Assess when simplification of a figure crosses into
   distortion of the content.

**Chapter 7 — Seductive Details**
1. (Analyze) Identify seductive details in a deck using the coherence
   principle: content that is interesting but not essential.
2. (Evaluate) Defend the cut: explain why removing interesting content
   improves learning outcomes, against the intuition that it reduces
   engagement.
3. (Apply) Produce a prompt that removes seductive details and
   tightens the deck to its teachable core.

**Chapter 8 — The Deck That Covers but Doesn't Teach**
1. (Analyze) Diagnose coverage failure at the deck level: a deck
   organized around the textbook's structure rather than the
   learner's build.
2. (Apply) Restructure a deck's opening five slides using the
   hook/build/consolidate arc.
3. (Evaluate) Assess whether a given deck sequence serves the
   learner's mental model construction or the author's topic organization.

**Chapter 9 — Live Deck vs. Study Artifact**
1. (Analyze) Identify the specific failures that occur when one
   deck is used for both live delivery and async study.
2. (Evaluate) Make the live/async decision for a given deck and
   defend it against the instinct to produce one version for both.
3. (Apply) Produce a prompt that adjusts text density, notes fields,
   and retrieval prompts for the chosen use case.

**Chapter 10 — The Headline That Says Nothing**
1. (Analyze) Identify topic-header + bullet slides that would be
   stronger as assertion-headline + visual evidence slides.
2. (Apply) Produce a prompt that rewrites a slide in the
   assertion-evidence structure: full-sentence headline stating
   the claim, visual supporting it.
3. (Evaluate) Assess whether the assertion is a claim or a label —
   the distinction that makes or breaks the structure.

**Chapter 11 — Owning Your DESIGN.md**
1. (Evaluate) Read a DESIGN.md and explain every decision in it
   in vocabulary from both frameworks.
2. (Create) Produce a DESIGN.md update that reflects the reader's
   own diagnostic decisions across all ten prior chapters.
3. (Evaluate) Defend the DESIGN.md against a skeptic: explain why
   each departure from Brutalist defaults is principled, not arbitrary.

---

### Prerequisite Map

| Prerequisite | Safe to Assume? | Where Addressed |
|---|---|---|
| Canva / Gamma / Beautiful.ai use | Yes — this is the entry point | — |
| Brutalist system basics | Probably | Introduction + Appendix A |
| DESIGN.md structure | Probably | Introduction + Appendix A |
| D3 / HTML coding | No — not required | System handles generation |
| Design training | No — explicitly not assumed | Entire book addresses this gap |
| Cognitive science vocabulary | No | Built inductively chapter by chapter |

**Front-loading decision:** Two prerequisites rated "Probably" —
DESIGN.md structure and Brutalist system basics. Both addressed in
the Introduction and Appendix A (system overview). Neither requires
a full chapter. The reader who has used any Brutalist book is fine
from Chapter 1. The reader who is new gets what they need in the
Introduction.

---

## PART 3 — CHAPTER SPECIFICATIONS

### Chapter Anatomy Template (Practitioner Handbook)

Each chapter follows this structure:

1. **The feeling** — one slide that doesn't feel right. No
   diagnosis yet. The reader sees it and recognizes the feeling.
2. **The two diagnostic questions** — one from cognitive science,
   one from visual design. Always both. Always in this order.
3. **The principle named** — stated in plain language, then in
   framework vocabulary. Never framework vocabulary first.
4. **Bad example** — the slide that fails. Annotated with the
   precise failure mode.
5. **Good example** — the slide that works. Annotated with what
   changed and why.
6. **The prompt** — exact text the reader can paste into the
   Brutalist system to move from bad to good.
7. **The DESIGN.md change** — which variable to update, what to
   change it to, and why in one sentence.
8. **The diagnostic questions to keep** — 3–5 questions the reader
   can apply to any slide to catch this failure mode in the future.
9. **What two people might disagree about** — where reasonable
   designers make different choices, and what vocabulary they use
   to defend each position.

**Enforcement:** A chapter missing items 4, 5, 6, or 7 is an
incomplete chapter. The before/after pair and the prompt are
non-negotiable. The book fails without them.

---

### Chapter 1 — The Slideument Problem

**One-line:** The reader learns to see the difference between a
slide (a visual anchor for a speaker) and a document (a
self-contained artifact), and why a deck that tries to be both
fails at both.

**The feeling:** A deck that looks complete — full sentences,
everything explained — but is somehow exhausting to look at
during a lecture and useless to study from afterward.

**Cognitive science failure:** Redundancy principle violation.
The slide contains the full verbal explanation the speaker is
also delivering. The verbal channel is overloaded. The student
reads instead of listens.

**Visual design failure:** Reynolds' slideument. The deck has
no point of view about what it is for.

**Prompt category:** Text density reduction + notes field
population.

**DESIGN.md variable:** Body text density defaults; notes field
conventions.

**Bridge:** A slide can have too much text for a different reason
than slideument failure — sometimes the hierarchy just isn't
clear enough to show the reader what matters. That's Chapter 2.

---

### Chapter 2 — No Clear Hierarchy

**One-line:** The reader learns to name hierarchy failure
precisely — which elements are competing, which Gestalt principles
are violated, and what a prompt must specify to establish clear
visual order.

**The feeling:** A slide where the eye doesn't know where to go
first. Everything feels equally important. Or nothing does.

**Cognitive science failure:** Extraneous cognitive load from
absent signaling. The student's working memory is spent
navigating the slide rather than processing its content.
Mayer's Signaling Principle violated.

**Visual design failure:** No implicit grid, no size hierarchy,
proximity groupings that don't match semantic groupings. Gestalt
principles of proximity and similarity violated.

**Key principles:**
- Size hierarchy: title > primary message > supporting detail.
  If everything is the same size, there is no hierarchy.
- Weight: bold signals importance. If everything is bold,
  nothing is.
- Proximity: elements that belong together must sit together.
  Elements that are separated are perceived as unrelated.
- Whitespace: not wasted space — it is the signal that says
  "this is one thing."

**Prompt category:** Typography scale + spacing + grouping.

**DESIGN.md variables:** Font size scale, font weight, spacing
rhythm, layout grid.

**What two people disagree about:** How aggressive to be with
size contrast. A subtle hierarchy reads as elegant to one person
and as insufficiently clear to another. Both are defensible.
The vocabulary for the disagreement: contrast ratio of size
between levels, not "I like it more subtle."

**Bridge:** Once hierarchy is clear, the next question is whether
there is too much content at any level of that hierarchy. That
is Chapter 3.

---

### Chapter 3 — Too Much Text

**One-line:** The reader learns to distinguish load-bearing text
from seductive text from slideument text — three different
reasons a slide has too much on it, each requiring a different
prompt.

**The feeling:** A slide that looks like a page. The reader
starts reading and loses the thread of what the speaker is saying.

**Cognitive science failure (type 1 — redundancy):** The text
repeats what the speaker is saying. Verbal channel overloaded.
This is slideument failure from Chapter 1, at the individual
slide level.

**Cognitive science failure (type 2 — seductive detail):** The
text is interesting but not essential. Coherence principle
violated. The student forms a schema around the interesting
content and integrates the core content poorly.

**Cognitive science failure (type 3 — density):** The text is
all essential but presented at once. Working memory saturated.
Segmenting principle applies: reveal in sequence.

**The test:** For each text element, ask: "Which learning
objective does this serve?" If the answer is none — cut it.
If the answer is "it's interesting context" — it is a seductive
detail. Cut it.

**The benchmark:** ~30–50 words per slide for live delivery.
More than 75 words is a document, not a slide.

**Prompt category:** Text reduction + assertion extraction.

**DESIGN.md variable:** Maximum words per slide (as a convention
the reader sets for themselves).

**Bridge:** Sometimes the text is right but the visual form is
wrong — a list of relationships that should be a diagram, or a
comparison that should be a table. That is Chapter 4.

---

### Chapter 4 — The Wrong Visual Form

**One-line:** The reader learns the visual form decision matrix
and how to name the mismatch between content type and
presentation form precisely enough to prompt the correct fix.

**The feeling:** A slide where the information is right but
something about the format makes it hard to see. A list of
things that should be connected. A comparison that requires
reading back and forth. A process that has no flow.

**The decision matrix:**

| Content type | Right form | Wrong form signal |
|---|---|---|
| Relationships between concepts | Diagram, node map | Bulleted list |
| Processes and sequences | Flowchart, timeline | Numbered list |
| Comparisons of attributes | Table | Side-by-side bullets |
| Trends over time | Line chart | Text description |
| Part-to-whole | Bar chart | Pie chart (usually) |
| Cause-effect mechanisms | Annotated diagram | Paragraph |
| Definitional content | Key term + short phrase | Full sentence |

**Cognitive science failure:** The visual channel is underused.
Mayer's Multimedia Principle: words + pictures > words alone.
A bulleted list of a process is words alone. A flowchart is
words + pictures.

**Visual design failure:** Tufte's data-ink ratio. A list of
relationships has infinite ink and almost no data. A node map
shows the same relationships with structure the eye can read
in seconds.

**The Tufte rule on 3D:** Never. The depth axis adds visual
complexity without adding information and actively distorts
perception of magnitudes.

**Prompt category:** Visual form replacement — specify the
correct form, the content, and the encoding.

**DESIGN.md variable:** Default visual forms per content type
(as conventions the reader sets).

**Bridge:** Once the right form is chosen, the question is
whether the color in that form is doing work or just decorating.
That is Chapter 5.

---

### Chapter 5 — Color Is Doing Nothing (or Harm)

**One-line:** The reader learns to distinguish semantic color
(encodes meaning) from decorative color (adds noise), apply
the contrast ratio test, and check for colorblind failure —
then update DESIGN.md with precision.

**The feeling:** A slide that looks colorful but where the
color doesn't seem to mean anything. Or a slide where something
is hard to read without knowing why.

**Three failure modes:**

*Failure 1 — Decorative color:* Color used for aesthetics, not
information. "If everything is colorful, nothing stands out."
The signaling principle requires that color means the same thing
every time it appears. Random color use destroys the signal.

*Failure 2 — Contrast failure:* Text or marks that fail the
WCAG 2.1 AA standard (4.5:1 for text, 3:1 for graphical
elements). In projection environments with ambient light,
target 7:1+. The reader cannot see it. This is an accessibility
failure and a design failure simultaneously.

*Failure 3 — Colorblind inaccessibility:* 8% of men, 0.5% of
women have red-green color vision deficiency. A slide that uses
red and green alone to encode distinctions fails for 1 in 12
male students before the first word is spoken.

**The Brutalist palette rule:** DESIGN.md specifies six
variables. Red is brand and primary series — never danger or
negative. Ochre is decorative accent only — never body text.
Gray scale for everything else. This is not arbitrary — it
is colorblind-safe and contrast-tested.

**The test:**
1. Does each color encode something specific and consistent?
2. Does every text element pass 4.5:1 contrast against its
   background?
3. Would a colorblind reader lose any information?

**Prompt category:** DESIGN.md color variable update with
contrast ratio and semantic role specified.

**DESIGN.md variables:** All six color variables, with roles
and contrast ratios documented.

**What two people disagree about:** How much personality color
can carry before it becomes noise. The vocabulary for this
disagreement: "what is this color encoding?" — if the answer
is "nothing," the disagreement is settled.

**Bridge:** The eye is now trained on individual slides. The
next category of failure is the textbook figure that arrived
on the slide without redesign. That is Chapter 6.

---

### Chapter 6 — The Textbook Figure on the Slide

**One-line:** The reader learns why direct textbook-to-slide
figure transfer always fails and what four operations to specify
in a prompt to redesign the figure for projection.

**The feeling:** A figure that looks authoritative and complete
but is somehow impossible to see from more than two feet away.
Labels too small. Too much labeled. No signal about where to
look.

**Why it always fails:** Textbook figures are designed for
print — high resolution, small size, studied closely and
re-read. Slides are projected large and viewed briefly. They
are different media. A figure that works in one medium fails
in the other without redesign.

**The four operations:**

*Operation 1 — Crop:* Show only the part that serves the
current learning objective. A full-system diagram in a lecture
about one subsystem is noise. Crop to the subsystem.

*Operation 2 — Enlarge labels:* Replace small print labels
with labels that pass the last-row test. If a student in the
last row cannot read the label, the label does not exist.

*Operation 3 — Signal:* Add color, arrows, or callout boxes
to direct attention to the specific point this slide is making.
The audience cannot study the figure — they can only follow
where you point.

*Operation 4 — Simplify:* Remove labels that do not serve
the current objective. A neuroscience diagram labeled for
a textbook chapter on the full nervous system should have
all but two things removed for a lecture slide on the
autonomic system.

**The limit:** Simplification can cross into distortion. A
figure that removes so much that it misrepresents the
relationship between the remaining elements is not a better
figure — it is a misleading one. Name this limit explicitly
every time.

**Prompt category:** Figure redesign — specify the four
operations with the specific labels to keep, remove, and add.

**DESIGN.md variable:** Figure label font size; signaling
color conventions for figures.

**Bridge:** The slide eye is built. Chapters 7–9 shift to the
deck — failure modes that only appear when you look at the
full sequence.

---

---

## — ACT ONE → ACT TWO —
### From Slide to Deck

*One paragraph. Appears as a section break between Chapters 6 and 7 in the
final book. Not a chapter. No prompt. No DESIGN.md change. A reorientation.*

---

You have been looking at slides.

A slide with a clear hierarchy. A slide with the right visual form. A slide
whose color encodes something, whose figure was redesigned for the last row,
whose text earned its place. You can now see these things and name them. That
is not nothing — most people who make slides cannot do what you can do after
six chapters.

But a slide is not a lecture. A deck of individually well-designed slides can
still fail to teach. The failure mode is different: not a bad slide, but a bad
sequence. Not too much text on one slide, but the wrong content in the wrong
order across twenty slides. Not a figure that wasn't redesigned for projection,
but a deck that was organized for the author's convenience rather than the
learner's build.

The next four chapters change the unit of analysis. The slide is no longer the
object. The deck is.

This requires a different kind of looking. You are no longer asking "what is
wrong with this slide?" You are asking "what is wrong with this sequence?" The
diagnostic questions are different. The prompts are different. The DESIGN.md
changes are different.

Everything you built in the first six chapters still applies — a deck of bad
slides is still a deck of bad slides. But a deck of good slides in the wrong
order, covering content the learner wasn't ready for, ending before anyone had
to use anything — that is a deck that covers without teaching. That is the
failure mode Chapter 7 addresses.

The shift is small. The difference in what you see is large.

---

**One-line:** The reader learns to apply the seductive details
diagnostic — interesting but irrelevant content actively harms
retention — and develop the discipline to cut content that
feels like it earns its place but doesn't.

**The feeling:** A deck that feels rich, well-sourced, and
full of interesting context. Students seem engaged. But
something is preventing them from retaining the core content.

**The counterintuitive rule:** Interesting content that is
not essential to the learning objective does not enhance
learning — it damages it. Harp and Mayer (1997, 1998) ran
six experiments and found that students who received a lesson
with entertaining anecdotes and dramatic photos recalled
structurally important content at one-third the rate of
students who received the stripped-down version.

**The mechanism:** Seductive details cause diversion. Students
form inappropriate schemas around the interesting material
and integrate the core content poorly. The effect is strongest
when seductive details appear early in the instruction, when
students have low prior knowledge, and when the intrinsic
load of the material is already high.

**The diagnostic test:**
For each element: "Which learning objective does this serve?"
If the answer is "it's interesting" or "it provides context"
or "it motivates students" — it is a seductive detail.
Interesting context that cannot be mapped to a learning
objective is a seductive detail regardless of how good the
story is.

**The counterintuitive corollary:** The fun fact at the
opening of a lecture may be damaging the retention of
everything that follows it.

**Prompt category:** Content audit + removal — specify the
seductive details by name and instruct the system to remove
them or move them to notes.

**DESIGN.md variable:** Notes field conventions — seductive
details that genuinely add value move to the notes field,
not the slide.

**What two people disagree about:** Whether a specific element
is essential or seductive. The vocabulary for this disagreement:
"which learning objective does this serve?" — a specific
objective or "general context" are different answers.

---

### Chapter 8 — The Deck That Covers but Doesn't Teach

**One-line:** The reader learns to diagnose coverage failure
at the deck level — a deck organized around the textbook's
structure rather than the learner's build — and restructure
the opening arc.

**The feeling:** A deck that seems complete — every topic from
the chapter is in there — but students zone out after the
first fifteen minutes and retention on the exam is low.

**The coverage vs. teaching distinction:**
A textbook chapter must cover the full territory. A lecture
must cause learning. These are different operations. A deck
organized around textbook headings is organized for coverage.
A deck organized around the learner's mental model construction
is organized for teaching.

**The lecture arc (Hook / Build / Consolidate):**

*Hook:* A problem, question, or phenomenon that creates the
need to know. Students learn better when they understand why
they need the information before receiving it. A deck that
opens with definitions has already failed the hook.

*Build:* Concepts introduced in dependency order: prerequisites
before complex ideas, concrete before abstract. Each concept
before the one that depends on it.

*Consolidate:* Retrieval practice or application that forces
students to use what they just learned before moving on.
A deck that ends when the content ends misses the most
powerful retention opportunity.

**The 15-minute chunking rule:** Working memory saturates
after roughly 15–20 minutes of continuous input. A 50-minute
lecture needs at least two consolidation moments — not just
one at the end.

**Prompt category:** Deck resequencing — specify the hook
(a problem or question), the build sequence (dependency order),
and the consolidation moment (a question or prompt).

**DESIGN.md variable:** Deck opening conventions; retrieval
prompt slide template.

---

### Chapter 9 — Live Deck vs. Study Artifact

**One-line:** The reader accepts that a single deck cannot
serve both live delivery and async study, makes the choice
for their specific deck, and adjusts it accordingly.

**The feeling:** A deck that was posted as study materials
after a lecture. Students found it nearly useless — "it just
has bullets, it doesn't explain anything." Or: a deck so
text-dense it explains everything but is impossible to use
in a live lecture without reading from the screen.

**The two products:**

| Dimension | Live lecture deck | Study artifact |
|---|---|---|
| Text density | Minimal — speaker is the text | Higher — slide carries explanation |
| Notes field | Full script or key points | May be empty |
| Pacing | Speaker controls | Student controls |
| Retrieval prompts | Discussion moments | Must be self-contained questions |
| Visual dominance | High — anchor attention | Moderate — must work without speaker |

**The decision:** Which is this deck for? This is not a design
question — it is a use question. Design follows the decision.
A deck that tries to do both fails at both.

**Solutions when both are needed:**
1. Build two versions from the same content
2. Populate the notes field fully so the live deck becomes
   studyable without redesign
3. Record the lecture, so the live deck can remain sparse

**Prompt category:** Text density adjustment + notes field
population — specified for live or async, not both.

**DESIGN.md variable:** Notes field conventions; text density
target per use case.

**What two people disagree about:** Whether one well-populated
notes field is enough to make a live deck usable as a study
artifact. Both positions are defensible. The vocabulary: what
exactly goes in the notes field, and whether students will
actually read it.

---

### Chapter 10 — The Headline That Says Nothing

**One-line:** The reader learns to identify topic-header +
bullets slides that would be stronger as assertion-headline +
visual evidence, and produces the rewrite.

**The feeling:** A slide that has a title like "Cognitive Load
Theory" followed by five bullet points. It is correct. It is
complete. It teaches nothing.

**The topic-header problem:** A topic header names the subject.
It tells the student what the slide is about. It does not tell
the student what to think about it. The student leaves knowing
the topic was covered. They do not leave with a claim in their
head.

**The assertion-evidence structure (Alley):**
- Headline: a complete sentence stating a claim.
  Not "Cognitive Load Theory." "Working memory holds only
  four items — slide design must respect this limit."
- Body: visual evidence that supports the claim. Not bullets.
  A diagram, chart, or image that demonstrates the assertion.

**Why it works:** Garner & Alley (2013) found that slides with
a full-sentence assertion headline + visual evidence produced
higher retention on both immediate and delayed tests than
traditional topic-header + bullets. The mechanism: the claim
gives the student a schema to hang the evidence on before
they see it.

**The test for a good assertion:**
It is a claim, not a label. "Redundancy reduces learning" is
a claim. "The Redundancy Principle" is a label. Labels do
not teach. Claims do.

**Prompt category:** Headline rewrite (label → claim) +
visual form selection for the evidence.

**DESIGN.md variable:** Headline style convention — sentence
or fragment, claim or label. This is a philosophical choice
the reader makes and documents.

**What two people disagree about:** Whether assertion headlines
are always better or whether some slides are legitimately
reference slides (definitions, term lists) where a label
is the right headline. Both positions are defensible.
The vocabulary: "is this slide making a claim or providing
a reference?" — different answers warrant different structures.

---

### Chapter 11 — Owning Your DESIGN.md

**One-line:** The reader integrates ten chapters of diagnostic
vocabulary into a DESIGN.md they can explain, defend, and
update — one that reflects their own design philosophy, not
the Brutalist default.

**The feeling:** Looking at a DESIGN.md after ten chapters
and seeing it differently. Variables that were arbitrary are
now decisions. Defaults that were accepted are now either
endorsed or changed.

**The integration:**
Each chapter gave the reader a vocabulary and a variable.
This chapter asks: what is YOUR answer to each of these
questions, and why?

- What is your text density target for live slides?
- What is your notes field convention?
- What is your hierarchy: how many size levels, what weight?
- What does each color in your palette encode?
- What is your default visual form for processes? For comparisons?
- What is your assertion style — claim or label?
- Are your figure labeling conventions set for the last row?

**The DESIGN.md as design philosophy:**
A DESIGN.md that is a collection of defaults is a starting
point. A DESIGN.md that is a collection of decisions — each
one traceable to a principle from one of the two frameworks —
is a design philosophy. The reader who can explain why they
chose 28pt body text over 24pt, why their red is brand not
danger, why their headlines are claims not labels — that
reader owns their slides.

**The reader's DESIGN.md may look different from yours:**
That is the point. The book is not teaching the Brutalist
aesthetic. It is teaching the vocabulary that makes any
aesthetic decision defensible and any design problem nameable.

**Final prompt:** Write your own DESIGN.md rationale document
— one paragraph per major decision, stating the principle
behind it in vocabulary from both frameworks.

**Deliverable:** A DESIGN.md the reader can show another
person and explain every line of.

### Chapter 12 — The Diagnostic Checklist

**One-line:** A single reference page — every diagnostic question
from every chapter, organized by failure mode — that the reader
can use on any slide, in any system, forever.

**What it is not:** A chapter. No new content. No new principles.
No before/after pair. No prompt. This is a reference artifact,
not a lesson.

**What it is:** The proof that the vocabulary was built. A reader
who can work through this checklist on a slide they have never
seen before has the eye. That was the goal of the book.

**Format:** One page. Two columns. Eleven failure modes as headers.
Three to five diagnostic questions under each. Plain language —
no framework jargon. Designed to be printed, pinned, and used.

**The questions (draft — refined from chapter diagnostic sections):**

*The Slideument Problem*
- Is this deck designed for live delivery, async study, or both?
- If both: what specifically fails in each context?
- Is the notes field doing the work the slide shouldn't?

*No Clear Hierarchy*
- Where does my eye go first? Is that where it should go?
- How many size levels are there? Can I name each one's role?
- Are elements that belong together physically close?
- Is whitespace grouping the right things?

*Too Much Text*
- Which learning objective does each text element serve?
- Is any text repeating what the speaker will say aloud?
- Is any text interesting but not essential?
- Is the total word count above 50 for a live deck?

*The Wrong Visual Form*
- What is the relationship between the elements on this slide?
- Is that relationship best shown as text, diagram, chart, or table?
- Would a reader understand the relationship faster with a visual?

*Color Is Doing Nothing (or Harm)*
- What does each color encode? Can I state it in one word?
- Does every text element pass 4.5:1 contrast against its background?
- Would a colorblind reader lose any information?
- Is any color decorative — present for aesthetics, not meaning?

*The Textbook Figure*
- Was this figure designed for print or for projection?
- Can the student in the last row read every label?
- Is there a visual signal directing attention to the specific point?
- Have I removed labels that don't serve this slide's objective?
- Does simplification distort the relationship between elements?

*Seductive Details*
- Which learning objective does this element serve?
- Is it interesting without being essential?
- Would removing it make the core content clearer?
- Is it appearing early in the deck where damage is highest?

*The Deck That Covers but Doesn't Teach*
- Does the deck open with a problem or question — or with a definition?
- Are concepts in dependency order: prerequisites before complex ideas?
- Is there a consolidation moment before the 20-minute mark?
- Is this deck organized around the textbook's structure or the learner's build?

*Live Deck vs. Study Artifact*
- What is this deck for: live delivery or async study?
- If live: is the text minimal enough that students won't read instead of listen?
- If async: does the slide carry enough explanation without a speaker?
- Is the notes field populated for whichever mode this isn't?

*The Headline That Says Nothing*
- Is the headline a claim or a label?
- Could a student leave this slide with a specific thought in their head?
- Does the body provide visual evidence for the headline's claim?
- Would replacing the bullets with one image make this clearer?

*Owning Your DESIGN.md*
- Can I explain every variable in my DESIGN.md in one sentence?
- Is each decision traceable to a principle from cognitive science
  or visual design?
- If I changed this variable, could I say why in vocabulary —
  not "I like it better"?

**Production note:** This page is designed to be the last page
of the book and a standalone PDF download. Two formats:
the book version (integrated layout) and the download version
(printer-friendly, no book styling).

**The prompt for this chapter:** There is none. This chapter
is the artifact that makes all the other prompts unnecessary
for a reader who has internalized the vocabulary.

---

### What This Book Is Not

*Permanently excluded:*

| Topic | Reason |
|---|---|
| Copyright rules for textbook content | Procedural, not diagnostic. Appendix B. |
| Full Brutalist system setup | Assumed or covered in series introduction. Appendix A. |
| Mayer's principles as academic content | Infrastructure, not subject matter. Never assigned. |
| Slide software comparison (PowerPoint vs. Keynote vs. Canva) | The reader has left those tools. Not relevant. |
| Animation and transitions | Minor issue; not a diagnostic chapter. Brief note in Chapter 8. |
| D3 coding instruction | The system handles generation. Not this book. |
| Accessibility law and compliance | Contrast ratios are covered in Chapter 5. Full accessibility law is out of scope. |

*Out of scope acknowledgment:* Copyright rules are important
and frequently mishandled. Appendix B covers the four-factor
fair use test and the practical rules for textbook figures in
slides. This is not a chapter because it is procedural, not
diagnostic — it does not build the eye.

---

### Appendices

**Appendix A — The Brutalist System for New Readers**
What CLAUDE.md, DESIGN.md, and PROJECT.md are. How to run
the textbook-to-slides conversion. How to give the system
a prompt. 2–3 pages. For readers who are new to the series.

**Appendix B — Copyright Rules for Textbook Content in Slides**
The four-factor fair use test. Key rules for text and figures.
The TEACH Act for online instruction. Practical rules.
Sourced from the deep research document already in pantry.

---

### Adoption Risk Register

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Reader skips to DESIGN.md changes without building vocabulary | High | Medium | Each chapter's prompt requires the vocabulary to write. Can't prompt correctly without reading. |
| Brutalist system changes invalidate specific prompts | Medium | Medium | Prompts are principled, not syntax-specific. Label the principle behind each prompt. |
| Reader's institution blocks code-based tools | Low | High | HTML/D3 runs in any browser. No institutional dependency. |
| Two-framework structure feels redundant (both frameworks say the same thing) | Medium | Low | They often do — and naming that convergence is a teaching moment, not a design flaw. |
| Chapter 9 (live vs. async) loses readers who only make live decks | Low | Low | Frame the choice as a decision to make once, not a problem to solve forever. |

**Top adoption risk:** Reader who uses the prompts without
reading the vocabulary. The prompt works but they cannot
explain why, and the next problem stumps them. Mitigation:
the diagnostic questions at the end of each chapter are the
real deliverable — the prompt is the demonstration that the
vocabulary was built.

---

### Market Size

This is a Brutalist series book. Market is the existing
Brutalist reader base plus the faculty/educator slide-maker
audience who discovers it through the series. Not a course
textbook adoption play — a direct sale to practitioners.

---

## PART 5 — OPEN QUESTIONS

| # | Question | Stakes | Owner | Status |
|---|---|---|---|---|
| 1 | How many before/after slide pairs per chapter? One extended pair or three quick pairs? | Chapter length and production effort | Author | **DECIDED: One extended pair per chapter. Depth over coverage. Consistent with the book's own pedagogy.** |
| 2 | Are the prompts written for the Brutalist system specifically or generalized for any AI slide tool? | Audience scope | Author | **DECIDED: Principles with Brutalist as demonstration. Prompts are portable. Brutalist is the reference implementation.** |
| 3 | Does Chapter 6 (Textbook Figure) require the Brutalist graphicacy book as background, or is it self-contained? | Prerequisite structure | Author | **DECIDED: Self-contained. Design perspective only — not which tool, not how to use the graphicacy book.** |
| 4 | Should the book include a "Diagnostic Checklist" as a final artifact? | Practitioner handbook usability | Author | **DECIDED: Yes. Chapter 12 — The Diagnostic Checklist. All 3–5 questions from all 11 chapters, one reference page.** |
| 5 | Does the book address AI-generated images on slides (Canva AI, DALL-E in decks)? | Aging risk and completeness | Author | **DECIDED: In scope, design perspective only — not which tool produced the image. No new chapter. Relevant chapters (4, 5, 6, 7) each acknowledge AI-generated images as a common trigger for that chapter's failure mode. One sentence in each "the feeling" section.** |

---

## PART 6 — CHANGELOG

| Version | Date | Change | Reason |
|---|---|---|---|
| 1.0 | 2026-05-13 | Initial TicTOC.md created from interactive /i1–/l3 intake | Full intake session complete |
| 1.1 | 2026-05-13 | Added Chapter 12 — The Diagnostic Checklist | Open Question 4 resolved: checklist as standalone reference artifact |
| 1.1 | 2026-05-13 | Prompts declared portable — principles first, Brutalist as demonstration | Open Question 2 resolved: broader audience, Brutalist is reference implementation not prerequisite |
| 1.3 | 2026-05-13 | All five Open Questions resolved | OQ1: one extended pair per chapter. OQ3: Chapter 6 self-contained, design perspective only. OQ5: AI-generated images in scope as design failure trigger, no new chapter, one sentence per relevant chapter (4, 5, 6, 7). |
| 1.4 | 2026-05-13 | Added Act One→Two interstitial between Chapters 6 and 7 | Final pre-draft item from /g2 audit resolved |

---

*TicTOC.md v1.4 — Complete. All open questions resolved. All /g2 fixes applied.*
*Ready to draft. Begin with Chapter 1 — The Slideument Problem.*
