---
tags: Security, Azure
---

Personal Access Tokens (PAT) are an alternative to username/passwords, upon creation PATs have specific permissions and scope, e.g. Create PRs, submit commits, make issues. Each PAT has an expiration date and can be revoked at any time. They are frequently used for [[Continuous Integration & Continuous Deployment (CI-CD)]] such as within build agents to access source code repositories, or by tools.

PATs can provide access to both [[Azure DevOps]] and [[Team Foundation Server (TFS)]] without the need for credentials