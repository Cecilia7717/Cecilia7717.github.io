---
title: "Use of Control Flow Graphs with Edge Consideration for Fault Localization"
collection: projects
type: "Summer project"
permalink: /projects/debugging-visualization
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
slideurl: "http://cecilia7717.github.io/files/CAPWIC.pdf"
paperurl: "http://cecilia7717.github.io/files/Debugging_VisualizationSCAM.pdf"
---

Improved the accuracy of 16.9% real faults tested with modifying the existing fault localization techniques by working with larger data sets and test cases and analyzed the difference.

Overview
======

Locating faults during software development is a time-consuming and costly process that often involves extensive testing by trying many different inputs and analyzing their outputs, which can be very expensive in terms of both time and money. Helping developers narrow their searches by selecting suspicious statements becomes important, where “suspicious” refers to code entities that are more likely to be responsible for observed failing test cases, i.e. those containing the fault. My research addresses this real-world challenge by improving debugging efficiency through more precise and informative fault localization techniques. 

Building on the foundations of Spectrum-Based Fault Localization (SBFL), I introduced an innovative extension, Tarantula+Edges, which uses Control Flow Graphs (CFGs) to help developers identify suspicious lines of code with improved accuracy. This approach incorporates CFG edges, focusing on branches and decision points, which allows it to detect faults in conditional statements — an area where traditional SBFL often struggles. In Tarantula+Edges, suspiciousness scores are calculated for both individual statements and the edges connecting them, enabling the tool to provide a clearer, path-oriented view of potential faults in code.

Additionally, I adapted this technique with Ochiai+Edges, applying the same CFG-edge considerations to enhance another well-known SBFL approach. Through experiments with both Tarantula+Edges and Ochiai+Edges, my research demonstrated that the integration of CFG edge analysis allows for more accurate fault localization, particularly in methods with complex decision logic. This dual approach not only highlights the most suspicious statements but also makes debugging paths through the code more transparent, directing engineers’ attention to the highest-probability areas of failure. Through rigorous testing on real-world software faults from the Defects4J benchmark and Java methods in the Apache Commons Math library, I demonstrated that this CFG-based technique enables developers to isolate faults more efficiently by focusing on the most suspicious paths in the code.

Ultimately, my work with Tarantula+Edges and Ochiai+Edges illustrates how CFG-based visualizations can significantly reduce the time and effort developers spend on fault localization by highlighting error-prone paths in the code. Moving forward, I am committed to refining these techniques, exploring further data-flow considerations and enhancing the interpretability of fault localization visualizations. By developing tools that reflect the intricacies of real-world software, I aim to bridge the gap between theoretical debugging methods and practical, user-friendly applications that make fault localization more efficient and accessible.
