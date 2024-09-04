# EntraPIMWorkbook
This Azure Mnitor workbook focus on Microsoft Entra Privilige Identity Management and provides visibility of Resource Audit History.

## Introduction
Microsoft Entra Privilege Identity Management have audit history log in 30 days by default. To retain longer than 30 days, it must be stored audit log outside of Microsoft Entra, such as in the Log Analaytics Workspace.

However, Microsoft Entra audit logs sent externally can be in a very difficult-to-understand format.

This workbook might help the audit log visibility for IT operator.


## Prerequisites
- This workbook needs Microsoft Entra diagnostics settings that Audit log would be sent to the Log Analytics Workspaces.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/TODO)

## Disclaimer
The column specifications for exported Audit Logs are not disclosed, and the KQL query is based on the information output by the writer's operation in test enviroment, so it is not guaranteed to work correctly in all environments. Please understand in advance.

## Feedback
Please let me know if any probrems or mistakes of this workbook with Issue or Pull Request.