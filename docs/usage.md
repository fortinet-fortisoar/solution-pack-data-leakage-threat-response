| [Home](https://github.com/fortinet-fortisoar/solution-pack-data-leakage-threat-response/blob/develop/README.md) | 
|--------------------------------------------|

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to simulate and reset scenarios. 
 
To understand the process FortiSOAR follows to respond to data leakage threat, we have included a scenario &mdash; **Data Leakage** with this solution pack. Refer to the section **Data Leakage Scenario** to understand how this solution pack's automation addresses your needs. 

## Data Leakage Scenario

This scenario generates two example alerts of Type *Data Leakage* in FortiSOAR's **Alerts** module. 

Navigate to the demo alert and note the following: 

- Following reported information is present for analyzing the case
    - Policy violation
    - Description and action
    - Violators username
    - File hash
    - Recommendations from CloudSOC

Users can launch the **Investigate Data Leakage Alert (Symantec CloudSOC)** playbook to perform following automated tasks:

- Identify employee watchlist status of user who is involved in data leak
- Identify if the file involved is a sensitive document
- Initiate containment actions for sensitive documents
- Block the user in Microsoft Active Directory and, using Symantec DLP, investigate if the user is involved in any other data leak event