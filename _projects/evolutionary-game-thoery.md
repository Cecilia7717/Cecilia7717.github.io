---
title: "The Evolutionary Dynamics of Machine Learning Techniques on Spam Filter"
order: 4
collection: projects
type: "REU project"
permalink: /projects/evolutionary-game-thoery
venue: "Bryn Mawr College"
location: "Bryn Mawr, PA, USA"
papersurl: 'http://cecilia7717.github.io/files/egt.pdf'
---

Analyzed the co-evolution of spam filters and spammers using evolutionary game theory, combining Nash/ESS analysis with spatial grid simulations to model attacker–defender dynamics.

Overview
======

This project investigates the arms race between spam filters and adversarial spammers through the lens of evolutionary game theory. Using payoff matrices derived from classifier performance and evasion effectiveness, I computed Nash equilibria and evolutionarily stable strategies (ESS) for both the defender population (Naive Bayes vs. SVM) and the attacker population (“Adding good words” vs. “Not adding”). The theoretical analysis shows that while SVM often emerges as the best classifier response, spammer strategies remain evolutionarily unstable, continually shifting to exploit weaknesses—an insight consistent with the endless adaptation cycle described in the literature.

To capture local propagation effects, I implemented spatial evolutionary simulations on 5×5 and 6×6 grids. These experiments show how strategies spread through imitation of high-payoff neighbors, producing patterns such as sustainable cooperative clusters (representing successful evasion tactics), unstable oscillations between attacker strategies, and rapid domination when multiple coordinated invaders seed the population. These findings illustrate how attacker–defender behavior evolves not only in aggregate populations but also in spatially structured settings, revealing why spam filtering remains a fundamentally dynamic and adversarial ecosystem. A detailed analysis, figures, and code outputs are available in the final report.
