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

<Table align={["left","left","left"]}>
  <thead>
    <tr>
      <th>
        Status
      </th>

      <th>
        Meaning
      </th>

      <th>
        Action
      </th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>
        queued
      </td>

      <td>
        DigiTax Queueing system is **queued** after trying to reach eTIMS
      </td>

      <td>
        Check in later. If you set up [Callback URLs](doc:call-back-urls), we'll post to your system when the eTIMS sync is done.
      </td>
    </tr>

    <tr>
      <td>
        un\_queued
      </td>

      <td>
        DigiTax Queueing system is **unqueued** after trying to reach eTIMS
      </td>

      <td>
        Check in later. If you set up [Callback URLs](doc:call-back-urls), we'll post to your system when the eTIMS sync is done.
      </td>
    </tr>

    <tr>
      <td>
        in\_progress
      </td>

      <td>
        DigiTax Queueing system is **in progress** after attempting to reach eTIMS
      </td>

      <td>
        Check in later
      </td>
    </tr>

    <tr>
      <td>
        completed
      </td>

      <td>
        eTIMS has received and accepted the transaction, and we have the final data
      </td>

      <td>
        For ITEM: You can now create a sale with this item\\
        For SALE: You have the `etims_url` hence can generate the QR code.
      </td>
    </tr>

    <tr>
      <td>
        failed
      </td>

      <td>
        eTIMS rejected the transaction
      </td>

      <td>
        Please initiate another transaction.
      </td>
    </tr>

    <tr>
      <td>
        paused
      </td>

      <td>
        DigiTax Queueing system is **paused** after trying to reach eTIMS. The queue will be unpaused in the background
      </td>

      <td>
        Check in later. If you set up [Callback URLs](doc:call-back-urls), we'll post to your system when the eTIMS sync is done
      </td>
    </tr>

    <tr>
      <td>
        submitted
      </td>

      <td>
        eTIMS has received and accepted the transaction; however, we do not have the final data from their system. Though this is unlikely, we have a workaround to get the data.
      </td>

      <td>
        If you don't have an `etims_url` kindly initiate a chat with us when this happens.
      </td>
    </tr>
  </tbody>
</Table>