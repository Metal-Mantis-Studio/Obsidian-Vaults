---
Tags: Azure, AZ-400
---
[[DevOps]]

## Permissions
![[Pasted image 20230801093218.png]]
## Deploying YAML templates
YAML templates can be deployed by either adding a single step to the build pipeline that runs the PowerShell script which copies and then deploys the template, or by Adding multiple build steps where each one performs a staging task. The PowerShell method is the go-to.
## Service Hooks
Service hooks allow you to trigger actions in other tools based on events that occurred within Azure DevOps. An example of this is to automatically add build release information to the associated tickets, the service hook would listen to commits within the [[Azure Repository]] and then send the information to the tickets (Work items).