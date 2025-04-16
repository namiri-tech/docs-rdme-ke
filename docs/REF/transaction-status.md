---
title: Transaction status
deprecated: false
hidden: false
metadata:
  robots: index
---
## DigiTax Queueing system

DigiTax provides the following:

* Asynchronous functionality that automatically retries eTIMS
* Get notifications on transaction statuses via [Callback URLs](doc:call-back-urls)
* Throttling traffic between the businesses throughput and eTIMS

This functionality is possible due to the DigiTax Queueing system.

> 📘 You don't run the risk of double-entry
>
> Every transaction that interacts with eTIMS is first off entered into the DigiTax Queueing system to **mitigate against possible eTIMS intermittency and downtime** or slow response rate.

## The different transaction statuses and what they mean

Since transactions are first off entered into the DigiTax Queueing system, we give you the following statuses. This is what they mean.

### Transaction statuses