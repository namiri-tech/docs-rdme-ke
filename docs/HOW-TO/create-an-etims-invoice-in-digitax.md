---
title: Create an eTIMS invoice in DigiTax
deprecated: false
hidden: false
metadata:
  robots: index
---
## eTIMS invoice on DigiTax

If you have joined any DigiTax webinar, then you know how to generate an invoice via the Digitax Dashboard. If you have not already joined, below is a link to a webinar recording in which a DigiTax team member talks about DigiTax and how to use it.

[DigiTax webinar video link](https://www.loom.com/share/a41c78b5cfa042a7963f0ec7ebbf0ab6?sid=0771aef2-3c16-4aab-a395-dbe68dbe468b)

You can fast-forward or rewind at your convenience. Please note the following key timestamp on the video linked above:

* **15:51** - Testing how to generate invoices

### eTIMS invoice sections

Below is a eTIMS invoice with sections highlighted.

<Image align="center" src="https://files.readme.io/6cf9281ea7dc361e56813535c9ff7006148174363c2e69bd2bda004baca480c4-211.png" />

An eTIMS invoice has three key components: (They are highlighted above)

1. A \*\*QR code\*\* redirecting to the a URL on "etims.kra.go.ke" &#x20;
   &#x20;  The QR code above redirects to this URL: \<https\://etims-sbx.kra.go.ke/common/link/etims/receipt/indexEtimsReceiptData?Data=P000000001G02JHEURBU6RQAMEF3Y> &#x20;
   &#x20;  The structure is \`https\://etims-sbx.kra.go.ke/common/link/etims/receipt/indexEtimsReceiptData\` \`?Data=\` \`\{KRAPIN}\` \`\{KRA Branch ID}\` \`\{Signature}\`
   2. The **tax breakdown** of that invoice
      3. **eTIMS metadata** that includes:
         * Date and Time of transaction
           * Invoice number
             * Signature
               * Internal Data
                 <br />

## Creating an eTIMS invoice via DigiTax API

<br />

To create an eTIMS invoice via the API, you need to:

1. Create an item
   2. Add stock to that item (if it is stockable). If note skip to step 3
      3. Make a sale
         4. Get the sale details
            <br />
            > 📘 Why do I have to create an item before generating an invoice?> In eTIMS, every line item in a sale invoice or credit note invoice needs to be registered first
