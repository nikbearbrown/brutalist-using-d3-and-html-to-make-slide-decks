# Brutalist: Using D3 and HTML to Make Slide Decks

**Nik Bear Brown**

---

## Copyright

Copyright © 2026 Nik Bear Brown. All rights reserved.

Published by Bear Brown, LLC.

No part of this publication may be reproduced, distributed, or transmitted in
any form or by any means without the prior written permission of the publisher,
except in the case of brief quotations in critical reviews and certain other
noncommercial uses permitted by copyright law.

ISBN: [INSERT ISBN]

First edition: 2026

For permissions inquiries: bear@bearbrown.co

---

## Dedication

*For the faculty member at 11:42 p.m., still up, still fighting the deck. You already know what's wrong. You just don't have the words for it yet.*

---

## Preface

This book exists because I kept watching the same scene play out, in my own office and in the offices of colleagues at three universities, year after year. A faculty member with twenty years of expertise in their field opens Canva, or Gamma, or Beautiful.ai, types a prompt — "make slides about the Krebs cycle" or "lecture on confounding variables" — and gets back something that looks fine. Looks polished. Looks professional. And they know, immediately, that it isn't right.

Then they sit there for forty minutes trying to fix it.

The fix never lands. They drag a text box. Recolor a heading. Cut a bullet. Add an image. Move it. Delete the image. Adjust the spacing. None of the adjustments compound, because none of them are aimed at the actual failure. The faculty member feels the slide is wrong. They can't say *why*, and so they can't say *what would make it right* — to themselves, to the AI tool, or to a designer if they had one. The result is exhaustion and a deck that is still wrong.

That is the gap this book closes.

The gap is not about design talent. It is about **diagnostic vocabulary**. Designers have a vocabulary for what is wrong with a slide. Cognitive scientists have a different vocabulary, also useful, for what is wrong with a slide. Faculty members are experts in their field but have rarely been given either vocabulary. So they make slides by paraphrasing textbooks, watch the slides not work, and have no language to say what failed.

The vocabulary is not hard. It is two questions per slide. *Cognitive science: is the verbal channel doing two jobs at once?* *Visual design: where does the eye land first, and is that the most important thing?* Twelve chapters in this book teach the twelve most common failure modes I have seen in academic decks, each with its own pair of diagnostic questions. The book is not theoretical. It is a practitioner's handbook for noticing what is wrong, and a set of prompts you can paste into the **Brutalist** system — a renderer-agnostic framework for AI-assisted creative production — to fix it.

I wrote this book now because three things converged. First, AI slide tools have crossed the threshold where the bottleneck is no longer generation — it is improvement. The output is good enough that the friction has moved upstream, into the question of *what to ask for*. Second, faculty are being asked to teach more, prepare more, and re-cover the same material in live and asynchronous formats simultaneously, while their slide budget shrinks. Third, the cognitive-science literature on multimedia learning — Sweller, Mayer, Reynolds, Tufte — has matured to the point where the rules are stable, replicable, and ready to be used. The pieces are on the table. What is missing is the bridge: a working vocabulary that lets a faculty member look at a slide and say, *that.*

I am qualified to write this book because I have failed at slides in public for over a decade. I teach data science, AI, and visualization at Northeastern University. I have built courses on AI fluency, branding-and-AI, and computational skepticism. I have given lectures with slides that did not work, watched students try to study from decks that could not be studied from, and rebuilt the same content three different ways to find out what changed. I co-built the Brutalist system because making the fix cheap is the difference between *I would change this if it were easy* and *let me just change it*. The book teaches the seeing; the system handles the doing.

This book does **not** teach you to make pretty slides. It does not teach you to use Brutalist (the system documentation lives elsewhere — see [brutalist.art](https://www.brutalist.art/)). It does not teach you cognitive science as an academic subject, design history, or accessibility law. It teaches a small, specific, transferable skill: the trained eye that knows what to tell the system to change.

If you finish this book and your DESIGN.md ends up looking different from the Brutalist defaults, that is the book working as intended. The book is prescriptive about the questions. It is not prescriptive about the answers.

— Nik Bear Brown
Boston, 2026
