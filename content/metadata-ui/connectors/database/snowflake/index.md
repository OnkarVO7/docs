---
title: Snowflake
slug: /metadata-ui/connectors/database/snowflake
---

<ConnectorIntro connector="Snowflake" hasUsage="true" hasProfiler="true" hasDBT="true" />

<Requirements />

<MetadataIngestionService connector="Snowflake"/>

<h4>Connection Options</h4>

- **Username**: Specify the User to connect to Snowflake. It should have enough privileges to read all the metadata.
- **Password**: Password to connect to Snowflake.
- **Account**: Enter the details for the Snowflake Account.
- **Role (Optional)**: Enter the details of the Snowflake Account Role. This is an optional detail.
- **Warehouse**: Warehouse name.
- **Database (Optional)**: The database of the data source is an optional parameter, if you would like to restrict the metadata reading to a single database. If left blank, OpenMetadata ingestion attempts to scan all the databases.
- **Private Key (Optional)**: Connection to Snowflake instance via Private Key.
- **Snowflake Passphrase Key (Optional)**: Snowflake Passphrase Key used with Private Key.
- **Connection Options (Optional)**: Enter the details for any additional connection options that can be sent to Snowflake during the connection. These details must be added as Key-Value pairs.
- **Connection Arguments (Optional)**: Enter the details for any additional connection arguments such as security or protocol configs that can be sent to Snowflake during the connection. These details must be added as Key-Value pairs. 
  - In case you are using Single-Sign-On (SSO) for authentication, add the `authenticator` details in the Connection Arguments as a Key-Value pair as follows: `"authenticator" : "sso_login_url"`
  - In case you authenticate with SSO using an external browser popup, then add the `authenticator` details in the Connection Arguments as a Key-Value pair as follows: `"authenticator" : "externalbrowser"`

<IngestionScheduleAndDeploy />

<ConnectorOutro connector="Snowflake" hasUsage="true" hasProfiler="true" hasDBT="true" />
