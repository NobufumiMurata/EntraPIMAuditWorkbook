# Entra PIM Workbook
This Azure Mnitor workbook focus on Microsoft Entra Privilige Identity Management and provides visibility of Resource Audit History.

## Introduction
Microsoft Entra Privilege Identity Management have audit history log in 30 days by default. To retain longer than 30 days, it must be stored audit log outside of Microsoft Entra, such as in the Log Analaytics Workspace.

However, Microsoft Entra audit logs sent externally might be in a very difficult-to-understand format.

This workbook might help the audit log visibility for IT operator.


## Prerequisites
- This workbook needs Microsoft Entra diagnostics settings that Audit log would be sent to the Log Analytics Workspaces.

## Deploy
1. Get the Log Analytics Workspace Resourse ID from JSON view of overview page.
2. Hit the "Deploy to Azure" button.

    [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FNobufumiMurata%2FEntraPIMAuditWorkbook%2Fmain%2FWorkbooks%2FMicrosoftEntraPIMAudit.workbook)

3. Fill the Resouce ID value obtained in 1 in "workbookSourceId" field. and type in "workbookDisplayName" field if you want to change.
4. Deploy to Azure.

## Disclaimer
The column (ex. Additional Fiels column) specifications for exported Audit Logs are not disclosed, and the KQL query is based on the information output by the writer's operation in test enviroment, so it is not guaranteed to work correctly in all environments. Please understand in advance.

## Feedback
Please let me know if any probrems or mistakes of this workbook with Issue or Pull Request. 