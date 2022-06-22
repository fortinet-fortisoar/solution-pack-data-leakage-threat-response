| [Home](https://github.com/fortinet-fortisoar/solution-pack-data-leakage-threat-response/blob/develop/README.md) | 
|--------------------------------------------|

# Contents

## Connectors

| Connector                  | Description                                                                                                                                                       |
|:---------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft Active Directory | Helps directly query AD to retrieve information about users, groups, and computers, in an organization, by using the Lightweight Directory Access Protocol (LDAP) |
| Symantec CloudSOC          | The Symantec CloudSOC platform enables companies to confidently leverage cloud applications and services while staying safe, secure, and compliant                |
| Symantec DLP               | Symantec DLP provide actions like get incident attachments, get incident details, get incident status, update incident etc.                                       |

>**Warning:** After deployment, this Solution Pack installs or upgrades the stated connectors list.

## Module Schemas

| Module Schema      | Description                                                                           |
|:-------------------|:--------------------------------------------------------------------------------------|
| Employee Watchlist | Manages an employee watchlist through their names and statuses                        |
| Sensitive Files    | Keeps track of sensitive files through the file's location, name, owner, and the type |

## Role

- Full App Permissions

## Playbook Collection

|02 - Use Case - Data Leakage Threat Response|
|:-------------------------------------------|

| Playbook Name                                           | Description                                                     |
|:--------------------------------------------------------|:----------------------------------------------------------------|
| Generate > DLP Alert                                    | Generates a DLP Demo Alert                                      |
| Generate - Symantec CloudSOC External Filesharing Alert | Create a single alert for  Symantec incidents                   |
| Investigate Data Leakage Alert (Symantec CloudSOC)      | Investigate data leakage alert  ingested from Symantec CloudSOC |

>**Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
