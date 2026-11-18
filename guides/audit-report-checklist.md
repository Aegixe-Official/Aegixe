# Smart Contract Audit Report Checklist

[中文](audit-report-checklist.zh-CN.md)

Use this worksheet to inspect evidence behind an audit claim. It is not an audit methodology or an assessment of any particular project.

## Record the context

| Field | Your evidence |
|---|---|
| Project and report title | |
| Original report URL and revision | |
| Auditor and report date | |
| Repository and reviewed commit | |
| Network and deployed addresses | |
| Check time in UTC | |

## Ten checks

1. **Authenticate the report.** Open the original from the auditor or the project's established security documentation. Cross-check names, dates and revisions. A badge or screenshot is insufficient.
2. **Read the scope.** Identify files, dependencies, commit and exclusions. A token review does not automatically cover the bridge, frontend, backend or operational wallets.
3. **Compare deployment and review.** Check the network and full addresses. For EVM contracts, inspect verified source, compiler settings, constructor arguments and linked libraries where relevant. Verification is not an audit.
4. **Read each finding.** Record impact, prerequisites and affected functions. Severity scales differ between reports; counts alone do not establish security.
5. **Check remediation.** Distinguish unresolved, acknowledged, accepted and fixed according to the report's definitions. Find remediation commits and retest evidence, then check the deployed version includes the change.
6. **Map privileges.** Identify minting, pausing, freezing, parameter changes, withdrawals and upgrade rights where applicable. Check whether the controller is a single key, multisig or timelock, and whether its configuration is independently visible.
7. **Check external assumptions.** Review dependencies on oracles, bridges, liquidity, external contracts, off-chain services and administrators. Record assumptions that cannot be verified.
8. **Understand coverage.** Note which methods were used and where coverage stops. Automated checks, manual review and testing provide different evidence; none proves the absence of vulnerabilities.
9. **Inspect changes after review.** An implementation upgrade, new module or changed privilege configuration may fall outside the original engagement.
10. **Write a bounded conclusion.** Describe the version and evidence checked, open findings and missing information. Do not turn 'audited' into an unrestricted safety claim.

## Finding worksheet

| Finding | Impact and prerequisites | Report status | Fix / retest evidence | Included in deployment? |
|---|---|---|---|---|
| | | | | |

## References and AEGIXE resources

- [Solidity: Security Considerations](https://docs.soliditylang.org/en/latest/security-considerations.html)
- [OpenZeppelin Contracts: Access Control](https://docs.openzeppelin.com/contracts/5.x/access-control)
- [AEGIXE audit report lookup](https://aegixe.com/ai_edit_query_new/)
- [AEGIXE services](https://aegixe.com/)



Updated 12 November 2026. See [sources and review status](../SOURCES.md) for scope.
