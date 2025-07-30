---
title: Create an Item
description: Recipe Description
hidden: false
recipe:
  color: '#018FF4'
  icon: 🦉
---
```json JSON
{
  "item_class_code": "99010000",
  "item_type_code": "2",
  "item_name": "DigiTax Product 01",
  "origin_nation_code": "KE",
  "package_unit_code": "NT",
  "quantity_unit_code": "U",
  "tax_type_code": "B",
  "default_unit_price": 1000,
  "stock_quantity": 100,
  "callback_url": "https://example.com/callback",
}
```

```json Response Example
{
  "id": "item_1D-54MPL3-D0C5-F00-B4R-BAZ",
  "item_class_code": "99010000",
  "item_type_code": "2",
  "item_name": "DigiTax Product 01",
  "origin_nation_code": "KE",
  "package_unit_code": "NT",
  "quantity_unit_code": "U",
  "tax_type_code": "B",
  "default_unit_price": 1000,
  "etims_item_code": "KE2NTU01290595",
  "is_stock_item": true,
  "stock_quantity": 100,
  "active": true,
  "status": "PENDING",
}
```

# Specify the Item classification code

<!-- json@2 -->

Review the Item classification code table here: https://ke.docs.digitax.tech/docs/items-item-classification-table#/

# Specify the Item type code

<!-- json@3 -->



# Specify the Item name

<!-- json@4 -->



# Specify the item's country of origin

<!-- json@5 -->



# Specify the item package unit code

<!-- json@6 -->



# Specify the item quantity unit code

<!-- json@7 -->



# Specify the item tax type code

<!-- json@8 -->



# Specify the item's default unit price

<!-- json@9 -->



# Specify the item's stock quantity

<!-- json@10 -->



# Specify the callback URL (optional)

<!-- json@11 -->

