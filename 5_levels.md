## Mostly Automated Proof Repair for Verified Libraries

The cost of maintaining formally specified and verified software is widely considered prohibitively high due to the need to constantly keep code and the proofs of its correctness in sync—the problem known as proof repair. One of the main challenges in automated proof repair for evolving code is to infer invariants for a new version of a once verified program that are strong enough to establish its full functional correctness.

In this work, we present the first proof repair methodology for higher-order imperative functions, whose initial versions were verified in the Coq proof assistant and whose specifications remained unchanged. Our proof repair procedure is based on the combination of dynamic program alignment, enumerative invariant synthesis, and a novel technique for efficiently pruning the space of invariant candidates, dubbed proof-driven testing, enabled by the constructive nature of Coq’s proof certificates.

We have implemented our approach in a mostly-automated proof repair tool called Sisyphus. Given an OCaml function verified in Coq and its unverified new version, Sisyphus produces a Coq proof for the new version, discharging most of the new proof goals automatically and suggesting high-confidence obligations for the programmer to prove for the cases when automation fails. We have evaluated Sisyphus on 10 ubiquitous OCaml functions taken from popular libraries, that manipulate arrays and mutable data structures, considering their verified original and unverified evolved versions. Sisyphus has managed to repair proofs for all those functions, suggesting correct invariants and generating a small number of easy-to-prove residual obligations.

1. Flagship area (conference)
2. Subarea (conference session)
3. Research topic
4. Research problem
5. Potential solution

1. Programming languages
2. Testing & Verification
3. Formally Specified and Verified Software
4. Proof repair
5. Proof-driven testing -- dynamic program alignment, enumerative invariant synthesis, and a novel technique for efficiently pruning the space of invariant candidates

## Cutting the Cake: A Language for Fair Division

The fair division literature in economics considers how to divide resources between multiple agents such that
the allocation is envy-free: each agent receives their favorite piece. Researchers have developed a variety of
fair division protocols for the most standard setting, where the agents want to split a single item, however, the
protocols are highly intricate and the proofs of envy-freeness involve tedious case analysis.
We propose Slice, a domain specific language for fair-division. Programs in our language can be converted
to logical formulas encoding envy-freeness and other target properties. Then, the constraints can be dispatched
to automated solvers. We prove that our constraint generation procedure is sound and complete. We also
report on a prototype implementation of Slice, which we have used to automatically check envy-freeness for
several protocols from the fair division literature

1. Flagship area (conference)
2. Subarea (conference session)
3. Research topic
4. Research problem
5. Potential solution
6. Contribution

1. PL
2. Verification
3. Fair Division
4. Intricate & tedious proofs
5. Domain specific language for fair-division
6. Proof of soundness, proof of completeness, prototype implementation
