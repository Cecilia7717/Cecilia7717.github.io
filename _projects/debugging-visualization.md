---
title: "Use of Control Flow Graphs with Edge Consideration for Fault Localization"
order: 6
collection: projects
type: "REU project"
permalink: /projects/debugging-visualization
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
paperurl: 'http://cecilia7717.github.io/files/Debugging_Visualization_SCAM.pdf'
slidesurl: 'http://cecilia7717.github.io/files/slides1.pdf'
---

Developed an edge-augmented fault-localization framework that integrates CFG branch behavior into SBFL techniques, yielding substantial accuracy improvements on real-world bugs.

Overview
======

This project enhances spectrum-based fault localization by incorporating **control-flow-graph (CFG) edge information**, addressing a major limitation of traditional SBFL techniques that rely solely on node-level coverage. I designed the **+Edges extension**, which augments eight widely used SBFL formulas with edge traversal data, enabling the analysis to capture branch frequency, divergence, and structural bottlenecks that often distinguish passing and failing executions. The goal is to more accurately model how faults manifest in conditional logic and multi-path control structures—scenarios where node-only approaches frequently mis-rank the true root cause.

To validate the method, I conducted a **large-scale evaluation on 262 real-world faults** from the Defects4J benchmark with **9 state-of-the-art SBFL techniques**. Across the board, edge-aware reasoning improved accuracy metrics, with particularly strong gains in branch-intensive programs; for instance, **Sørensen+Edges achieved a 55.8% improvement in Mean First Rank**. This research resulted in the paper *Use of Control Flow Graphs with Edges Consideration for Fault Localization* (Chen & Murphy, 2025), presented at **CAPWIC 2025**, and the full manuscript is currently under submission.
