---
title: "Course Scheduling Optimization with "
order: 1
collection: projects
type: "REU project"
permalink: /projects/algorithm-compare
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
paperurl: 'http://cecilia7717.github.io/files/alg.pdf'
---

Built and analyzed an end-to-end course scheduling system that optimizes classroom assignments, timeslots, and student enrollments, combining algorithm design, theoretical runtime analysis, and real Registrar data. :contentReference[oaicite:1]{index=1}

Overview
======

This project focuses on designing and analyzing an end-to-end scheduling algorithm that assigns classrooms, time slots, and student enrollments under realistic constraints. I implemented a baseline algorithm that ranks classes by popularity, schedules them into the largest suitable rooms, and then assigns each student four non-conflicting courses drawn from their preference lists. The algorithm’s worst-case runtime, \(O(r^2 t + s + c\log c)\), was derived analytically and then experimentally validated with large synthetic datasets. As shown in the scatterplots and regression results (pp. 5–8), the number of students \(s\) overwhelmingly determines runtime, while the number of rooms, classes, and time slots contributes minimally.

To extend the method beyond synthetic settings, I adapted the algorithm to real Bryn Mawr and Haverford Registrar data, addressing key challenges such as missing instructor assignment, non-uniform preference list lengths, and overlapping time periods. I then implemented and compared five enhancement strategies—greedy and dynamic-programming filters for non-overlapping timeslots, an independent-set formulation for maximal timeslot selection, a popularity–conflict hybrid ranking of classes, and a simulated-annealing post-optimization to repair conflict-heavy schedules. These approaches produced measurable improvements in scheduling quality, with independent-set and simulated annealing achieving the strongest performance (pp. 13–18). Full analysis and pseudocode are available in the project report.
