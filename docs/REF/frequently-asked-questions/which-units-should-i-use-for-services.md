---
title: Which packaging unit and quantity unit should I use for services?
deprecated: false
hidden: false
metadata:
  robots: index
---
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