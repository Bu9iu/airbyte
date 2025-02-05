# Hellobaton

## Sync overview

This source can sync data from the [hellobaton API](https://app.hellobaton.com/api/redoc/). At present this connector only supports full refresh syncs meaning that each time you use the connector it will sync all available records from scratch. Please use cautiously if you expect your API to have a lot of records.

## This Source Supports the Following Streams

- activity
- companies
- milestones
- phases
- project_attachments
- projects
- task_attachemnts
- tasks
- templates
- time_entries
- users

Hellobaton adds new streams fairly regularly please submit an issue or PR if this project doesn't support required streams for your use case.

### Data type mapping

| Integration Type | Airbyte Type | Notes |
| :--------------- | :----------- | :---- |
| `string`         | `string`     |       |
| `integer`        | `integer`    |       |
| `number`         | `number`     |       |
| `array`          | `array`      |       |
| `object`         | `object`     |       |

### Features

| Feature           | Supported?\(Yes/No\) | Notes |
| :---------------- | :------------------- | :---- |
| Full Refresh Sync | Yes                  |       |
| Incremental Sync  | No                   |       |
| Namespaces        | No                   |       |

### Performance considerations

The connector is rate limited at 1000 requests per minute per api key. If you find yourself receiving errors contact your customer success manager and request a rate limit increase.

## Getting started

### Requirements

- Hellobaton account
- Hellobaton api key

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                             | Subject                             |
| :------ | :--------- | :------------------------------------------------------- | :---------------------------------- |
| 0.2.13 | 2024-08-10 | [43465](https://github.com/airbytehq/airbyte/pull/43465) | Update dependencies |
| 0.2.12 | 2024-08-03 | [43233](https://github.com/airbytehq/airbyte/pull/43233) | Update dependencies |
| 0.2.11 | 2024-07-27 | [42678](https://github.com/airbytehq/airbyte/pull/42678) | Update dependencies |
| 0.2.10 | 2024-07-20 | [42232](https://github.com/airbytehq/airbyte/pull/42232) | Update dependencies |
| 0.2.9 | 2024-07-13 | [41888](https://github.com/airbytehq/airbyte/pull/41888) | Update dependencies |
| 0.2.8 | 2024-07-10 | [41538](https://github.com/airbytehq/airbyte/pull/41538) | Update dependencies |
| 0.2.7 | 2024-07-09 | [41277](https://github.com/airbytehq/airbyte/pull/41277) | Update dependencies |
| 0.2.6 | 2024-07-06 | [40838](https://github.com/airbytehq/airbyte/pull/40838) | Update dependencies |
| 0.2.5 | 2024-06-26 | [40445](https://github.com/airbytehq/airbyte/pull/40445) | Update dependencies |
| 0.2.4 | 2024-06-22 | [40195](https://github.com/airbytehq/airbyte/pull/40195) | Update dependencies |
| 0.2.3 | 2024-06-15 | [39113](https://github.com/airbytehq/airbyte/pull/39113) | Make compatible with builder |
| 0.2.2 | 2024-06-06 | [39189](https://github.com/airbytehq/airbyte/pull/39189) | [autopull] Upgrade base image to v1.2.2 |
| 0.2.1 | 2024-05-21 | [38507](https://github.com/airbytehq/airbyte/pull/38507) | [autopull] base image + poetry + up_to_date |
| 0.2.0 | 2023-08-19 | [29490](https://github.com/airbytehq/airbyte/pull/29490) | Migrate CDK from Python to Low Code |
| 0.1.0 | 2022-01-14 | [8461](https://github.com/airbytehq/airbyte/pull/8461) | 🎉 New Source: Hellobaton |

</details>
