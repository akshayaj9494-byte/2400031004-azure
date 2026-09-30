# Azure Sentinel Analytics Rules for a Small Security Team

## Problem
Too many false alerts make it difficult for a small security team to find real threats.

## Solution
We use Microsoft Sentinel, Azure Activity Logs and KQL queries to detect suspicious activity and reduce false alerts.

## Architecture
Azure → Azure Activity Logs → Log Analytics → Microsoft Sentinel → KQL → Alerts

## Azure Resources
- Resource Group: `rg-sentinel-project`
- Log Analytics Workspace: `law-sentinel-project`
- Microsoft Sentinel
- Azure Activity Logs

## KQL Queries
We created detection queries for:
- Multiple Failed Azure Operations
- Suspicious Resource Deletion
- Repeated Authorization Failures

## Results
- Azure Activity logs successfully received
- 8 activity records were found during testing
- KQL queries were tested successfully
- No suspicious activity matching the failure threshold was found during testing

## Project Evidence
Screenshots of the Azure setup and KQL testing are included in this repository.

## Team Project
Azure Sentinel Analytics Rules for a Small Security Team
