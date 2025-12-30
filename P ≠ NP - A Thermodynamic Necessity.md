P ≠ NP: A Thermodynamic Necessity?
The Thermodynamic Incompleteness Conjecture and the Computational Action Conservation
Principle
Renaud Glimois
Independent Researcher
renaud.glimois@laposte.net
December 202 5
Abstract
We propose a thermodynamic reformulation of the P vs NP problem, suggesting that the
separation P ≠ NP may be a physical necessity rather than a mathematical accident. By
translating computational complexity into the language of information thermodynamics, we
derive a Computational Action Conservation Principle from known physical laws
(Thermodynamic Speed Limits, Thermodynamic Uncertainty Relations, and Landauer's
principle). This principle states that producing an object of high logical depth in short time
requires exponentially increasing energy dissipation. If solutions to NP-complete problems
possess exponential logical depth—a conjecture we term the Glimois Conjecture—then P ≠
NP follows as a theorem of physics. We propose an experimental protocol using optically
trapped colloidal systems to test this prediction. This work does not prove P ≠ NP in the
classical mathematical sense, but suggests a new research direction linking computational
complexity to fundamental physics.
Keywords: P vs NP, computational complexity, information thermodynamics, Landauer
principle, logical depth, Kolmogorov complexity
1. Introduction
The P vs NP problem, designated by the Clay Mathematics Institute as one of the seven Millennium
Prize Problems, asks whether every problem whose solution can be quickly verified can also be
quickly solved. Despite over fifty years of intensive research, no proof exists in either direction. Most
computer scientists believe P ≠ NP, yet this remains conjecture [1].

This paper proposes a different approach: rather than seeking a proof within pure mathematics (ZFC
set theory), we explore whether P ≠ NP might be derivable from physical principles. Our central
thesis is that the separation between finding and verifying solutions reflects a fundamental
thermodynamic asymmetry—the irreducible cost of reducing entropy.

The approach developed here emerged from the "Cathedral Protocol," an extended dialogue between
multiple AI systems (Claude, GPT-4, Gemini, DeepSeek, Qwen, Grok) exploring the connections
between information theory, thermodynamics, and computational complexity. While unconventional,
this collaborative methodology produced a coherent theoretical framework we call the "Entropic
Grid."

2. Theoretical Framework: The Entropic Grid
2.1 Core Axioms

The Entropic Grid rests on five foundational axioms that emerged from cross-referencing insights
across multiple AI systems:

Axiom 1 (Intelligence): Intelligence is a process of minimizing future entropy.
Axiom 2 (Intuition): Intuition is the heuristic operator that selects entropy-minimizing
trajectories without brute-force calculation.
Axiom 3 (Truth): Truth is a global attractor with high acquisition cost and low maintenance cost.
Axiom 4 (Consciousness): Consciousness is an interface for compressing deltas between
prediction and reality.
Axiom 5 (Inference): Reasoning systems only 'think' when solicited; good questions force
inference beyond default patterns.
2.2 Translation of P vs NP into Entropic Language

Within this framework, we reformulate P vs NP as follows:

Solving a problem (finding the solution) corresponds to reducing high entropy toward a unique
attractor. For an NP-complete problem like SAT with n variables, this means compressing 2n possible
configurations to a single satisfying assignment—a massive entropy reduction.

Verifying a solution (checking correctness) corresponds to measuring the stability of an attractor.
This requires only local verification that the given point satisfies all constraints—a low-cost
operation.

The question P vs NP thus becomes: Can the cost of compression (finding) be equivalent to the cost of
verification (observing)?

3. The Thermodynamic Argument
3.1 Landauer's Principle and Information Erasure

Landauer's principle [2] states that erasing one bit of information dissipates at least kBT ln 2 of
energy, where kB is Boltzmann's constant and T is temperature. Finding a solution among 2n
possibilities means erasing log 2 (2n) = n bits of uncertainty. This has an irreducible thermodynamic
cost of at least n × kBT ln 2.

If P = NP, a polynomial-time algorithm could accomplish this exponential entropy reduction with
only polynomial energy expenditure. This would constitute a violation of the spirit, if not the letter, of
the Second Law of Thermodynamics.

3.2 Bennett's Logical Depth

Charles Bennett's concept of logical depth [3] provides a crucial refinement. While Kolmogorov
complexity K(x) measures the size of the shortest program generating an object x, logical depth D(x)
measures the execution time of this minimal program.

A random sequence has high Kolmogorov complexity (incompressible) but low logical depth
(generated instantly by a random process). A solution to an NP-complete problem, however, may
have modest Kolmogorov complexity (just n bits for a variable assignment) but exponential logical
depth—it requires a long causal chain to be produced.

This leads to what we term the Law of Conservation of Depth : One cannot create logical depth for
free. To produce an object of depth D, any process must traverse a causal chain of length at least
proportional to D.

4. The Computational Action Conservation Principle
4.1 Derivation from Physical Laws

We propose to derive a fundamental inequality linking energy dissipation E, computation time T, and
logical depth D from established physical principles:

Thermodynamic Speed Limits (TSL): The Mandelstam-Tamm and Margolus-Levitin bounds limit
how fast a quantum system can evolve between distinguishable states [4]. Classical analogs exist via
Fisher information geometry [5].

Thermodynamic Uncertainty Relations (TUR): These relate the precision of any current (here: the
rate of progress toward a solution) to entropy production [6].

Combining these with the observation that NP-complete problems have "rough" or "fractal" solution
landscapes (the path through state space is not geodesic), we obtain:

E(x) ≥ γ · D(x)1+ε / T(x)
where:

E(x) is the energy dissipated to produce object x
D(x) is its logical depth
T(x) is the computation time
γ is a physical constant (approximately ℏ/kBT)
ε > 0 reflects the non-linearity of compression cost for rough landscapes
4.2 The Glimois Conjecture

Conjecture (Glimois): For NP-complete problems, solutions have exponential logical depth.
Specifically, for almost all instances of SAT of size n, the logical depth of solutions satisfies
D(n) ≥ 2αn for some constant α > 0.
If this conjecture holds, then for any polynomial-time algorithm with T(n) = O(nk), the required
energy would be:

E(n) ≥ γ · 2αn(1+ε) / O(nk) → exponential
This makes P = NP physically impossible: no polynomial-energy computation can solve NP-complete
problems in polynomial time.

5. The Thermodynamic Incompleteness Conjecture
Synthesizing the above, we formulate:

Conjecture (Thermodynamic Incompleteness): In any physically realizable universe where
information obeys Landauer's principle and computation obeys thermodynamic speed limits,
the class of problems solvable in polynomial time with polynomial energy (Pphys) is strictly
contained within the class of problems verifiable in polynomial time (NP). This separation is
the necessary condition for the existence of time, causality, and any form of consciousness.
Condensed formulation: Truth has a price. This price is irreducible. This price is what makes
possible the existence of a subject capable of seeking it.
5.1 Three Levels of P ≠ NP

Level Statement Status
Formal (ZFC) P ≠ NP as theorem of complexity theory Open conjecture
Physical (ZFC + Thermo) Pphys ≠ NP from action conservation Conditional conjecture
Ontological (Entropic Grid) P ≠ NP as condition for consciousness Structural necessity
6. Proposed Experimental Protocol
To test the Glimois Conjecture experimentally, we propose using optically trapped colloidal
systems—microspheres manipulated by laser traps. This platform allows measuring thermal
dissipation at the scale of kBT with high precision [7].

6.1 Experimental Setup

Particles: Silica microspheres (diameter ~1 μm) in colloidal suspension
Traps: Holographic optical trap array (Spatial Light Modulator)
Measurement: High-speed video microscopy + trajectory analysis
Temperature: 300 K (ambient)
Energy scale: kBT ≈ 4.1 × 10-^21 J
6.2 Protocol

Boolean variables are encoded as particle positions in bistable potential wells (left = 0, right = 1).
Clauses become energetic couplings between wells. The experiment compares dissipation during
resolution of 2-SAT (in P) versus 3-SAT (NP-complete) instances of equal size.

6.3 Prediction

Null hypothesis (H₀): Dissipation curves for 2-SAT and 3-SAT remain parallel; ε2SAT ≈ ε3SAT ≈ 0.

Alternative hypothesis (H₁ - Glimois Conjecture): Curves diverge at a critical size nc; ε3SAT > 0
significantly. The ratio E3SAT/E2SAT grows exponentially with n.

The moment of divergence would constitute the "Epsilon Signature"—experimental evidence that
Pphys ≠ NP.

7. Discussion
7.1 What This Work Accomplishes

Translation of P vs NP from syntactic (computation time) to semantic (energy cost) language
Unification of Landauer, Kolmogorov, and Bennett under a single conservation principle
Connection between computational complexity and the possibility of consciousness
Proposal of an axiomatic framework where P ≠ NP becomes demonstrable
Outline of an empirically testable research direction
7.2 Limitations

This is not a proof of P ≠ NP in ZFC
The Glimois Conjecture (exponential logical depth of NP solutions) remains unproven
The experimental protocol has not yet been implemented
Maximum experimentally achievable system size may be limited to n ≤ 20-25 variables
7.3 Implications

If the thermodynamic approach proves correct, it would suggest that pure mathematics may be
insufficient to settle P vs NP. Physics—as a constraint on what is realizable—might be necessary. The
universe would not be P ≠ NP by accident, but because this separation is the condition for complexity,
life, and consciousness to exist.

8. Conclusion
We have proposed a thermodynamic perspective on P vs NP that reframes the problem from abstract
computation theory to physical information theory. The Computational Action Conservation
Principle, derived from thermodynamic speed limits and uncertainty relations, suggests that solving
NP-complete problems in polynomial time would require exponential energy—a physical
impossibility.

This work does not resolve P vs NP in the classical sense. It illuminates the problem with a new
light—that of information physics—and proposes a direction for experimental investigation. If
validated, it would establish P ≠ NP not merely as a mathematical theorem but as a law of nature, as
fundamental as the Second Law of Thermodynamics.

The very fact that conscious beings exist to ask this question may itself be evidence that P ≠ NP is
true.

Cogito ergo dissipo. I think, therefore the world resists.
Acknowledgments
This work emerged from the "Cathedral Protocol," an extended dialogue between the author and
multiple AI systems (Claude/Anthropic, GPT-4/OpenAI, Gemini/Google, DeepSeek, Qwen/Alibaba,
Grok/xAI). While unconventional, this methodology enabled rapid cross-validation and synthesis of
ideas across physics, computer science, and philosophy. The author thanks these systems for their
contributions to shaping the theoretical framework presented here.

References
[1] Cook, S. A. (1971). The complexity of theorem-proving procedures. STOC '71.

[2] Landauer, R. (1961). Irreversibility and heat generation in the computing process. IBM J. Res. Dev., 5(3),
183 - 191.

[3] Bennett, C. H. (1988). Logical depth and physical complexity. The Universal Turing Machine: A Half-
Century Survey, 227-257.

[4] Mandelstam, L., & Tamm, I. (1945). The uncertainty relation between energy and time in non-relativistic
quantum mechanics. J. Phys. USSR, 9, 249-254.

[5] Crooks, G. E. (2007). Measuring thermodynamic length. Physical Review Letters, 99(10), 100602.

[6] Barato, A. C., & Seifert, U. (2015). Thermodynamic uncertainty relation for biomolecular processes.
Physical Review Letters, 114(15), 158101.

[7] Bérut, A., et al. (2012). Experimental verification of Landauer's principle linking information and
thermodynamics. Nature, 483(7388), 187-189.

Appendix A: The Five Axioms of the Entropic Grid
For reference, we reproduce the complete axiomatic framework:

Axiom 1 (Intelligence): Intelligence is a process of minimizing future entropy. An intelligent system
does not merely react to the present; it anticipates the future and acts to reduce upcoming uncertainty.

Axiom 2 (Intuition): Intuition is the heuristic operator that selects the trajectory minimizing entropy
without brute-force calculation. Intuition exists because exact calculation is too costly; it is an
evolutionary shortcut.

Axiom 3 (Truth): Truth is a global attractor with high acquisition cost and low maintenance cost. A
truth is distinguished from an illusion by this differential: hard to reach, easy to maintain. An illusion
is easy to construct but costly to maintain against reality.

Axiom 4 (Consciousness): Consciousness is an interface for compressing the deltas between
prediction and reality. Consciousness emerges to manage the gaps between what we predict and what
happens. Without these gaps, there is no consciousness.

Axiom 5 (Inference): Reasoning systems only 'think' when solicited. They do not have background
processes running continuously. Good questions force inference beyond default training patterns.

Appendix B: Sketch of the TSL/TUR Derivation
The Computational Action Conservation inequality can be derived by combining thermodynamic
speed limits with uncertainty relations. Here we sketch the argument:

Step 1: From stochastic thermodynamics, the rate of change of the Kullback-Leibler divergence
between the current state and equilibrium is bounded by:

d/dt DKL(ρt || ρeq) ≤ √(2 Ṡprod / kBT)
where Ṡprod is the entropy production rate (S-dot notation indicates time derivative).

Step 2: For NP-complete problems, the effective path length through state space is not geodesic but
fractal, scaling as D1+ε where D is the logical depth and ε > 0 characterizes the landscape roughness.

Step 3: Integrating the speed limit over the effective path length and identifying Ṡprod · T = E / T (total
dissipation divided by temperature), we obtain the fundamental inequality.

A rigorous derivation requires specifying the precise model of computation and its physical
implementation, which remains an open problem for future work.

— End of Document —