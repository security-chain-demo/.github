Software Supply Chain Security – Demo
======================================

This is a Proof-of-Concept showing how to incorporate fixing security vulnerabilities
without any additional software you have to buy. It only uses

- GitHub Actions
- JIRA (we assume, you already use that as an issue tracker)

When doing a deployment, the GitHub Actions pipeline will scan for vulnerabilities
with [Trivy](https://trivy.dev/), and sync the found issues to JIRA.

In JIRA they can be handled within the usual workflow.
In addition, a Grafana dashboard can visualize the data.

For more information, see the repositories

- [deployment](https://github.com/security-chain-demo/deployment/)
- [github-actions](https://github.com/security-chain-demo/github-actions/)
