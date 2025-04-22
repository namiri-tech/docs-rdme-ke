---
title: Which item class code should I use?
deprecated: false
hidden: false
metadata:
  robots: index
---
## Which item class code should I use?

An item\_class\_code is required when creating an item. eTIMS uses a subset of the open, global, multi-sector standard for efficient, accurate classification of products and services - United Nations Standard Products and Services Code® (UNSPSC®).

You can download the entire list [here](https://www.unspsc.org/) (unspsc.org). To determine which item class code to use, follow the steps below.

### Process

1. Search for the item name [here](https://usa.databasesets.com/unspsc) (usa.databasesets.com/unspsc). If no result is returned, use synonyms or segments of the name (especially if it is a compound word like *eyeglass*)
2. Copy the first four numbers of the item's code from the item you've determined as exactly matching your item, or closest to it by definition.
3. Search for those copied first four numbers at the guide page - [Items: Item Classification Table](doc:items-item-classification-table)\\\
   (If there are more than one entry, pick the closest by definition)

### Example:

**eyeglass frames** are not available on the [Items: Item Classification Table](doc:items-item-classification-table) therefore:

* I searched for it (step #1 above), got "42142903".
* (step #2 above) I copy the first four numbers of the code "4214"
* (step #3 above) In the [Items: Item Classification Table](doc:items-item-classification-table), there are two entries starting with "4214".
  1. "42140000" (Patient care and treatment products and supplies)
  2. "42141600" (Basins and bedpans and urinals and admission kits)

I'll use "42140000" which is more general, instead of "42141600".

Moreover, **eyeglass frames** are close in definition to "Patient care and treatment products and supplies" than "Patient care and treatment products and supplies", right?

### On the dashboard

<Image align="center" src="https://files.readme.io/7db3c1f8446e54ba4c2363b377f9e0a6a8a9ade373a445ef79ec273a21ac0e5c-AA.png" />

### On the API

```json
{
  "item_class_code": 42140000,
  "item_type_code": 2,
  "item_name": "Rayban glasses",
  ..
}
```