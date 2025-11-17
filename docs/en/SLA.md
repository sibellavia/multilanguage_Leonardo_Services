# Service Level Agreement (SLA)

This section defines the terms, metrics, and service commitments applicable to the services offered and described.

## Availability Calculation

The Uptime Annual Percentage of the services is determined as follows:

![Annual Uptime Percentage](assets/images/extract/media/SLA.png)  

The Uptime Percentage is calculated as Maximum Available Minutes less Downtime divided by Maximum Available Minutes, where:

- *"Maximum Available Minutes"* is the total accumulated minutes during an Applicable Period that have two or more instances deployed across two or more Availability Zones in the same region. Maximum Available Minutes is measured from when at least two services across two Availability Zones in the same region have both been started resultant from action initiated by Customer to the time Customer has initiated an action that would result in stopping or deleting the service.
- *“Downtime”* is the total accumulated minutes that are part of Maximum Available Minutes that have no service connectivity in the region.

## Service credits
The Customer is entitled to the following credits in the event of failure to meet the following availability levels:

| Uptime Percentage | Service Credit |
| ----------------- | -------------- |
| < 99.90%          | 5%             |
| < 99%             | 10%            |
| < 90%             | 15%            |

