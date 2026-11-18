---
title: DigiTax API Details
deprecated: false
hidden: false
metadata:
  robots: index
---
In every API endpoint, path, query and/or body parameters are passed along with the GET, POST, PUT and DELETE requests.

> Examples:\
> **body parameters** for [**Create item**](ref:post_items),
> **path parameters** for [**Get a specific item**](ref:get_items-item-id) OR
> **both body parameters and path parameters** for [**Update an item**](ref:put_items-item-id)

The responses contain attributes related to the passed-in body parameters and/or path parameters, which unveil the data model used in the application.

## Data attributes

We break down the attributes consistent with each broad categorization of the API endpoints in:

1. Related to Items
   * [Items: General Data Attributes](doc:item-attributes-items)
   * [Items classification](doc:items-item-classification-table)
2. Related to Sales
   * [Sales attributes](doc:invoice-attributes)