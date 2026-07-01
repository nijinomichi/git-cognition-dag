# Core Failure Condition (draft)

The discussion section lists four ways the Git-as-cognition account can break.
This section isolates the core beneath them. The decisive point is
counterintuitive: the theory does not fail when Git fails. A corrupt
repository, a lost commit, or a broken tool is an operational problem, not a
theoretical refutation. The theory fails in a stricter and stranger way, and
it does so under exactly two conditions.

## Condition 1: Loss of isomorphism across V, E, P, H

The model assumes that commits (V), parent relations (E), pointers (P), and
history operations (H) share a single temporal structure. The theory holds
only while these four remain isomorphic to one time. It breaks when that
shared structure dissolves, even though every component still exists:

- History persists but meaning is not carried forward: only V survives as
  record, without transferred understanding.
- HEAD moves but its cognitive meaning does not follow: P becomes
  de-semanticized, a position with no interpretive content.
- Merges occur but understanding is not integrated: H becomes mechanical, an
  operation without comprehension.

At this point the structure is intact but the time inside it is dead. V, E, P,
and H are all present, yet they no longer index the same lived temporal order,
so the cognition claim loses its referent. This is failure by structural
survival: nothing is broken, and yet the mapping is gone.

## Condition 2: Convergence on a read-nothing optimum

Git is, in this account, an external memory meant to be read. The second
failure is the collapse of that reading. As optimization proceeds, systems can
converge on a state where no external observer, human or AI, actually reads
history, and an AI consumes it only as an internal representation. The
consequence is precise:

- V, E, P, H all remain.
- But interpretation disappears.
- Git becomes a compression log rather than a meaning structure.

This is the most severe mode because the theory does not become false; it
becomes true and irrelevant. Every formal claim can still hold while the
phenomenon the theory was about, cognition made external and legible, has
quietly ceased to exist. A correct account of a thing that no one inhabits is
no longer a live theory.

## The core, in one line

The theory does not die when Git breaks. It dies when Git stops being read as
time: when V, E, P, H lose their shared temporal structure, or when the act of
reading history disappears.

## Relation to the rest of the paper

The four breakdown modes in the discussion are surface expressions of these
two core conditions, and the empirical falsification conditions test whether
the model earns its keep while those cores still hold. Naming the core
failure this precisely is what prevents the account from surviving as an
unfalsifiable metaphor: it can be correct, and it can still be rendered
meaningless, and it says exactly when.


## Condition 3: Collapse of distributed identity

A further assumption is implicit and, in practice, the most fragile: that
multiple agents are looking at the same Git. The theory treats G as a shared
object. In reality the same repository is read as different objects at once:

- Human A reads Git as a meaning structure.
- Human B reads it as a work log.
- An AI reads it as a probabilistic token sequence.
- A CI/CD system reads it as a bare state transition.

They are not looking at the same G, yet they proceed as if they were. This
shared illusion is the collapse point. When distributed identity fails, there
is no single G for cognition to be about, and the coordination the theory
describes has no common referent even though every agent believes it does.

## Final breakdown: the return to philosophy

All three conditions converge on one terminal state. The theory returns from
theory to philosophy at the moment Git is reduced from a structure that holds
time to a mere store of changes. At that point:

- V, E, P, H are only graph definitions.
- Cognition disappears.
- The theory still holds, and yet explains nothing.

This is the quiet death: not contradiction, but evacuation of meaning while
the formalism stands.

## The collapse, in one line

The theory compresses to a single condition: the moment history stops being
read, Git as time dies.

## Architecture of the account

The paper is closed as a single structure:

```
Entrance   abstract -> introduction
Body       formal_model -> failure_taxonomy -> experimental_direction
Test axis  limits_and_falsifiability
Collapse   discussion + core_failure_condition
Exit       future_work
Synthesis  synthesis_map
```
