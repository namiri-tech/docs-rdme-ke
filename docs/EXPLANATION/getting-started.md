---
title: 'Getting Started: DigiTax and KRA eTIMS'
excerpt: >-
  **DigiTax Kenya API (Version 1) Hub** contains guides and API reference pages
  for further understanding, equipping you on how to integrate with the KRA
  eTIMS System
hidden: false
metadata:
  title: DigiTax Kenya API Hub - V1
  robots: index
---
<Cards columns={2}>
  <Card title="Navigation" icon="fa-compass">
    If you're new to the DigiTax Kenya API Hub, learn how to navigate our pages [here](https://ke.docs.digitax.tech/v1.0/docs/how-to-use-this-site).
  </Card>

  <Card title="Support" icon="fa-question">
    If you get stuck, or have questions, [email us](mailto:support@namiri.tech) OR\
    Talk to us via the **DigiTax chat** on the bottom right of any page.
  </Card>

  <Card title="KRA eTIMS integration with DigiTax" icon="fa-bars">
    Explore this page and other detailed guide pages to gain understanding of the KRA eTIMS System and how DigiTax integration works.
  </Card>

  <Card title="DigiTax Kenya API Reference" icon="fa-plug">
    Get the pre-requisites, explore the API endpoints, and learn its feature set via our **interactive API reference** [here](https://ke.docs.digitax.tech/v1.0/reference).
  </Card>
</Cards>

<Accordion title="DigiTax is multi-national. Explore other countries here ..." icon="fa-globe">
  You are currently reading a guide in the DigiTax Kenya API Hub.

  If you're looking for another country or the general homepage for DigiTax API, navigate to the [DigiTax API homepage](https://docs.digitax.tech), or country-specific API hub pages (ordered alphabetically):

  * <i class="icon-guides" /> [DigiTax Kenya API Hub](https://ke.docs.digitax.tech)\
    This page is DigiTax Kenya API (Version 1) Hub and only applicable if you were using the DigiTax API before version 2 was released. Otherwise we encourage you to use the link above to navigate to the latest API version of DigiTax Kenya 👆.
  * <i class="icon-guides" /> [DigiTax Nigeria API Hub](https://ng.docs.digitax.tech)
  * <i class="icon-guides" /> [DigiTax Zambia API Hub](https://zm.docs.digitax.tech)
</Accordion>

<br />

## Electronic Tax Invoicing in Kenya

African countries lately have been opting to digitize their tax systems by imposing e-Invoicing or Electronic Tax Invoicing and Reporting. Electronic Tax Invoicing is a nascent Fintech category in the Pan-African region.

Kenya is one of the countries and the country's tax authority/ regulator, **KRA** (Kenya Revenue Authority) has a transformative e-invoicing system, named **eTIMS** (electronic Tax Information Management System). In this documentation, DigiTax Kenya API Hub, we shall simply refer to it as *KRA eTIMS* or *eTIMS*.

## Introduction to KRA eTIMS and DigiTax platform

### KRA eTIMS

**eTIMS** (electronic Tax Invoice Management System) is the transformative e-invoicing system by Kenya's country's tax authority, **KRA** (Kenya Revenue Authority). The use of this system and other tax related changes was enacted by the Finance Act, 2023, which was signed on by the President of Kenya on 26 June 2023. Its implementation was halted temporarily by the High Court of Kenya for the next 6 months. It became effective on 1 January 2024 and has been utilized by taxpayers since then.

### DigiTax platform

DigiTax platform, by Namiri Technology (the company), constitutes a suite of digital solutions crafted for effective, simple, and painless tax compliance through **electronic tax invoicing**. These solutions enable taxpayers (individuals and businesses) to generate, digitally sign, and transmit compliant invoices as per connected tax authorities' requirements.

## More about DigiTax

The suite of digital solutions or products under DigiTax, through which one can generate eTIMS invoices, are:

* **DigiTax App** (Compatible with Android and Android POS devices),
* **DigiTax Dashboard** (Responsive, Web-Browser based, Desktop application)
* **DigiTax API** (for system-to-system integration without the issue of platform hopping), and
* **DigiTax Plugins** like DigiTax WooCommerce, DigiTax Odoo, DigiTax Quickbooks, DigiTax Sage Online, among others.

DigiTax connects with regional tax authorities/ regulators, so far:

* ***DigiTax Nigeria*** integrates you with <Glossary>FIRS</Glossary> e-Invoicing System
* ***DigiTax Kenya*** integrates you with <Glossary>KRA</Glossary> eTIMS (electronic Tax Information Management System)
* ***DigiTax Zambia*** integrates you with <Glossary>ZRA</Glossary> Smart Invoice System

to offer you a streamlined invoicing system that ensures compliance and supports the growth of your business.

<Image align="center" border={true} caption="DigiTax - Tax Regulators" src="https://files.readme.io/c4b6c503b46201821ae3d228d057ee6db2585be40a27a8607b90ec0d60b733ff-eInvoice.png" />

### DigiTax API Features

The DigiTax API is built with various industry standards for API platforms in mind. Read more on this [here](https://ke.docs.digitax.tech/v1.0/reference/using-the-digitax-kenya-api#digitax-api).

> We invite you to use **DigiTax Kenya API** to integrate your system with eTIMS for automation and to reduce platform-hopping

***

These include:

* RESTful API
* OpenAPI (formerly Swagger): An open-source standard that allows a standardized way to generate, document, and test our APIs.
* Secure authentication with cryptographically signed JWTs (JSON Web Tokens)

To use this API, you'll need access to DigiTax Dashboard environment to get an X-API-Key. Get in touch with [our team](mailto:support@namiri.tech).

These are the steps required to get up and running - [Prerequisites of using DigiTax API](https://ke.docs.digitax.tech/v1.0/reference/prerequisites-of-using-the-api)

***

### Guaranteed safety and integrity

We comply with industry and security best practices.

> 👍 DigiTax is built with the best industry practices and to the highest security standards

## DigiTax Kenya and eTIMS

> **DigiTax Kenya** integrates you with eTIMS

**DigiTax** is a solution that sits between you; the taxpayer, and the KRA eTIMS.

With DigiTax, you gain access to a streamlined invoicing system that ensures compliance and supports your business's growth. Together, DigiTax and FIRS e-Invoicing are transforming how businesses in Nigeria manage their tax and invoicing obligations.

For us to support individuals and businesses to generate eTIMS invoices, DigiTax is licensed as an eTIMS OSCU integrator/ provider.

**OSCU** stands for ***O**nline **S**ales **C**ontrol **U**nit*. This means that the Control Unit needs to connect to the online KRA eTIMS server to sign/ stamp (generate eTIMS metadata and signature) invoices.

The speed at which eTIMS invoices are generated is dependent on network capacity, connectivity, and responsiveness of KRA's eTIMS server and the Control Unit transmitting the network traffic.

OSCU is different from VSCU. DigiTax doesn't have a VSCU option. That said, the DigiTax team has developed features like **offline URLs**, **callback URLs**, and others which provide compelling value (including VSCU-like service) that our customers rely on daily.

> 🥇 DigiTax is the leading KRA & ODPC-approved eTIMS integrator

## DigiTax Kenya API Hub

This API Hub contains guides and API reference pages for further understanding, equipping you on how to integrate with the DigiTax Kenya API.

### Explore DigiTax Kenya API Guides

Gain understanding of DigiTax Kenya integration through our detailed guides.

You're in the guides section of DigiTax Kenya API Hub. Explore other pages below to gain context on DigiTax and eTIMS and understanding of how DigiTax makes it easier for you to integrate your invoicing system with eTIMS.

### Explore DigiTax Kenya API reference

For a great developer experience, the endpoints in the [DigiTax Kenya API reference](/reference) are interactive.

Once you're set up in the DigiTax Dashboard, you can generate a Test/ LIVE **X-API-Key** for authorization.

Explore the API endpoints [here](/reference)

***

## Once again, welcome to the DigiTax Kenya API Hub

Once again, thank you for reviewing the getting started page of the DigiTax Kenya API hub. We're excited you're here! 💚

We invite you to use **DigiTax Kenya API** to integrate your system with eTIMS for automation and to reduce platform-hopping

To recap:

* Explore our detailed guides to gain understanding of DigiTax Kenya integration. Learn how to navigate them [here](doc:how-to-use-this-site)
* Get the [Prerequisites for using DigiTax Kenya API](https://ke.docs.digitax.tech/update/reference/prerequisites-of-using-the-api)
* For support, [email us](mailto:support@namiri.tech) OR talk to us via the **DigiTax chat** on the bottom-right of any page

Welcome to the Less Taxing solution - DigiTax.

<Image align="center" width="300px" src="https://files.readme.io/f982859d4fdca89de7d179a31795b159cb6c2e34a9a4dc578b85aba910daf13f-Full-Logo_Slogan_Colour.png" />