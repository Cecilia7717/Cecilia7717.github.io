---
title: "Automated Software Analysis and Test Generation"
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

This project enhances spectrum-based fault localization by incorporating **control-flow-graph (CFG) edge information**, addressing a major limitation of traditional SBFL techniques that rely solely on node-level coverage. I designed the **+Edges extension**, which augments eight widely used SBFL formulas with edge traversal data, enabling the analysis to capture branch frequency, divergence, and structural bottlenecks that often distinguish passing and failing executions. The goal is to more accurately model how faults manifest in conditional logic and multi-path control structures—scenarios where node-only approaches frequently mis-rank the true root cause.

To validate the method, I conducted a **large-scale evaluation on 262 real-world faults** from the Defects4J benchmark with **9 state-of-the-art SBFL techniques**. Across the board, edge-aware reasoning improved accuracy metrics, with particularly strong gains in branch-intensive programs; for instance, **Sørensen+Edges achieved a 55.8% improvement in Mean First Rank**. This research resulted in the paper *Use of Control Flow Graphs with Edges Consideration for Fault Localization* (Chen & Murphy, 2025), presented at **CAPWIC 2025**, and the full manuscript is currently under submission.
