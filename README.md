# Azure Sentinel Analytics Rules for a Small Security Team

## Problem
Default security rules can create too many false alerts. A small security team needs focused detection rules.

## Solution
Azure Activity Logs are collected in Log Analytics and analyzed with KQL.

### Architecture
Azure Subscription
→ Azure Activity Logs
→ Log Analytics Workspace
→ Microsoft Sentinel
→ KQL Detection Queries
→ Analytics Rules
→ Alerts / Incidents
→ Security Team

## Implemented
- Azure for Students subscription
- Resource Group: `rg-sentinel-project`
- Log Analytics Workspace: `law-sentinel-project`
- Microsoft Sentinel enabled
- Azure Activity logs connected
- Log ingestion verified
- `AzureActivity | count` returned 8 records during testing
- KQL detection query tested
- Query saved

## Detection Rules
1. Multiple Failed Azure Operations
2. Suspicious Resource Deletion
3. Repeated Authorization Failures

## False Positive Reduction
Instead of alerting on every failed activity, the queries group events by caller and time window and use a threshold.

## Current Limitation
Analytics rule deployment through the Defender portal could not be completed because the account does not have the required Defender/Sentinel onboarding permissions.

## Screenshots
See the `Screenshots` folder.
