---
title: Offline URLs
deprecated: false
hidden: false
metadata:
  robots: index
---
# Overview for offline URLs

To promptly update a customer or a business about a sale's progress, sync to KRA; DigiTax has a new offline URL feature.

Meaning that when integrating, you can formulate a QR code immediately to mitigate the following scenarios where:

* Your system is running offline
* Your system has an intermittent connection to DigiTax API
* There's extended downtime on eTIMS, and we have not resolved the transaction on the DigiTax API side

## Format

The offline URL is in the format `https://receipt.dg.tax/r`/`<business_id>`/`<trader_invoice_number>`

Example: [https://receipt.dg.tax/r/business_01KK0ZMC0XTYBXXPBS8BN3SDTA/SAL26-065-072410521-DAU2F2](https://receipt.dg.tax/r/business_01KK0ZMC0XTYBXXPBS8BN3SDTA/SAL26-065-072410521-DAU2F2)- `https://receipt.dg.tax/r/business_01KK0ZMC0XTYBXXPBS8BN3SDTA/SAL26-065-072410521-DAU2F2`

## How do I get my `business_id`?

There are two ways: via the DigiTax Dashboard and via the API.

### via the DigiTax Dashboard

`business_id` is the alphanumeric value in the path when logged into the dashboard and viewing your business account.

Example:

If your current URL (if you are already in a business on the DigiTax dashboard) is `https://digitax.tech/dashboard/orgs/organisation_01KFATS94E7BSAB0GB5SJGG7B4/apps/business_01KK0ZMC0XTYBXXPBS8BN3SDTA` then:  

The business_id would be **`business_01KK0ZMC0XTYBXXPBS8BN3SDTA`** which:

* is after the "_.../apps/_"
* and has a prefix "business_"

<Image align="center" src="https://files.readme.io/563e37eb0dc1527ab0c2f07417959dfab9d6862f5ac3986b939269f9e0d47a64-Screenshot_2026-03-10_at_12.32.062x.png" />

### via the DigiTax API

If you make a GET request to 

### What is the `trader_invoice_number`?

The `trader_invoice_number` is the alphanumeric identifier you generate or pick from your system to tie an invoice in your records (or system records) with an invoice on DigiTax and consequently on eTIMS.

> A maximum of 50 characters is allowed!

> 🚧 Currently, for offline URL to work the `<trader_invoice_number>` should only have characters that are safe to use in URLs without URL encoding.
>
> These are:
>
> * Alphanumeric characters: A-Z, a-z, 0-9
> * Hyphen: -
> * Underscore: _
> * Period (dot): .
> * Comma: ,
>
> We'll release an update that allow other characters.

## Completed status

If the transaction is complete, like the one above, you have a link to view the eTIMS verification.  
URL of a complete transaction: \<[https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/v5241554)>

See screenshot below.

<Image align="center" src="https://files.readme.io/87e07673d0f2b2426654aec5614f93c8e2545772bc732a1e9137d215304d99e3-A2.png" />

## Other statuses

If the transaction is incomplete, like the one below, you do not get a link to view the eTIMS verification.

* URL of a failed transaction: \<[https://etims.ke/r/clno9s9zb02fqs601u5i79a06/DR24251250](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/DR24251250)>  
  See screenshot below.

  <Image align="center" src="https://files.readme.io/d713084d262969c8556496da8e33fd854bdb140a6a0678429df14355661437c4-A3.png" />
* URL of a submitted transaction: \<[https://etims.ke/r/clno9s9zb02fqs601u5i79a06/SL24-100-095834436](https://etims.ke/r/clno9s9zb02fqs601u5i79a06/SL24-100-095834436)>  
  See screenshot below.

  <Image align="center" src="https://files.readme.io/fad68e4f4debcb2f04208a6f5d60c2ff3e7e784764d4a45fb7e03506f9ccdd0f-A4.png" />
