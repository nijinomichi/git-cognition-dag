# Paper Synthesis Map (Phase 2.5, draft)

Purpose: connect the existing fragment drafts into a single argument spine.
This is an integration blueprint, not new content generation. It rearranges
and links what already exists in `paper/`.

Status of repository at time of writing: four draft sections exist
(`formal_model.md`, `failure_taxonomy.md`, `experimental_direction.md`,
`future_work.md`), but no synthesis layer connects them.

## 0. Shared core (the spine across all drafts)

All four drafts consistently use the formal model `G = (V, E, P, H)`:

- V = commits (durable state nodes)
- E = parent edges (ancestry)
- P = movable pointers (branches, HEAD)
- H = history operations (merge, rebase, reset)

Central claim: memory, revision, and collaboration can all be expressed
without leaving G, so Git can be analyzed as cognition-bearing
infrastructure rather than only a file management tool.

Three diagrams recur as the model's evidence layer and bind the sections:
`commit_dag_01.txt`, `merge_conflict_graph.txt`, `cognitive_branching_model.txt`.

The (V, E, P, H) vocabulary is the glue of the synthesis. Each section is
placed as a mapping onto this vocabulary.

## 1. Synthesis map (fragment -> paper structure)

| Standard section | Live fragment | Role in synthesis | Status |
| --- | --- | --- | --- |
| Abstract | (none) | Compress (V,E,P,H) + claim + eval into ~5 sentences | To generate |
| 1. Introduction | README core hypothesis | Problem statement: Git = memory architecture | To generate (README material exists) |
| 2. Related Work | (none) | HCI / VCS cognition / distributed cognition | To generate |
| 3. Formal Model | formal_model.md | Spine. Basis of the Method | Draft exists |
| 4. Failure Taxonomy | failure_taxonomy.md | Demonstrates model's explanatory power (Structural/Semantic/Cognitive) | Draft exists |
| 5. Experiments / Eval | experimental_direction.md | User study + system-level + venue framing | Draft exists (no results) |
| 6. Discussion | scattered in section endings | Connect taxonomy <-> eval | To integrate |
| 7. Future Work | future_work.md | Tooling / interface / multi-agent | Draft exists |
| 8. Conclusion | (none) | Restate the claim | To generate |

## 2. Narrative spine (the missing connective tissue)

The fragments exist, but the causal arrows between them are not yet written:

```
Formal Model (V,E,P,H)
   |  "what breaks in this vocabulary"
   v
Failure Taxonomy -- Structural (V,E,P) / Semantic (H) / Cognitive (interpretation)
   |  "can the breakage be measured"
   v
Experimental Direction -- user study / system metrics
   |  "if measurable, what to improve"
   v
Future Work -- tooling / interface / multi-agent
```

The synthesis work is to write an explicit transition (1-2 sentences) for
each arrow, turning each arrow into a bridging paragraph.

## 3. Verified strong connections (assets already aligned)

- formal_model's three diagrams <-> failure_taxonomy references the same
  diagrams (commit_dag_01 -> structural, merge_conflict_graph -> semantic):
  model and failure theory are already mapped.
- failure_taxonomy's Cognitive failure <-> experimental_direction's
  cognitive load proxies / incorrect inferences about HEAD: failure and
  measurement indicators already correspond.
- experimental_direction's multi-agent hint <-> future_work's multi-agent
  evaluation: eval and future work are continuous.

Consequence: the first three arrows already have material. What is missing
is the entrance (Abstract / Introduction / Related Work) and the exit
(Discussion / Conclusion).

## 4. Phase 2.5 output and generation order

This file is the single integration blueprint. It preserves the fragments,
keeps generation controlled, and binds everything with the (V,E,P,H) spine.

Generation order for the missing sections:

1. Introduction (README material exists)
2. Abstract
3. Discussion / Conclusion
4. Related Work (can be last)

This is the correct precondition for Phase 3 (full generation + licensing).

