# RingCentral

This page contains the setup guide and reference information for the [RingCentral](https://developers.ringcentral.com/api-reference/) source

## Prerequisites

Auth Token (which acts as bearer token), account id and extension id are mandate for this connector to work, Account token could be recieved by following (Bearer ref - https://developers.ringcentral.com/api-reference/authentication), and account_id and extension id could be seen at response to basic api call to an endpoint with ~ operator. Example- (https://platform.devtest.ringcentral.com/restapi/v1.0/account/~/extension/~/business-hours)

## Setup guide

### Step 1: Set up RingCentral connection

- Get your bearer token by following auth section (ref - https://developers.ringcentral.com/api-reference/authentication)
- Setup params (All params are required)
- Available params
  - auth_token: Recieved by following https://developers.ringcentral.com/api-reference/authentication
  - account_id: Could be seen at response to basic api call to an endpoint with ~ operator. \
     \ Example- (https://platform.devtest.ringcentral.com/restapi/v1.0/account/~/extension/~/business-hours)
  - extension_id: Could be seen at response to basic api call to an endpoint with ~ operator. \
     \ Example- (https://platform.devtest.ringcentral.com/restapi/v1.0/account/~/extension/~/business-hours)

## Step 2: Set up the RingCentral connector in Airbyte

### For Airbyte Cloud:

1. [Log into your Airbyte Cloud](https://cloud.airbyte.io/workspaces) account.
2. In the left navigation bar, click **Sources**. In the top-right corner, click **+new source**.
3. On the Set up the source page, enter the name for the RingCentral connector and select **RingCentral** from the Source type dropdown.
4. Enter your `auth_token, account_id, extension_id`.
5. Click **Set up source**.

### For Airbyte OSS:

1. Navigate to the Airbyte Open Source dashboard.
2. Set the name for your source.
3. Enter your `auth_token, account_id, extension_id`.
4. Click **Set up source**.

## Supported sync modes

The RingCentral source connector supports the following [sync modes](https://docs.airbyte.com/cloud/core-concepts#connection-sync-modes):

| Feature                       | Supported? |
| :---------------------------- | :--------- |
| Full Refresh Sync             | Yes        |
| Incremental Sync              | No         |
| Replicate Incremental Deletes | No         |
| SSL connection                | Yes        |
| Namespaces                    | No         |

## Supported Streams

- user_business_hours
- company_business_hours
- callblock_settings
- blocked_allowed_phonenumbers
- forwarding_numbers
- company_call_handling_rules
- user_call_records
- user_active_calls
- call_monitoring_groups
- call_queues
- call_record_settings
- greetings
- ivr_prompts
- fax_cover

## API method example

GET https://platform.devtest.ringcentral.com/restapi/v1.0/account/~/extension/~/business-hours

## Performance considerations

RingCentral [API reference](https://platform.devtest.ringcentral.com/restapi/v1.0) has v1 at present. The connector as default uses v1.

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                       | Subject        |
| :------ | :--------- | :------------------------------------------------- | :------------- |
| 0.1.13 | 2024-08-10 | [43662](https://github.com/airbytehq/airbyte/pull/43662) | Update dependencies |
| 0.1.12 | 2024-08-03 | [43148](https://github.com/airbytehq/airbyte/pull/43148) | Update dependencies |
| 0.1.11 | 2024-07-27 | [42591](https://github.com/airbytehq/airbyte/pull/42591) | Update dependencies |
| 0.1.10 | 2024-07-20 | [42294](https://github.com/airbytehq/airbyte/pull/42294) | Update dependencies |
| 0.1.9 | 2024-07-13 | [41891](https://github.com/airbytehq/airbyte/pull/41891) | Update dependencies |
| 0.1.8 | 2024-07-10 | [41433](https://github.com/airbytehq/airbyte/pull/41433) | Update dependencies |
| 0.1.7 | 2024-07-10 | [41328](https://github.com/airbytehq/airbyte/pull/41328) | Update dependencies |
| 0.1.6 | 2024-07-06 | [40973](https://github.com/airbytehq/airbyte/pull/40973) | Update dependencies |
| 0.1.5 | 2024-06-25 | [40480](https://github.com/airbytehq/airbyte/pull/40480) | Update dependencies |
| 0.1.4 | 2024-06-22 | [40054](https://github.com/airbytehq/airbyte/pull/40054) | Update dependencies |
| 0.1.3 | 2024-06-06 | [39111](https://github.com/airbytehq/airbyte/pull/39111) | Make compatible with builder |
| 0.1.2 | 2024-06-04 | [38937](https://github.com/airbytehq/airbyte/pull/38937) | [autopull] Upgrade base image to v1.2.1 |
| 0.1.1 | 2024-05-20 | [38382](https://github.com/airbytehq/airbyte/pull/38382) | [autopull] base image + poetry + up_to_date |
| 0.1.0   | 2023-05-10 | [Init](https://github.com/airbytehq/airbyte/pull/) | Initial commit |

</details>
