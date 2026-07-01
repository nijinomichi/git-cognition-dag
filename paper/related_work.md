# Related Work (boundary conditions)

This section does not survey the literature. It defines the boundary of the model `G = (V, E, P, H)` by naming, for each adjacent framework, the one structural feature that framework cannot preserve. The purpose is negative: to fix where existing models stop being able to represent what this model represents. No claim of superiority is made; each framework remains correct within its own scope.

## Distributed systems / version control theory

These frameworks treat G as a data structure to be replicated, merged, and made consistent. They preserve V, E, and P as state to be synchronized. What they cannot preserve is H as a cognition-bearing operation: in their vocabulary a merge is a reconciliation of divergent state, not an act of integrated understanding. The temporal order encoded in E is treated as causality for consistency, not as lived time indexed to an observer. The boundary: correctness of state is expressible; the reading of state as memory is not.

## Cognitive science (external memory / cognitive offloading)

These frameworks can describe Git as an external store into which memory is offloaded, and can model the human retrieval that reads it. They preserve the observer and the read. What they cannot preserve is the internal graph structure `G = (V, E, P, H)` as the memory's own form: the store is treated as opaque content, not as a typed graph whose edges and pointers carry the temporal index. The boundary: the offloading relation is expressible; the structure of the thing offloaded into is not.

## Philosophy of trace / memory theory

These frameworks preserve the trace as that which remains and defers meaning, and take the persistence of the mark seriously. What they cannot preserve is the operational and pointer layer: P (movable reference) and H (executable revision) have no counterpart in a theory of the inert trace. In G, the past is not only left behind as V and E; it is re-entered and re-pointed. The boundary: the persistence of the mark is expressible; the movable, operable present that reads and rewrites it is not.

## Formal verification / probabilistic state systems

These frameworks preserve V and the transition structure as states and transitions over which properties are checked or probabilities assigned. What they cannot preserve is the requirement that the structure be read by an external observer for it to bear cognition: a verified or probabilistically-modeled state system is complete without any reader. In G, an unread structure is a collapsed one. The boundary: the state machine is expressible; the dependence of meaning on external reading is not.

## Summary of the boundary

Each adjacent framework preserves some proper subset of `(V, E, P, H)` plus, at most, the read relation, but none preserves all four components together with the reading observer as a single structure. That intersection is exactly the region this model occupies. The model is defined by what falls outside every neighbor, not by improving on any one of them.
