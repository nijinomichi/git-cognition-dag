# Experimental Direction

The hypothesis can be evaluated either as a controlled user study or as a system-level evaluation framework. In both cases, the goal is to test whether the formal properties of G = (V, E, P, H) predict measurable differences in comprehension, recovery, and collaboration quality.

## Controlled user study

A controlled study can compare participants performing Git tasks across repositories that differ in branching depth, merge frequency, and history rewriting intensity. The dependent variables should include error recovery time, task completion time, branch comprehension accuracy, and post-task reconstruction of project history. Useful cognitive load proxies include time-to-explanation for a commit graph, number of navigation commands required before confident action, self-reported mental effort, and the rate of incorrect inferences about HEAD, branch ancestry, or merge provenance. If the hypothesis is correct, increases in branching complexity and rewrite activity should correlate with comprehension degradation and slower recovery after mistakes.

## System-level evaluation

A system-level framework can model repositories as graphs and derive metrics from observable operations. Candidate metrics include average branching depth, merge fan-in, pointer volatility, frequency of non-fast-forward rewrites, conflict recurrence, and median recovery path length after disruptive operations such as reset or failed merge. Collaboration efficiency can be estimated through measures such as time from divergence to integration, number of reconciliation steps per feature branch, and ratio of accepted to abandoned alternative branches. These indicators operationalize the idea that Git is not only storing states but coordinating distributed temporal reasoning.

## CHI / NeurIPS framing

For CHI-style work, the strongest contribution is likely an HCI account of cognitive load, interpretability, and collaborative sensemaking in Git workflows. For a systems- or NeurIPS-adjacent framing, the stronger contribution is a formal and evaluative account of graph-mediated reasoning under uncertainty, potentially extending to multi-agent development settings. In either venue style, the empirical question is the same: whether structural properties of the repository graph systematically shape human understanding and collaborative error tolerance.
