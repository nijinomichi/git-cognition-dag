# Abstract (draft)

We model Git as a distributed system of temporal cognition rather than as a
version control tool. We formalize a repository as G = (V, E, P, H), where V
is the set of commits as durable state nodes, E is the set of parent edges
defining ancestry, P is the set of movable pointers such as branches and
HEAD, and H is the set of history operations including merge, rebase, and
reset. In this model, persistent structure is separated from interpretive
access: commits and edges define the underlying directed acyclic graph, while
pointers and history operations determine which paths become salient to a
user at a given moment, so user-facing time is a projected narrative rather
than raw graph order. We argue that memory, revision, and collaboration can
all be expressed without leaving G, which lets Git be analyzed as
cognition-bearing infrastructure. We show the model's explanatory power
through a failure taxonomy that distinguishes structural failures in
(V, E, P), semantic failures arising in H during merge and rebase, and
cognitive failures in which users cannot reliably infer what happened or
which path is current. We propose that the hypothesis is testable both as a
controlled user study, measuring error recovery time and comprehension under
varying branching and rewrite intensity, and as a system-level evaluation
using graph-derived metrics such as pointer volatility and recovery path
length. We outline directions toward operational analysis tools, cognition-
aware interfaces, and multi-agent human-AI settings, positioning Git as a
reproducible substrate for error-tolerant distributed reasoning.

