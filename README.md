## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

**Data Leakage Threat Response Solution Pack** is designed to provide a set of investigation and utility playbooks to respond to data leakage.

Configure Cloud Access Security Broker(CASB) connector, such as Symantec CloudSOC, to capture events of policy violation like **External File Sharing**. It creates an alert of type **Data Leakage** and triggers a response workflow.

Refer to Simulation Scenario - Data Leakage to experience the use case without CASB configuration.

### Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to Simulate and Reset scenarios.

This Solution Pack ships with the following simulation scenarios.

**Data Leakage**

The scenario generates a demo alert of the type **Data Leakage**.

Navigate to the generated alert and observe the following:

- Reported information (policy violation action/description, violators username) is present for analyzing the case
- Recommendations from CloudSOC

**Investigate Data Leakage Alert (Symantec CloudSOC)**: Launch the **Investigate Data Leakage Alert (Symantec CloudSOC)** playbook and observe various investigation activities such as

- Identify employee watchlist status of user involved in data leakage
- Identify if the file involved is a sensitive document
- Initiate containment actions for sensitive document
- Block the user in Microsoft Active Directory and, using Symantec DLP, investigate if the user is involved in any other DLP(Data Leakage Policy) event

## Prerequisite

Ensure that the below solution packs are deployed:

|**Solution Pack**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules and Action playbooks|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents

1. Connector(s)

    |**Sr.No.**|**Connector**|
    | :- | :- |
    |1|Microsoft Active Directory|
    |2|Symantec CloudSOC|
    |3|Symantec DLP|

    **Warning:** After deployment, this Solution Pack installs or upgrades the stated connectors list.

2. Modules Schema(s)
    - Employee Watchlist
    - Sensitive Files

3. Role(s)
    - Full App Permissions

4. Playbook Collection(s)

    - 02 - Use Case - Data Leakage Threat Response (3):


    |**Playbook Name**|**Description**|
    | :- | :- |
    |Generate > DLP Alert|Generates a DLP Demo Alert|
    |Generate - Symantec CloudSOC External Filesharing Alert|Create a single alert for  Symantec incidents|
    |Investigate Data Leakage Alert (Symantec CloudSOC)|Investigate data leakage alert  ingested from Symantec CloudSOC|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
