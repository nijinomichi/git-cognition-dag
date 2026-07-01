# Limits and Falsifiability (draft)

Before discussing what the model explains, we state the conditions under which
it would be wrong. A framing of Git as a distributed system of temporal
cognition is only useful if it can fail; otherwise it is decoration on top of
existing practice. This section fixes those failure conditions first, so that
the discussion and conclusion are constrained by them rather than free to
overclaim.

## What the claim actually asserts

The testable core is narrow: that the formal properties of G = (V, E, P, H)
predict measurable differences in comprehension, recovery, and collaboration
quality. The claim is not that Git is literally a mind, nor that the cognition
framing is the only valid description. It is that structural properties of the
repository graph systematically shape human understanding and collaborative
error tolerance. Everything below is a way that assertion could turn out to be
false.

## Falsification conditions

1. No structural signal. If graph-derived metrics such as branching depth,
   pointer volatility, merge fan-in, and recovery path length show no
   consistent relationship with comprehension, recovery time, or error rates,
   the cognition framing adds nothing over the file-store framing. A null
   result here is a direct refutation, not a missing detail.

2. Framing without predictive gain. If the (V, E, P, H) vocabulary describes
   failures only after they occur but never predicts where they will occur or
   improves how they are handled, the model is a relabeling exercise. It must
   earn its keep by anticipation, not narration.

3. Dominance of external factors. If comprehension and collaboration quality
   are driven mainly by team process, documentation, communication norms, or
   individual skill, and the graph structure is a minor or negligible term,
   then Git-as-cognition is the wrong causal locus even if it is internally
   coherent.

4. Non-generalization across contexts. The model may hold in small,
   exploratory projects but not in large, policy-heavy codebases where pointer
   discipline and merge norms are institutionally enforced, or vice versa. If
   the effect direction reverses or vanishes across project size and
   governance style, the model is at best local, not a general account.

5. Breakdown under multi-agent settings. The extension to human-AI
   co-development is falsified if agents operating under partial knowledge and
   asynchronous updates do not exhibit the predicted structural failure modes,
   or if the graph offers no leverage for coordinating them.

## Scope boundaries (where the model is silent)

The model does not claim to describe the semantic content of code, the
correctness of software, or the psychology of individual developers beyond
their interaction with repository structure. It is silent on non-Git
coordination artifacts such as issue trackers and chat, except where those
change how the graph is read. Treating these silences as failures would be a
category error; treating the falsification conditions above as failures would
not.

## Consequence for the discussion

Because these conditions are stated in advance, the discussion that follows is
allowed to claim only what survives them. Any generalization about human
cognition, collaboration, or human-AI systems must be qualified by which
falsification condition it has not yet cleared. This is what keeps the
conclusion an argument rather than a piece of prose.

