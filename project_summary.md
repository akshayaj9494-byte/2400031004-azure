# Project Summary

## 1. Problem Understanding
Our problem is too many false alerts. It is difficult for a small security team to find real threats. We use Sentinel to find suspicious activity.

## 2. Design and Approach
We collect Azure Activity Logs in Log Analytics. Sentinel checks these logs using KQL queries. We use limits to reduce false alerts.

## 3. Implementation and Functionality
We created the Resource Group, Log Analytics Workspace and Microsoft Sentinel. We connected Azure Activity Logs. We tested KQL and received 8 activity records.

## 4. Demonstration and Results
The logs were successfully received. The failed-operation query returned no matches because no suspicious activity reached the selected threshold during testing.

## 5. Individual Contribution
I created the Azure resources, configured Sentinel, connected the logs, and tested KQL queries.
