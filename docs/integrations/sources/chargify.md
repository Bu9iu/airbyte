# Chargify

## Overview

The Chargify source supports Full Refresh syncs for Customers and Subscriptions endpoints.

### Available streams

Several output streams are available from this source:

- [Customers](https://developers.chargify.com/docs/api-docs/b3A6MTQxMDgyNzY-list-or-find-customers)
- [Subscriptions](https://developers.chargify.com/docs/api-docs/b3A6MTQxMDgzODk-list-subscriptions)

If there are more streams you'd like Airbyte to support, please [create an issue.](https://github.com/airbytehq/airbyte/issues/new/choose)

### Features

| Feature                       | Supported? |
| :---------------------------- | :--------- |
| Full Refresh Sync             | Yes        |
| Incremental Sync              | No         |
| Replicate Incremental Deletes | No         |
| SSL connection                | Yes        |
| Namespaces                    | No         |

### Performance considerations

The Chargify connector should not run into Chargify API limitations under normal usage. Please [create an issue](https://github.com/airbytehq/airbyte/issues) if you see any rate limit issues that are not automatically retried successfully.

## Getting started

### Requirements

- Chargify API Key
- Chargify domain

### Setup guide

Please follow the [Chargify documentation for generating an API key](https://developers.chargify.com/docs/api-docs/YXBpOjE0MTA4MjYx-chargify-api).

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                             | Subject                                     |
| :------ | :--------- | :------------------------------------------------------- | :------------------------------------------ |
| 0.4.13 | 2024-08-10 | [43612](https://github.com/airbytehq/airbyte/pull/43612) | Update dependencies |
| 0.4.12 | 2024-08-03 | [43222](https://github.com/airbytehq/airbyte/pull/43222) | Update dependencies |
| 0.4.11 | 2024-07-27 | [42765](https://github.com/airbytehq/airbyte/pull/42765) | Update dependencies |
| 0.4.10 | 2024-07-20 | [42300](https://github.com/airbytehq/airbyte/pull/42300) | Update dependencies |
| 0.4.9 | 2024-07-13 | [41811](https://github.com/airbytehq/airbyte/pull/41811) | Update dependencies |
| 0.4.8 | 2024-07-10 | [41375](https://github.com/airbytehq/airbyte/pull/41375) | Update dependencies |
| 0.4.7 | 2024-07-09 | [41130](https://github.com/airbytehq/airbyte/pull/41130) | Update dependencies |
| 0.4.6 | 2024-07-06 | [40962](https://github.com/airbytehq/airbyte/pull/40962) | Update dependencies |
| 0.4.5 | 2024-06-25 | [40314](https://github.com/airbytehq/airbyte/pull/40314) | Update dependencies |
| 0.4.4 | 2024-06-22 | [40123](https://github.com/airbytehq/airbyte/pull/40123) | Update dependencies |
| 0.4.3 | 2024-06-15 | [38814](https://github.com/airbytehq/airbyte/pull/38814) | Make connector compatible with builder |
| 0.4.2 | 2024-06-06 | [39306](https://github.com/airbytehq/airbyte/pull/39306) | [autopull] Upgrade base image to v1.2.2 |
| 0.4.1 | 2024-05-20 | [38444](https://github.com/airbytehq/airbyte/pull/38444) | [autopull] base image + poetry + up_to_date |
| 0.4.0 | 2023-10-16 | [31116](https://github.com/airbytehq/airbyte/pull/31116) | Add Coupons, Transactions, Invoices Streams |
| 0.3.0 | 2023-08-10 | [29130](https://github.com/airbytehq/airbyte/pull/29130) | Migrate Python CDK to Low Code |
| 0.2.0 | 2023-08-08 | [29218](https://github.com/airbytehq/airbyte/pull/29218) | Fix schema |
| 0.1.0 | 2022-03-16 | [10853](https://github.com/airbytehq/airbyte/pull/10853) | Initial release |

</details>
