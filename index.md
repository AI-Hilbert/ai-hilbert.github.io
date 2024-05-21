---
title: AI-Hilbert
---


<p align="right">
 <a href="https://ai-hilbert.github.io/authors"> About the authors 👤 👤 👤 </a>
</p>
<p align="right">
 <a href="https://ai-hilbert.github.io/references"> References and Videos 📖 📚 🎦 </a>
</p>
<p align="right">
 <a href="https://github.com/IBM/AI-Hilbert"> Code and Data  <img height="30" width="30" src="figures/github.svg" /> </a>
</p>

<br clear="left"/>

## APOLOGIES FOR THE APPEARANCE! THIS WEBSITE IS STILL WORK IN PROGRESS
It will be ready soon!

## AI-Hilbert overview


A fundamental challenge in science is explaining natural phenomena in a manner consistent with both noisy experimental data and background knowledge about the universe's laws. 
While the Scientific Method has historically driven significant progress, the rate of new discoveries and their economic contributions have stagnated despite increased investment. Figures like Dirac have noted the increasing difficulty of making groundbreaking discoveries, and research indicates a decline in the marginal value of scientific discoveries over time. This stagnation suggests that the "low-hanging fruit" of science—simple laws involving low-degree polynomials—has largely been picked, necessitating more sophisticated approaches. 
Simultaneously, advances in global optimization methods have made it possible to explore the space of scientific laws more efficiently. 
Leveraging these advances, we propose AI-Hilbert, a new approach that integrates background knowledge and experimental data to derive consistent scientific laws articulated as polynomial equalities and inequalities. 
Unlike existing methods that may produce inconsistent or spurious results, AI-Hilbert uses polynomial optimization to derive laws that are formally provable and consistent with both theoretical and empirical data. 
This method minimizes discrepancies between proposed laws and experimental data while ensuring consistency with background theory, providing formal proofs of correctness. 
AI-Hilbert is scalable, operating in polynomial time in the number of variables and axioms, and requires less data than purely data-driven methods due to its use of background knowledge to restrict the search space. 

<p align="center">
<img src="figures/scientific_method_comparison_box.png" width="500"/>
</p>

The scientific discovery community has traditionally relied on classical methods or data-driven techniques for making discoveries. Our proposed AI-Hilbert system introduces a novel approach by proposing scientific laws that are consistent with a background theory, formally expressed through polynomial equalities and inequalities. This integration allows AI-Hilbert to make scientific discoveries with fewer data points compared to state-of-the-art methods. In contrast, existing approaches often yield laws that may be inconsistent with either the background theory or the data. To illustrate the difference we presents a stylized version of the scientific method, showing how new laws are proposed from background theory and experimental data using classical techniques, data-driven methods, or AI-Hilbert. While data-driven discoveries might conflict with background theory, and classical methods may overlook relevant data, AI-Hilbert ensures consistency with both. 

<p align="center">
<img src="figures/scientific_method_flowchart.png" width="500"/>
</p>


### The Method

Our method, AI-Hilbert, seeks to discover an unknown polynomial formula that describes a physical phenomenon while aligning with both a background theory of polynomial equalities and inequalities (B) and a set of experimental data (D). 
This method involves a multi-step algorithm, where the inputs include B, D, constraints and bounds (C) dependent on hyperparameters (Λ), and a distance function (dc) defining the distance from a polynomial to the background theory. 
Initially, AI-Hilbert formulates a polynomial optimization problem targeting a specific concept identified by a dependent variable, integrating the background theory, data, and constraints. 
It then reformulates this problem into a semidefinite optimization problem, solving it using a mixed-integer conic optimization solver. 
The output is a candidate formula representing the phenomenon, excluding unobserved variables and accompanied by multipliers providing certificates of its derivability from the background theory. 
This approach ensures that the derived formula is consistent with both the observed data and the underlying scientific principles encapsulated in the background theory.

<p align="center">
<img src="figures/Figure1.png"  width="500"/>
</p>


### When the theory is enough
AI-Hilbert successfully derives valid scientific laws
solely from a complete and consistent background theory. Namely, by deriving the Hagen-
Poissuille Equation (Section 3.3) and deriving the Radiated Gravitational Wave Power Equation
(Section 3.4). 

<p align="center">
<img src="figures/animated1.gif"  alt="" width="230"/>
<img src="figures/animated2.gif"  alt="" width="400"/>
</p>

### Using the data to refine the theory

we demonstrate that AI-Hilbert is capable of deriving a valid scientific law
from an inconsistent yet complete background theory. We illustrate this capability through two
scenarios: Firstly, when two axioms in the background theory contradict each other (Section 3.5),
by using measurement data to discern the correct axiom. Secondly, where an incorrect candidate
formula is incorporated into a complete and consistent background theory (Section 3.6). In both
cases, we use real-life, noisy, experimental data

<p align="center">
<img src="figures/time.gif"  alt="" width="600"/>
</p>

### Using the data to compensate incomplete knowledge

demonstrate that AI-Hilbert successfully derives a valid scientific law from an
incomplete yet consistent background theory and experimental data. Specifically, we demonstrate
that AI-Hilbert is data-efficient, in the sense that as the number of axioms supplied increases,
less data is required to successfully derive a scientific law.

<p align="center">
<img src="figures/Distance_vs_noise_kepler_noiselesscase_allaxiomsmissing.png"  width="300"/>
&emsp;&emsp;
<img src="figures/Distance_vs_noise_kepler_noiselesscase_axiom1missing.png"  width="300"/>
</p>


### Conclusions and Limitations

