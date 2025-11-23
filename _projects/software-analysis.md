---
title: "Evaluation of Test Generation Tools on Defects4J Bugs"
collection: projects
type: "REU project"
permalink: /projects/software-analysis
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
paperurl: 'http://cecilia7717.github.io/files/software.pdf'
---

Evaluated and improved automated test-generation techniques by analyzing how EvoSuite and EditAS2 perform on real Defects4J Time bugs, identifying coverage gaps and proposing domain-aware strategies to better detect semantic and time-dependent faults.

Overview
======

This project examines how automated software testing tools behave when confronted with real-world time-handling bugs. I analyzed **EvoSuite** and **EditAS2** on the Defects4J *Time* project, which contains 12 faults involving exception safety, date-handling semantics, DST behavior, calendar calculations, and chronology inconsistencies. EvoSuite frequently achieved high coverage—often **above 93% line and 97% condition coverage**—yet still failed to trigger many semantic bugs. For instance, EvoSuite executed Time-7’s `parseInto()` method but never generated leap-day inputs, instead producing nonsensical strings like `"/2i({p{]:$bw"` (Figure 21). Similarly, for Time-8, EvoSuite ran the buggy method but never generated the minute values **−59 to −1** required to manifest the bug. In contrast, EvoSuite successfully detected simpler functional faults such as Time-9 by generating `(45, 45)`, which returned a malformed string `"+45:45"` instead of throwing an exception.

On the oracle side, **EditAS2** frequently produced invalid or semantically irrelevant assertions—for example, calling `getValue()` with no index (Time-4), using unsupported Hamcrest matchers (Time-12), or producing meaningless equality comparisons for exception-based bugs (Time-1, Time-2). These issues highlight why assertion generation fails on safety and semantic faults where exception contracts, not value comparisons, define correctness. Based on these findings, I proposed two improvements: **domain-aware exception templates** that default to `assertThrows(...)` when prefixes reveal missing safety checks, and **domain-aware input-seeding heuristics** to guide EvoSuite toward meaningful values such as leap-year dates, DST transition timestamps, or semantically overlapping DateTimeFieldTypes. These results demonstrate the limitations of current automated test-generation tools and point toward practical pathways for improving their effectiveness.
