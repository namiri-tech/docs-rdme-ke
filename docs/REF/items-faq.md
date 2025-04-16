---
title: Items FAQ
deprecated: false
hidden: false
metadata:
  robots: index
---
## Which item class code should I use?

### Process

1. Search for the item here: \<https\://www\.unspsc.org/>
2. Search for the first four numbers here: \<https\://docs.digitax.tech/docs/items-classification> (If there are more than one entry, go to the nearest one by definition)
3. EXTRA: If you'd like to know more about the code, search for it here: \<https\://usa.databasesets.com/unspsc>

### Example:

**eyeglass frames** are not available on the [DigiTax's eTIMS item classification code list](https://docs.digitax.tech/docs/items-classification)  therefore:

* I searched for it (step #1 above), got "42142903".
* (step #2 above) In the [DigiTax's eTIMS item classification code list](https://docs.digitax.tech/docs/items-classification), there are two entries starting with "4214".
  1. "42140000" (Patient care and treatment products and supplies)
  2. "42141600" (Patient care and treatment products and supplies)

I'll use "42140000" which is more general, instead of "42141600".

Moreover, **eyeglass frames** are close in definition to "Patient care and treatment products and supplies" than "Patient care and treatment products and supplies", right?

### On the dashboard

<Image align="center" src="https://files.readme.io/7db3c1f8446e54ba4c2363b377f9e0a6a8a9ade373a445ef79ec273a21ac0e5c-AA.png" />

### On the API

```json
{
  "item_class_code": 42141600,
  "item_type_code": 2,
  "item_name": "Rayban glasses",
  ..
}
```

## Which packaging unit and quantity unit should I use for services?

For physical items, the packaging unit and quantity unit are self-explanatory.

For services, we advise that you use: "NET" for packaging unit and "pieces/ item" for quantity unit.

### On the Dashboard

<Image align="center" src="https://files.readme.io/ea9af4bf61b5a94f8d5415fba6c6b8276257c3a72d7f74062fdc9cf593c5383f-AAB.png" />

### On the API

```json
{
  ...
  "package_unit_code": NT,
  "quantity_unit_code": U,
  ...
}
```