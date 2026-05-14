---

## Acknowledgments

This book exists because faculty at three universities let me watch them fight with slides. They will go unnamed here because the diagnostic anecdotes in the chapters are anonymized composites of the patterns I saw across all of them — but the patterns are theirs, and I am in their debt.

Particular thanks to colleagues at Northeastern who tested the Brutalist system in their own teaching pipelines and pushed back on every chapter draft that drifted from practitioner to theory: the book is shorter and sharper because of them. Thanks also to the students of INFO 7375, INFO 7390, and the AI Fluency cohort, who watched me build the diagnostic vocabulary on their decks before it had a name.

The cognitive-science backbone — Sweller, Mayer, Tufte, Reynolds, Atkinson, Wiggins and McTighe — does the load-bearing work behind every chapter. The vocabulary belongs to them. The translation into slide-design diagnostics is what this book attempts.

---

## About the Author

**Nik Bear Brown** is an Associate Teaching Professor at Northeastern University's College of Engineering, where he teaches data science, AI, computational skepticism, and the design of AI-assisted production pipelines. He is the architect of the **Brutalist** system for AI-assisted creative production — a renderer-agnostic framework whose modules include *Brutalist D3 × Claude* (slide decks and graphicacy), *Brutalist After Effects × Claude*, *Brutalist Blender × Claude*, and *Brutalist Remotion × Claude*. The framework lives at [brutalist.art](https://www.brutalist.art/).

His PhD is in computer science from UCLA (computational and systems biology, with AI and statistics as minor fields). He holds master's degrees in Information Design and Data Visualization and in business administration from Northeastern. Before academia he worked as a molecular biologist at DNAX Research Institute and Cetus Corporation; he did a part-time postdoc at Harvard Medical School in deep learning while teaching at Northeastern.

He has built slides that did not work in front of thousands of students, which is the credential most relevant to this book. He writes at [nikbearbrown.com](https://www.nikbearbrown.com) and [skepticism.ai](https://www.skepticism.ai), and reaches at [bear@bearbrown.co](mailto:bear@bearbrown.co).

Pronouns: they/them. Fun fact: once ran away with the circus, worked as a photojournalist, did some sumo wrestling.

---

## Notes

### Chapter 1 — The Slideument Problem

1. The slideument coinage and its development is in Garr Reynolds's blog and *Presentation Zen* (Reynolds 2008/2019).
2. The NASA Columbia accident's PowerPoint slide is reproduced and analyzed in the Columbia Accident Investigation Board report, Volume 1, August 2003, and in Tufte's *The Cognitive Style of PowerPoint* (2003/2006).

### Chapter 2 — No Clear Hierarchy

1. Mayer's Signaling Principle is treated in *Multimedia Learning* (3rd ed., 2020); see also van Gog's chapter in the *Cambridge Handbook of Multimedia Learning*.
2. Bringhurst's modular type scales are in *The Elements of Typographic Style* (4th ed.).

### Chapter 3 — Too Much Text

1. The Coherence and Modality Principles are in Mayer 2020. Empirical anchor: Harp & Mayer 1997 / 1998 on coherence violations and learning.
2. Kosslyn's per-slide word-count work appears in *Clear and to the Point* (Oxford, 2007). The "≤6 words" Reynolds heuristic is practitioner consensus, not measured fact — practitioners should treat it as guidance.

### Chapter 4 — The Wrong Visual Form

1. Cleveland & McGill's perceptual-ranking study is "Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods," *Journal of the American Statistical Association* 79, no. 387 (1984): 531–554.
2. Tamara Munzner's taxonomy of visual encodings is in *Visualization Analysis and Design* (CRC Press, 2014).

### Chapter 5 — Color Is Doing Nothing (or Harm)

1. Web Content Accessibility Guidelines (WCAG) 2.1, especially Understanding 1.4.3 on contrast (minimum). APCA, the contrast algorithm proposed for WCAG 3.0, is noted but its normative status as of 2026 is `[verify]`.
2. ColorBrewer (Cynthia Brewer, Penn State) at [colorbrewer2.org](https://colorbrewer2.org).
3. Heer & Stone, "Color Naming Models for Color Selection, Image Editing and Palette Design," CHI 2012.

### Chapter 6 — The Textbook Figure on the Slide

1. Mayer's Pre-Training, Segmenting, and Spatial Contiguity Principles, *Multimedia Learning* 2020.
2. Colin Ware, *Information Visualization: Perception for Design* (4th ed., 2020).
3. OpenStax *Biology 2e*, §7.2 (glycolysis), used as the public-domain figure for the worked example.

### Chapter 7 — Seductive Details

1. Origin paper: Garner, Gillingham & White, "Effects of 'Seductive Details' on Macroprocessing and Microprocessing in Adults and Children," *Cognition and Instruction* 6 (1989): 41–57. (Sometimes mis-cited as "Garner & Brown 1989.")
2. Harp & Mayer 1998, "How Seductive Details Do Their Damage," *Journal of Educational Psychology* 90, no. 3: 414–434.
3. Meta-analysis: Rey 2012, "A Review and a Meta-Analysis of the Seductive Details Effect," *Educational Research Review* 7, no. 3: 216–237.

### Chapter 8 — The Deck That Covers But Doesn't Teach

1. Wiggins & McTighe, *Understanding by Design* (2nd ed., ASCD, 2005).
2. Karpicke & Roediger, "The Critical Importance of Retrieval for Learning," *Science* 319 (2008): 966–968.
3. Cepeda et al., "Distributed Practice in Verbal Recall Tasks: A Review and Quantitative Synthesis," *Psychological Bulletin* 132, no. 3 (2006): 354–380.

### Chapter 9 — Live Deck vs. Study Artifact

1. Mayer's Modality Principle, *Multimedia Learning* 2020.
2. Means et al. 2010, *Evaluation of Evidence-Based Practices in Online Learning*, U.S. Department of Education meta-analysis.
3. Atkinson, *Beyond Bullet Points* (4th ed., 2018).

### Chapter 10 — The Headline That Says Nothing

1. Garner & Alley 2013, "How the Design of Presentation Slides Affects Audience Comprehension," *International Journal of Engineering Education*.
2. Wolfe et al. 2024, *Journal of Business and Technical Communication* — recent replication across three populations.
3. Minto, *The Pyramid Principle* (3rd ed., 2009).

### Chapter 11 — Owning Your DESIGN.md

1. Brad Frost, *Atomic Design* (2016). Free online at [atomicdesign.bradfrost.com](https://atomicdesign.bradfrost.com).
2. W3C Design Tokens Community Group specification (first stable, October 2025) — note the normative status `[verify]` as of 2026.
3. Ellen Lupton, *Thinking with Type* (3rd ed., 2024).

### Chapter 12 — The Diagnostic Checklist

1. Atul Gawande, *The Checklist Manifesto* (Metropolitan Books, 2009).
2. Pronovost et al., "An Intervention to Decrease Catheter-Related Bloodstream Infections in the ICU," *New England Journal of Medicine* 355 (2006): 2725–2732. DOI 10.1056/NEJMoa061115.
3. Haynes et al., "A Surgical Safety Checklist to Reduce Morbidity and Mortality in a Global Population," *New England Journal of Medicine* 360 (2009): 491–499. DOI 10.1056/NEJMsa0810119.
4. Bosk et al., "Reality Check for Checklists," *The Lancet* 374, no. 9688 (2009): 444–445.

---

## References

Alley, Michael. *The Craft of Scientific Presentations*. 2nd ed. Springer, 2013.

Atkinson, Cliff. *Beyond Bullet Points: Using Microsoft PowerPoint to Create Presentations That Inform, Motivate, and Inspire*. 4th ed. Microsoft Press, 2018.

Bosk, Charles L., Mary Dixon-Woods, Christine A. Goeschel, and Peter J. Pronovost. "Reality Check for Checklists." *The Lancet* 374, no. 9688 (2009): 444–445.

Bringhurst, Robert. *The Elements of Typographic Style*. 4th ed. Hartley & Marks, 2013.

Brown, Peter C., Henry L. Roediger III, and Mark A. McDaniel. *Make It Stick: The Science of Successful Learning*. Belknap Press, 2014.

Cepeda, Nicholas J., Harold Pashler, Edward Vul, John T. Wixted, and Doug Rohrer. "Distributed Practice in Verbal Recall Tasks: A Review and Quantitative Synthesis." *Psychological Bulletin* 132, no. 3 (2006): 354–380.

Cleveland, William S., and Robert McGill. "Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods." *Journal of the American Statistical Association* 79, no. 387 (1984): 531–554.

Columbia Accident Investigation Board. *Report Volume 1*. NASA, August 2003.

Frost, Brad. *Atomic Design*. 2016. [atomicdesign.bradfrost.com](https://atomicdesign.bradfrost.com).

Garner, Ruth, Mark G. Gillingham, and C. Stephen White. "Effects of 'Seductive Details' on Macroprocessing and Microprocessing in Adults and Children." *Cognition and Instruction* 6 (1989): 41–57.

Garner, Joanna K., and Michael Alley. "How the Design of Presentation Slides Affects Audience Comprehension." *International Journal of Engineering Education* 29, no. 6 (2013).

Gawande, Atul. *The Checklist Manifesto: How to Get Things Right*. Metropolitan Books, 2009.

Harp, Shannon F., and Richard E. Mayer. "How Seductive Details Do Their Damage: A Theory of Cognitive Interest in Science Learning." *Journal of Educational Psychology* 90, no. 3 (1998): 414–434.

Haynes, Alex B., et al. "A Surgical Safety Checklist to Reduce Morbidity and Mortality in a Global Population." *New England Journal of Medicine* 360 (2009): 491–499.

Heer, Jeffrey, and Maureen Stone. "Color Naming Models for Color Selection, Image Editing and Palette Design." Proceedings of CHI 2012.

Karpicke, Jeffrey D., and Henry L. Roediger III. "The Critical Importance of Retrieval for Learning." *Science* 319 (2008): 966–968.

Kosslyn, Stephen M. *Clear and to the Point: 8 Psychological Principles for Compelling PowerPoint Presentations*. Oxford University Press, 2007.

Lupton, Ellen. *Thinking with Type: A Critical Guide for Designers, Writers, Editors, & Students*. 3rd ed. Princeton Architectural Press, 2024.

Mayer, Richard E. *Multimedia Learning*. 3rd ed. Cambridge University Press, 2020.

Means, Barbara, Yukie Toyama, Robert Murphy, Marianne Bakia, and Karla Jones. *Evaluation of Evidence-Based Practices in Online Learning: A Meta-Analysis and Review of Online Learning Studies*. U.S. Department of Education, 2010.

Minto, Barbara. *The Pyramid Principle: Logic in Writing and Thinking*. 3rd ed. Pearson, 2009.

Munzner, Tamara. *Visualization Analysis and Design*. CRC Press, 2014.

Pronovost, Peter, et al. "An Intervention to Decrease Catheter-Related Bloodstream Infections in the ICU." *New England Journal of Medicine* 355 (2006): 2725–2732.

Rey, Günter Daniel. "A Review and a Meta-Analysis of the Seductive Details Effect." *Educational Research Review* 7, no. 3 (2012): 216–237.

Reynolds, Garr. *Presentation Zen: Simple Ideas on Presentation Design and Delivery*. 3rd ed. New Riders, 2019.

Sweller, John, Paul Ayres, and Slava Kalyuga. *Cognitive Load Theory*. Springer, 2011.

Tufte, Edward R. *The Cognitive Style of PowerPoint: Pitching Out Corrupts Within*. 2nd ed. Graphics Press, 2006.

Tufte, Edward R. *The Visual Display of Quantitative Information*. 2nd ed. Graphics Press, 2001.

Ware, Colin. *Information Visualization: Perception for Design*. 4th ed. Morgan Kaufmann, 2020.

Wiggins, Grant, and Jay McTighe. *Understanding by Design*. 2nd ed. ASCD, 2005.

Wolfe, Joanna, Vasanth Shanmugaraj, Lisa Reineke, Maria Caton Peet, and Anne Moreau. "Assertion-Evidence Slide Structure Across Engineering, Computer Science, and Medical Student Populations." *Journal of Business and Technical Communication* (2024).

---

## On the Absence of an Index

This is a Kindle and online book. It does not include a printed index. Three reasons.

First, e-reader search makes printed indexes obsolete for this format — every term in the book is one keystroke away, with results that scale to your reading window rather than to a static page count. Second, this book is integrated with **Medhavy** ([medhavy.com](https://www.medhavy.com/)) — मेधावी, from the Sanskrit for *intelligent* or *intellectually brilliant* — an AI-powered intelligent textbook platform that indexes the book semantically rather than alphabetically. Search Medhavy for a diagnostic question and it will surface the chapter that teaches the question, not the page where the term first appears. Third, the diagnostic vocabulary is short enough that the table of contents and the chapter 12 checklist together already serve as a working index.

If you need to find something, search the e-reader. If you need to *use* something, open chapter 12.

---

## Glossary

**Assertion-Evidence (AE) structure.** Slide design where the headline asserts the slide's claim and the body provides supporting evidence. Atkinson 2018; Garner & Alley 2013. *Opposite of:* topic-label headlines.

**Coherence Principle.** Mayer's finding that adding non-essential material to a multimedia lesson decreases learning, even when the material is interesting. The cognitive basis for the seductive-details chapter (Ch 7).

**Cognitive Load Theory (CLT).** Sweller's framework distinguishing intrinsic load (the difficulty of the content), extraneous load (cognitive effort caused by poor design), and germane load (productive effort that builds schemas). Design's job is to reduce extraneous load.

**DESIGN.md.** The persistent visual-rules file in the Brutalist system. Holds palette, typography, spacing, density limits, and mode toggles (live vs. study). Loaded by the model when visual decisions are in scope. Yours to own.

**Diagnostic question.** A question the reader applies to any slide to detect a specific failure mode. Twenty-four total across the book, collected in Chapter 12.

**Do-confirm checklist.** A checklist run after the work is done, to confirm nothing was missed. Brutalist's slide checklist is do-confirm. (*Contrast:* read-do, where each item is performed in order as it is read.)

**Modality Principle.** Mayer's finding that spoken narration + visual beats on-screen text + visual for complex material — the verbal channel does not have to do two jobs at once. The cognitive basis for the live-deck vs. study-artifact distinction (Ch 9).

**Multimedia Principle.** Mayer's foundational finding: words + pictures outperforms words alone. The cognitive basis for choosing the right visual form (Ch 4).

**Redundancy Principle.** Mayer's finding that on-screen text + identical narration reduces learning compared to narration alone. The cognitive basis for the slideument failure (Ch 1).

**Seductive details.** Engaging-but-irrelevant material added to a lesson. Decreases learning even when memorable. Origin: Garner, Gillingham & White 1989. Foundational mechanism paper: Harp & Mayer 1998.

**Segmenting Principle.** Mayer's finding that learners process content better when it is broken into smaller, learner-paced segments rather than presented continuously.

**Signaling Principle.** Mayer's finding that visual cues directing attention to the most important content improve learning. The cognitive basis for typographic hierarchy (Ch 2) and meaningful color encoding (Ch 5).

**Slideument.** Garr Reynolds's term for a slide that tries to be both a speaker's anchor and a self-contained document, and fails at both. Originating sin of academic decks.

**WCAG contrast minimum.** Web Content Accessibility Guidelines 2.1 specifies a 4.5:1 contrast ratio for normal text (3:1 for large text) as the AA threshold. Used in Ch 5 as the floor for slide text contrast.

---

## Errata

Reported errors and corrections are maintained at [nikbearbrown.com/brutalist-slides-errata](https://www.nikbearbrown.com) (link will be active after publication).

To report an error, contact: [bear@bearbrown.co](mailto:bear@bearbrown.co).
