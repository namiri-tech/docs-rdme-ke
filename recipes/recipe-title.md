---
title: Recipe Title
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
  "callback_url": "https://example.com/callback", // optional
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

# Create an Item

<!-- json@ -->

