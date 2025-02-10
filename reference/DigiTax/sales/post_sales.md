---
title: Add sale
excerpt: >
  Add sale and credit notes. The difference between a sale and a credit note is
  the `receipt_type_code` which is a required field. A sale has a receipt type
  code of <b>S</b> while a credit note has a receipt type code of <b>R</b>. When
  adding a credit note, the original invoice number is required. For a Sale:
  `receipt_type_code` is "S" For a Credit note: `receipt_type_code` is "R" and
  `original_invoice_number` is required. Note: `original_invoice_number` is a
  numeric value (This should be an existing eTIMS invoice number of the sale
  invoice you intend to credit) Note: `trader_invoice_number` should be unique,
  unless you deactivated the sale or the sale queue_status is "failed".
api:
  file: openapi.json
  operationId: post_sales
hidden: false
---