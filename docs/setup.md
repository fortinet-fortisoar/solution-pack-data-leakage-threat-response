| [Home](https://github.com/fortinet-fortisoar/solution-pack-data-leakage-threat-response/blob/develop/README.md) | 
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution pack that appears, search for and select **Data Leakage Threat Response Solution Pack**.
3. Click the **Data Leakage Threat Response Solution Pack** solution pack card.
4. Click the **Install** button on the bottom to begin installation.


## Prerequisites

The **Data Leakage Threat Response Solution Pack** solution pack depends on the following solution packs. 

| Solution Pack Name | Purpose                                                     |
|:-------------------|:------------------------------------------------------------|
| SOAR Framework     | Required for Incident Response modules and Action playbooks |
| SOC Simulator      | Required for Scenario Module and SOC Simulator connector    |

# Configuration

For optimal performance of **Data Leakage Threat Response Solution Pack** solution pack, you can install and configure: 
- Cloud Access Security Broker(CASB) connector to capture events of policy violation like External File Sharing
    - To configure Symantec CloudSOC as a CSAB, refer to [Configuring Symantec CloudSOC](https://docs.fortinet.com/document/fortisoar/1.0.0/symantec-cloudsoc/1/symantec-cloudsoc-v1-0-0#Configuration_parameters)
