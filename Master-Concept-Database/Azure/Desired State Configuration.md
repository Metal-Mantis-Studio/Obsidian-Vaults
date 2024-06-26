---
Tags: Azure, AZ-400, Azure-Automation
---
A DSC is a configuration management platform nested within [[Azure Automation]]  which allows you to define and maintain the desired state of your [[Azure Resources]] and [[Azure Virtual Machine]] run by [[PowerShell]]. Using your defined desired states the DSC Engine will handle the changes necessary by itself.

Configuration Nodes are the individual resource you are defining a desired state for, this could include VM settings, installed software,  Windows Features and more. It contains a pull mode, in which the DSC checks [[Azure Automation]] for the latest config script and updates if necessary as well as a push mode which is typically manually initiated for a one-time update or an immediate compliance.
