# Paper Synthesis Map (Phase 4, closed)

Purpose: connect the fragment drafts into a single argument spine. This is an integration blueprint, not new content generation. It rearranges and links what exists in `paper/` and records which arrows are now closed.

Status: all standard sections are now drafted, including the closure layer (related_work.md, conclusion.md). The spine is complete and the system is closed. This file is now an index of a reviewable artifact, not a generation plan.

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
| 2. Related Work | related_work.md | Boundary conditions: 4 domains, structural incompatibility only | Draft exists |
| 3. Formal Model | formal_model.md | Spine. Basis of the Method | Draft exists |
| 4. Failure Taxonomy | failure_taxonomy.md | Model's explanatory power (Structural/Semantic/Cognitive) | Draft exists |
| 5. Experiments / Eval | experimental_direction.md | User study + system-level + venue framing | Draft exists (no results) |
| 6. Discussion | discussion.md | Theoretical failure: 4 collapse types | Draft exists |
| 6b. Core Failure Condition | core_failure_condition.md | Isolates the core beneath the taxonomy: isomorphism loss + read-nothing optimum | Draft exists |
| 7. Limits / Falsifiability | limits_and_falsifiability.md | Empirical falsification conditions | Draft exists |
| 8. Future Work | future_work.md | Tooling / interface / multi-agent | Draft exists |
| 9. Conclusion | conclusion.md | Minimal closure: definition + novelty + limitation + collapse | Draft exists |

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

## 3. Closure status (all sections drafted)

Entrance: abstract.md, introduction.md.
Interior: formal_model.md -> failure_taxonomy.md -> core_failure_condition.md (continuous).
Failure side: limits_and_falsifiability.md (empirical) + discussion.md (theoretical, 4 types). The theory states both when it holds and when it collapses.
Forward exit: future_work.md.
Boundary: related_work.md (structural incompatibility with 4 adjacent domains; boundary definition only).
Closure: conclusion.md (minimal layer: definition + novelty + limitation + collapse).

All standard sections now have a live fragment. No section is open.

## 4. State

The paper is a closed, reviewable artifact: every arrow in the spine has a written fragment, and the closure layer (related_work + conclusion) is in place. The conclusion is minimal and does not re-open the system. This map is now an index of a complete structure rather than a generation plan.
