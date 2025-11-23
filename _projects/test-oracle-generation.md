---
title: "Automated Exceptional Test Oracle Generation"
order: 5
collection: projects
type: "REU project"
permalink: /projects/test-oracle-generation
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
---

Investigated how to automatically generate accurate test oracles for real-world exceptional bugs by combining traditional oracle-generation tools with LLM-based reasoning.

Overview
======

This project focuses on the automated generation of test oracles for exceptional bugs—cases where program executions diverge not through assertion failures but through subtle exception-triggering conditions that many automated tools fail to capture. Through a systematic study of TOGA, TOGLL, and EditAS2 across real-world bugs from Defects4J, I found that TOGLL’s performance on exceptional bugs drops by 38.88% compared to its accuracy across all bug categories. This quantitative gap underscores how poorly existing tools model exception semantics and suggests that new techniques are needed to handle complex control-flow paths, implicit precondition violations, and context-specific error states.

To address these limitations, I engineered prompting strategies for large language models to produce more precise oracle predictions, emphasizing semantic reasoning about program state rather than pattern matching. I integrated Claude and xAI via the Model Context Protocol (MCP) to automatically classify fault types and analyze oracle quality, creating a pipeline that systematically inspects LLM reasoning behaviors across diverse failure patterns. Beyond improving accuracy, this framework provides a clearer understanding of why certain exceptional conditions are missed and how LLMs can supplement traditional tools for more robust automated testing.
