# Introduction (draft)

Almost everyone who works with Git has, at some point, lost track of where
their own work actually is. A branch points somewhere unexpected, a rebase
rewrites a history that colleagues had already reasoned about, or a reset
leaves a project technically intact but no longer legible to the people
depending on it. These moments are usually filed away as user error. We argue
that they are not accidents at the edges of a file management tool; they are
symptoms of what Git actually is.

The standard framing calls Git a version control system, as if its job were
to store and retrieve file states. That framing quietly fails to explain the
most common and most costly experiences of using it. It does not explain why
two technically valid histories can encode incompatible assumptions, why a
merge can succeed syntactically while destroying shared meaning, or why teams
repeatedly disagree about what happened even when they are all looking at the
same repository. If Git were only a file store, these conflicts would be
rare. They are instead routine, which suggests the file-store framing is
describing the wrong object.

This paper proposes a different object. We treat Git not as version control
but as a distributed system of temporal cognition: a shared, external memory
in which multiple people record, revise, branch, and reconcile their
understanding of a project over time. Under this reading, a repository is not
a filing cabinet but a coordination surface for distributed reasoning under
uncertainty, and its failures are failures of collective memory and shared
interpretation rather than mere mistakes.

The stakes of this reframing are practical, not only conceptual. As software
is increasingly written by distributed teams, and increasingly co-authored by
human and AI agents operating on partial knowledge, the question of how a
shared history stays legible, recoverable, and trustworthy becomes a
first-order problem. A tool that silently converts coordination failures into
"user errors" cannot be improved, because it hides where the breakdown
actually happens. Naming Git as a cognition system is what makes those
breakdowns visible and, therefore, addressable.

To make this claim precise rather than metaphorical, we formalize a
repository as G = (V, E, P, H): commits as durable state nodes (V), parent
edges as ancestry (E), movable pointers such as branches and HEAD (P), and
history operations such as merge, rebase, and reset (H). This separation of
persistent structure from interpretive access lets us state exactly where
memory, revision, and collaboration live inside the system, and exactly where
they break. The remainder of the paper develops this model, uses it to build
a taxonomy of structural, semantic, and cognitive failures, proposes how the
hypothesis can be evaluated empirically, and outlines its extension to
tooling, interfaces, and multi-agent collaboration.

