---
tags: Azure, AZ-400, Directed-Monitoring, Synthetic-Monitoring, YAML, Bicep-Module, Deployment-Gate, ARM-Template
---
### Directed Monitoring
Monitoring using actual user actions

### Synthetic Monitoring
Monitoring using a recreation of user actions

### Analytics
Parse logs from multiple sources
Identify root causes
Visualisation
Alerting and Monitoring

### YAML Templates
In YAML, parameters can be accessed via either
```YAML
${{parameters.yourparam}}
${{parameters['yourparam']}}
```

### ARM Template Deployment
![[ARM-Template Deployment.png]]

### BICEP Modules

### Deployment Gate
A part of [[Continuous Integration & Continuous Deployment (CI-CD)]] which ensures certain conditions are met or specific approvals are obtained before code changes reach production

# Deployment Jobs
https://learn.microsoft.com/en-us/azure/devops/pipelines/process/deployment-jobs?view=azure-devops

Canary Deployment - Rolls out a deployment of the new version to a small number of users, as confidence grows, expand the deployment until everyone has it
Rolling Deployment - Rolls out a deployment of the new version to a few instances at a time, phasing out the older versions. It offers a smooth transition where the risk downtime is minimised. 
Blue/Green Deployment - When both a Blue (Live) and Green (new version) environments are simultaneous live at all times, only one of the two environments will be handling traffic whilst the over is entirely idle. On an update, traffic will be redirected from the Blue to the Green deployment resulting in no downtime whatso ever 
