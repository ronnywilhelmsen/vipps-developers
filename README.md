# Vipps Developers

Document version: 2.3.1.

This repository contains various resources for Vipps developers, including:

* [Getting started](vipps-getting-started.md) with Vipps development
* [Settlements](https://github.com/vippsas/vipps-developers/tree/master/settlements)
  for information about settlements
* [How to contribute](contribute.md) to Vipps projects on GitHub

## Table of contents

- [API documentation](#api-documentation)
- [Partners](#partners)
- [Plugins](#plugins)
- [Status page](#status-page)
- [The Vipps test environment (MT)](#the-vipps-test-environment-mt)
- [Postman](#postman)
- [API Dashboard](#api-dashboard)
- [Vipps design guidelines](#vipps-design-guidelines)
- [Vipps API servers](#vipps-api-servers)
- [Vipps request servers](#vipps-request-servers)
- [Additional developer resources](#additional-developer-resources)
- [Questions?](#questions)

## API documentation

See: [Getting started](vipps-getting-started.md).

The most commonly used APIs:
* [Vipps eCom API](https://github.com/vippsas/vipps-ecom-api)
* [Vipps Login API](https://github.com/vippsas/vipps-login-api)
* [Vipps Recurring API](https://github.com/vippsas/vipps-recurring-api)

All Vipps APIs are available here: https://github.com/vippsas

## Partners

See our [Partner section](partners/).

## Plugins

Vipps provides several open source plugins for various web solutions.
See our [Plugins section](https://github.com/vippsas/vipps-plugins).

## Status page

* Test environment: https://vipps-test.statuspage.io
* Production environment: https://vipps.statuspage.io
* BankID production: https://www.bankid.no/status/
* BankID preprod: https://bankidpreprod.statuspage.io

## The Vipps test environment (MT)

See
[The Vipps test environment (MT)](https://github.com/vippsas/vipps-developers/blob/master/vipps-test-environment.md)
for more information about general test functionality,
the iOS and Android test apps, etc

## Postman

See our
[Postman guide](https://github.com/vippsas/vipps-developers/blob/master/postman-guide.md)
or the
[Postman documentation](https://www.getpostman.com/docs/)
for more information about using Postman.

## API Dashboard

All customers have acces to an API Dashboard on
[portal.vipps.no](https://portal.vipps.no) under the "Utvikler" tab.

It show information about your API usage, an overview of errors, etc.
Here's an example for one endpoint:

![API Dashboaard](newsletters/images/2021-02-api-dashboard-initiate-payment.png)

## Vipps design guidelines

Guidelines, logos, buttons, etc is here:
[vipps-design-guidelines](https://github.com/vippsas/vipps-design-guidelines).

## Vipps API servers

* Test (MT): apitest.vipps.no
* Production: api.vipps.no

**Please note:** Vipps may change the IP addresses for the API servers. To ensure
that you are whitelisting the correct IP addresses please use these hostnames
and DNS, and automatically update your firewall rules if there are DNS changes.

## Vipps iremest servers

Requests made by Vipps are made from the servers specified below.
Vipps normally only uses one server at a time, and change servers approximately
every three months.

| Production (Prod)   | Disaster recovery (DR) | Test (MT)              |
| ------------------- | ---------------------- | ---------------------- |
| callback-1.vipps.no | callback-dr-1.vipps.no | callback-mt-1.vipps.no |
| callback-2.vipps.no | callback-dr-2.vipps.no | callback-mt-2.vipps.no |
| callback-3.vipps.no | callback-dr-3.vipps.no | callback-mt-3.vipps.no |
| callback-4.vipps.no | callback-dr-4.vipps.no | callback-mt-4.vipps.no |

The disaster recovery environment is as important as the production environment.

**Please note:** Vipps may change the IP addresses for the request servers. To ensure
that you are whitelisting the correct IP addresses please use these hostnames
and DNS, and automatically update your firewall rules if there are DNS changes.

For API products where Vipps makes requests to your servers, please make sure
that these request servers are allowed through firewalls, etc.

## Additional developer resources

* Developer overview: https://vipps.no/developer
* Products, personal: http://vipps.no/privat
* Products, business: http://vipps.no/bedrift

## Questions?

We're always happy to help with code or other questions you might have!
Please create an [issue](https://github.com/vippsas/vipps-developers/issues),
a [pull request](https://github.com/vippsas/vipps-developers/pulls),
or [contact us](https://github.com/vippsas/vipps-developers/blob/master/contact.md).

Sign up for our [Technical newsletter for developers](https://github.com/vippsas/vipps-developers/tree/master/newsletters).
