# Brutalist: Using D3 and HTML to Make Slide Decks

**Nik Bear Brown** · Bear Brown, LLC · 2026

*A practitioner's handbook for faculty who use AI tools to make slides and can't yet say what is wrong with the output.*

---

## What this book is

AI slide tools — Canva, Gamma, Beautiful.ai, the Brutalist system — produce decks the user cannot improve because the user lacks the language to say what to change. This book builds that language. Twelve short chapters teach the twelve most common failure modes in academic decks, each diagnosed with one cognitive-science question (Sweller, Mayer, Reynolds) and one visual-design question (Tufte, Bringhurst, Atkinson). Every chapter ends with a paste-able prompt for the Brutalist system and a `DESIGN.md` change that prevents the failure from recurring.

The central argument: **you can't prompt precisely if you can't see precisely.** This book builds the seeing.

Read it cover to cover the first time — about six hours of reading total — to build the eye. Then keep Chapter 12 (the diagnostic checklist) at hand and run it before every deck ships.

## Who it is for

Faculty members who teach with slides. PhDs in their field, novices in design. Comfortable enough with the Brutalist code system to use it, or willing to learn. No prior D3 expertise required.

## Who it is not for

Designers (the vocabulary is theirs). Instructional designers (likewise). Faculty who do not use AI slide tools at all (the book assumes a tool in the loop). Readers looking for accessibility law (Chapter 5 covers contrast ratios — that is the scope).

## Table of Contents

**Front matter**
- Title page · Copyright · Dedication · Preface

**Chapter 0 — Introduction**
The 11:42 p.m. faculty member, the central argument, the chapter map, a note about AI.

**Act One — Building the eye on individual slide problems**

| # | Title | Diagnostic move |
|---|-------|-----------------|
| 1 | The Slideument Problem | Speaker's anchor vs. self-contained document |
| 2 | No Clear Hierarchy | Where does the eye land first? |
| 3 | Too Much Text | Can a student read and listen at once? |
| 4 | The Wrong Visual Form | Does the form match the content's structure? |
| 5 | Color Is Doing Nothing (or Harm) | Does each color encode meaning? |

**Act Two — From slide to deck**

| # | Title | Diagnostic move |
|---|-------|-----------------|
| 6 | The Textbook Figure on the Slide | Designed for slide or designed for textbook? |
| 7 | Seductive Details | Is anything non-essential to the objective? |
| 8 | The Deck That Covers but Doesn't Teach | What should the student be able to do? |
| 9 | Live Deck vs. Study Artifact | Speaker's anchor or self-contained explanation? |
| 10 | The Headline That Says Nothing | Is the headline a claim or a label? |
| 11 | Owning Your DESIGN.md | The system you receive vs. the system you own |
| 12 | The Diagnostic Checklist | All twenty-four questions, do-confirm |

**Back matter**
- Acknowledgments · About the Author · Notes (per chapter) · References · On the Absence of an Index · Glossary · Errata

## About the Author

**Nik Bear Brown** is an Associate Teaching Professor at Northeastern University's College of Engineering. He teaches data science, AI, computational skepticism, and the design of AI-assisted production pipelines, and is the architect of the **Brutalist** system for AI-assisted creative production — the renderer-agnostic framework whose modules include the D3 / slide-deck book in your hands, *Brutalist After Effects × Claude*, *Brutalist Blender × Claude*, and *Brutalist Remotion × Claude*. PhD in computer science (UCLA), with master's degrees in Information Design and Data Visualization and in business administration from Northeastern. He writes at [nikbearbrown.com](https://www.nikbearbrown.com) and reaches at [bear@bearbrown.co](mailto:bear@bearbrown.co).

## How to read this book

Cover to cover, in order, the first time. Each chapter compounds on the previous; reading out of order works for reference but not for building the diagnostic eye. The chapters are short — twenty to thirty minutes each. Sections 4–7 of each chapter (the before/after pair, the paste-able prompt, the `DESIGN.md` change) are the load-bearing ones. If you skim, skim everything else; do not skim those four.

After the first read, keep Chapter 12 (the diagnostic checklist) at hand. Run it once per deck before you ship. The checklist is the chapter you carry. The earlier chapters teach you what the questions mean.

## Companion: Medhavy

This book integrates with **Medhavy** ([medhavy.com](https://www.medhavy.com/)) — मेधावी, from the Sanskrit for *intelligent* — an AI-powered intelligent textbook platform that indexes the book semantically. Search Medhavy for a diagnostic question and it will surface the chapter that teaches it. Come learn something with us.

## Companion: Brutalist

The Brutalist system documentation lives at [brutalist.art](https://www.brutalist.art/). This book is the diagnostic-vocabulary layer; the system is the cheap-iteration loop that turns diagnoses into rendered slides. You do not need to use Brutalist to get value from this book — the diagnostic questions transfer to any AI slide tool — but the book's prompts are written against Brutalist's `DESIGN.md` conventions.

## Copyright

Copyright © 2026 Nik Bear Brown. All rights reserved.

Published by Bear Brown, LLC.

No part of this publication may be reproduced, distributed, or transmitted in any form or by any means without the prior written permission of the publisher, except in the case of brief quotations in critical reviews and certain other noncommercial uses permitted by copyright law. See [LICENSE.md](./LICENSE.md) for full terms.

ISBN: [INSERT ISBN]
First edition: 2026.

## Contact

Permissions inquiries · Errata · Adoption discussions: [bear@bearbrown.co](mailto:bear@bearbrown.co)

---

## Who This Book Is For

This is a book for faculty who teach with slides. Not for designers. Not for instructional-design specialists. Not for the eight people in your department who already read Tufte. It is for the historian, the chemist, the political scientist, the engineer, the literature professor — anyone who has slides to make for tomorrow and no design training. You know your field. You do not yet have a name for what is wrong with the deck. That is what is being taught here.

---

## How to Read It

Twelve chapters in two acts. Act One (chapters 1–5) trains the eye on individual slide problems. Act Two (chapters 6–11) moves from slide-level diagnosis to deck-level structure. Chapter 12 is the diagnostic checklist — the reference artifact you keep after the rest of the book has done its work.

**Act One — building the eye:**

- **Chapter 1, The Slideument Problem.** A deck that is exhausting to lecture from and useless to study from. Reynolds's term. The deck does not know what it is for.
- **Chapter 2, No Clear Hierarchy.** A slide where every element competes for attention. Mayer's Signaling Principle and Bringhurst's typographic hierarchy.
- **Chapter 3, Too Much Text.** A textbook paragraph pasted onto a slide. Mayer's Coherence and Modality Principles.
- **Chapter 4, The Wrong Visual Form.** Bullets where a 2×2 matrix would communicate instantly. Cleveland and McGill on perceptual ranking.
- **Chapter 5, Color Is Doing Nothing (or Harm).** Decoration where there should be encoding. WCAG contrast and ColorBrewer.

**Act Two — from slide to deck:**

- **Chapter 6, The Textbook Figure on the Slide.** A figure that worked in a textbook fails on a slide. Different reading conditions.
- **Chapter 7, Seductive Details.** The stock photo, the fun fact, the quirky cartoon — engagement that reduces learning. Harp and Mayer 1998.
- **Chapter 8, The Deck That Covers but Doesn't Teach.** A sixty-slide deck that touches every topic and builds no capability. Wiggins and McTighe on backward design.
- **Chapter 9, Live Deck vs. Study Artifact.** One deck cannot be both. The fix is producing two artifacts from one source.
- **Chapter 10, The Headline That Says Nothing.** "Introduction." "Methods." "Results." Topic labels are not claims. Atkinson on assertion-evidence.
- **Chapter 11, Owning Your DESIGN.md.** The meta-chapter. The vocabulary becomes your design system. The Brutalist defaults are starting points, not verdicts.
- **Chapter 12, The Diagnostic Checklist.** All twenty-four questions on one page. Do-confirm. Run it before every deck ships.

---

## Signature Simulations

<!-- TODO: populate from chapter content -->

---

*"You can't prompt precisely if you can't see precisely — this book builds the seeing."*
