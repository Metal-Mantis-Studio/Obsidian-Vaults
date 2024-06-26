---
tags: Azure
---
Azure Artifacts allows developers and organisations to create, host and share [[Source Control/Packages]] and is a part of [[Azure DevOps]] providing a secure and centralised package management system such as NuGet, npm, Maven and Python [[Source Control/Packages]].
It allows private [[Source Control/Packages]] to be stored securely as well as create and store them for different package types.
Artifacts can be accessed via RBAC for precise role assignments and can store multiple versions of packages for all use cases. 
## Azure Artifacts Credential Provider
Credential Provider automates the acquisition of credentials needed to restore NuGet packages declared in the .NET workflow. It integrates alongside MSBuild, DotNet, NuGet and works on Windows, Linux and Mac. When using packages from an Azure Artifact Feed, credential provider will automatically acquire and store a token on behalf of NuGet.