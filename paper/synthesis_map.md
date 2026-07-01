# Paper Synthesis Map (Phase 3, draft)

Purpose: connect the fragment drafts into a single argument spine. This is an integration blueprint, not new content generation. It rearranges and links what exists in `paper/` and records which arrows are now closed.

Status: the entrance and exit sections that were missing in Phase 2.5 have since been drafted. The spine is now largely continuous; two sections remain genuinely open. This file stays a live map, not a finished index.

## 0. Shared core (the spine across all drafts)

All sections use the formal model `G = (V, E, P, H)`:

- V = commits (durable state nodes)
- E = parent edges (ancestry)
- P = movable pointers (branches, HEAD)
- H = history operations (merge, rebase, reset)

Central claim: memory, revision, and collaboration can all be expressed without leaving G, so Git can be analyzed as cognition-bearing infrastructure rather than only a file management tool.

Three diagrams recur as the model's evidence layer and bind the sections: `commit_dag_01.txt`, `merge_conflict_graph.txt`, `cognitive_branching_model.txt`.

The (V, E, P, H) vocabulary is the glue of the synthesis. Each section is a mapping onto this vocabulary. A section that cannot be stated in this vocabulary does not belong in the spine.

## 1. Synthesis map (fragment -> paper structure)

| Standard section | Live fragment | Role in synthesis | Status |
| --- | --- | --- | --- |
| Abstract | abstract.md | Compress (V,E,P,H) + claim + eval into ~5 sentences | Draft exists |
| 1. Introduction | introduction.md | Problem statement: Git = memory architecture | Draft exists |
| 2. Related Work | (none) | HCI / VCS cognition / distributed cognition | Open |
| 3. Formal Model | formal_model.md | Spine. Basis of the Method | Draft exists |
| 4. Failure Taxonomy | failure_taxonomy.md | Model's explanatory power (Structural/Semantic/Cognitive) | Draft exists |
| 5. Experiments / Eval | experimental_direction.md | User study + system-level + venue framing | Draft exists (no results) |
| 6. Discussion | discussion.md | Theoretical failure: 4 collapse types | Draft exists |
| 6b. Core Failure Condition | core_failure_condition.md | Isolates the core beneath the taxonomy: isomorphism loss + read-nothing optimum | Draft exists |
| 7. Limits / Falsifiability | limits_and_falsifiability.md | Empirical falsification conditions | Draft exists |
| 8. Future Work | future_work.md | Tooling / interface / multi-agent | Draft exists |
| 9. Conclusion | (none) | Restate the claim without closing the system | Open |
## 2. Narrative spine (arrows, now mostly closed)

The causal arrows between fragments are the connective tissue. Their current state:

```
Formal Model (V,E,P,H)
   | "what breaks in this vocabulary"      [CLOSED via failure_taxonomy]
   v
Failure Taxonomy -- Structural (V,E,P) / Semantic (H) / Cognitive (interpretation)
   | "beneath the taxonomy, what is the core failure"  [CLOSED via core_failure_condition]
   v
Core Failure Condition -- isomorphism loss + read-nothing optimum
   | "can the breakage be measured / falsified"  [CLOSED via limits_and_falsifiability + experimental_direction]
   v
Experimental Direction / Limits -- user study / system metrics / falsification conditions
   | "if measurable, what to improve"     [CLOSED via future_work]
   v
Future Work -- tooling / interface / multi-agent
```

Discussion (discussion.md) runs alongside as the theoretical-failure layer: four collapse types (Representational, Coordination, Temporal, External). Its one-line kernel: history stops being read = time dies.

## 3. What is now closed vs. still open

Closed (entrance + interior + one exit direction):

- Abstract, Introduction: entrance written.
- Formal Model -> Failure Taxonomy -> Core Failure Condition: interior chain continuous.
- Limits/Falsifiability (empirical) and Discussion (theoretical, 4 types): the failure side is now closed on both empirical and theoretical fronts. The theory specifies both when it holds and when it collapses.
- Future Work: forward exit written.

Still open (deliberately, not by neglect):

- Related Work: can be last; positions the claim against HCI / VCS cognition / distributed cognition.
- Conclusion: must restate the claim without sealing the system. The repo stays coherently unfinished; the conclusion should leave room for external observers rather than declare closure.

## 4. Generation order for remaining sections

1. Related Work (situates the argument for outside readers)
2. Conclusion (restate claim; preserve unfinishedness and space for external reading)

Everything else is drafted. The map's job now is to keep the two open sections visible as open, and to prevent the drafted sections from being over-optimized into a "finished" artifact. Coherence over finish.
