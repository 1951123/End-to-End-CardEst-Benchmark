# ESS coordination rules for this upstream-derived fork

This file governs **ESS-directed development in this fork only**; it does not override upstream contributor practices.


## ESS cross-repository coordination (central Issue: ess-research#358)

- **All new ESS-directed Issues are created only at [1951123/ess-research](https://github.com/1951123/ess-research/issues)**. Do not open task Issues in this dependency repository. Historical upstream Issues, external community contributions and GitHub PR discussions are not reclassified as ESS research Issues.
- One central `ess-research#N` may be implemented by **multiple independent repository PRs**. Each dependency PR must include `Research Issue: 1951123/ess-research#N`, and the central Issue should link the participating PRs. Component PR merge does not alone close the central Issue.
- Task branches, Worktrees and runtime task identifiers in all ESS-owned repos use the **central `ess-research` Issue number N**, never the local PR number. Keep one writer per branch/Worktree and respect each repository's source and run ownership.
- `ess-research` owns scientific questions, approvals, the D-009 Train/Downstream protocol, integration, official evaluation and evidence. Component repositories own their code and focused tests; cross-repository writes/expensive official tests are not authorized just by an Issue reference.
- Formal consumers pin **full immutable Git SHAs**, plus relevant build/interface/data identities. Branch names, editable installs and moving upstream heads are not valid scientific provenance.
- Forks of upstream benchmarks are **upstream-derived dependencies**, not independent ESS research centers: prefer adapters in `ess-research`; modify a fork via a linked PR only when required, and identify upstream and fork commits.

This coordination policy supplements, rather than changes, scientific decision D-009 or existing protected-input, resource, review and experiment restrictions.
