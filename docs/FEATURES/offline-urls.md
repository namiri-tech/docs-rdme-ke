---
title: Offline URLs
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

To promptly update a customer to a business about a sale progress sync to KRA, DigiTax has a new Promise URL feature. Meaning that when integrating, you can formulate a QR code immediately to mitigate the following scenarios where:

* your system is running offline
* your system has intermittent connection to DigiTax API
* there's extended downtime on eTIMS, and we have not resolved the transaction on the DigiTax API side

## Format

The Offline URL is in the format: `https://etims.ke/r`/`<business_id>`/`<trader_invoice_number>`

Example: [https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554)-  `https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554`

### How do I get my `business_id`?

The `business_id` is the alphanumeric value in the path when logged into the dashboard and viewing your business account.

Example:

If your URL is `https://digitax.tech/dashboard/orgs/clqt3am8r000/apps/clqthjtvg0001l7`, `clqthjtvg0001l7` (which is after the "*.../apps/*") would be the **business\_id**.

<Image align="center" src="https://files.readme.io/2ecd4929c39f4c62d61b09fef735aac0a816b0858a904e786b89378bbc862a04-A1.png" />

### What is the `trader_invoice_number`?

The `trader_invoice_number` is the alphanumeric identifier you generate or pick from your system to tie an invoice in your records (or system records) with an invoice on DigiTax and consequently on eTIMS.

> A maximum of 50 characters is allowed!

> 🚧 Currently, for offline URL to work the `<trader_invoice_number>` should only have characters that are safe to use in URLs without URL encoding.
>
> These are:
>
> * Alphanumeric characters: A-Z, a-z, 0-9
> * Hyphen: -
> * Underscore: \_
> * Period (dot): .
> * Comma: ,
>
> We'll release an update that allow other characters.

## Completed status

If the transaction is complete, like the one above, you have a link to view the eTIMS verification.\
URL of a complete transaction: \<[https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554)>

See screenshot below.

<Image align="center" src="https://files.readme.io/87e07673d0f2b2426654aec5614f93c8e2545772bc732a1e9137d215304d99e3-A2.png" />

## Other statuses

If the transaction is incomplete, like the one below, you do not get a link to view the eTIMS verification.

* URL of a failed transaction: \<[https://etims.ke/r/clno9s9zb02fqs601u5i79a06/DR24251250](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/DR24251250)>\
  See screenshot below.

  <Image align="center" src="https://files.readme.io/d713084d262969c8556496da8e33fd854bdb140a6a0678429df14355661437c4-A3.png" />
* URL of a submitted transaction: \<[https://etims.ke/r/clno9s9zb02fqs601u5i79a06/SL24-100-095834436](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/SL24-100-095834436)>\
  See screenshot below.

  <Image align="center" src="https://files.readme.io/fad68e4f4debcb2f04208a6f5d60c2ff3e7e784764d4a45fb7e03506f9ccdd0f-A4.png" />