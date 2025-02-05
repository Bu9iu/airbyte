# Northpass LMS

This page contains the setup guide and reference information for the Northpass LMS source connector.

## Prerequisites

- A [Northpass LMS Account](https://www.northpass.com) at least
<!-- env:oss -->
- A Northpass API Token generated [here](https://developers.northpass.com/docs/api-authentication)
  <!-- /env:oss -->

## Setup guide

<!-- env:oss -->

### Step 1: (For Airbyte Open Source) Setup a Northpass LMS Account

Setup and account in [Northpass](https://www.northpass.com/). 


### Step 2: (For Airbyte Open Source) Obtain an api key

A simple api key is all that is needed to access the Northpass LMS API. This token is generated [here](https://developers.northpass.com/docs/api-authentication).


#### For Airbyte Cloud:

To set up Northpass LMS as a source in Airbyte Cloud:

1. [Log in to your Airbyte Cloud](https://cloud.airbyte.com/workspaces) account.
2. In the left navigation bar, click **Sources**. In the top-right corner, click **+ New source**.
3. Find and select **Northpass LMS** from the list of available sources.
4. Enter a **Source name** of your choosing.
5. Enter the **api key** you obtained from Northpass LMS.
6. Click **Set up source** and wait for the tests to complete.

<!-- /env:cloud -->

<!-- env:oss -->

#### For Airbyte Open Source:

To set up Northpass LMS as a source in Airbyte Open Source:

1. Log in to your Airbyte Open Source account.
2. In the left navigation bar, click **Sources**. In the top-right corner, click **+ New source**.
3. Find and select **Northpass LMS** from the list of available sources.
4. Enter a **Source name** of your choosing.
5. Enter the **api key** you obtained from Northpass LMS.
6. Click **Set up source** and wait for the tests to complete.

<!-- /env:oss -->

## Supported Sync Modes

The Northpass LMS source connector supports the following [sync modes](https://docs.airbyte.com/cloud/core-concepts#connection-sync-modes):

- [Full Refresh - Overwrite](https://docs.airbyte.com/understanding-airbyte/connections/full-refresh-overwrite/)
- [Full Refresh - Append](https://docs.airbyte.com/understanding-airbyte/connections/full-refresh-append)

Incremental modes are not supported as the Northpass LMS API at the time of this writing.

## Supported Streams

The Northpass LMS source connector can sync the following streams.

### Main Tables

Link to Northpass LMS API documentation [here](https://developers.northpass.com/docs/).

- [People](https://developers.northpass.com/reference/get_v2-people)

- [Courses](https://developers.northpass.com/reference/get_v2-courses)

- [Course Enrollments](https://developers.northpass.com/reference/get_v2-courses-course-uuid-enrollments)

## Changelog

<details>
  <summary>Expand to review</summary>

| Version  | Date       | Pull Request                                             | Subject                                                                                                                              |
|:---------|:-----------|:---------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------|
| 0.1.1 | 2024-08-10 | [43484](https://github.com/airbytehq/airbyte/pull/43484) | Update dependencies |
| 0.1.0 | 2024-08-06 | [43319](https://github.com/airbytehq/airbyte/pull/43319) | New Source: Northpass LMS |
</details>
