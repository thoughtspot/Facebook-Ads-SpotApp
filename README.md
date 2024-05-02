# Facebook Ads SpotApp

SpotApps are ThoughtSpot’s out-of-the-box solution templates built for specific use cases and data sources. They utilize ThoughtSpot Modeling Language (TML) Blocks, which are pre-built pieces of code that are easy to download and implement directly from the product.

The Facebook Ads SpotApp mimics the Facebook data model. When deployed, it creates several Worksheets, Answers, and Liveboards based on your Facebook data in your cloud data warehouse.

This is a sample Liveboard, created after you deploy the Facebook Ads SpotApp:
![Facebook Ads SpotApp Liveboard](https://github.com/thoughtspot/Facebook-Ads-SpotApp/assets/102629468/4ee94f6f-4e1d-4bfe-bfd9-a6fcc82a6501)

Use the Facebook Ads SpotApp to measure ad performance across platforms to grow reach, engagement, and sales.

## Prerequisites

Before you can deploy the Facebook Ads SpotApp, you must complete the following prerequisites:

- **Review Required Data**: Examine the required tables and columns for the SpotApp.
- **Ensure Column Compatibility**: Make sure that your columns match the required column type listed in the schema for your SpotApp.
- **Sync Data**: Synchronize all tables and columns from Facebook to your cloud data warehouse. While you can choose to sync only the required tables and columns, ThoughtSpot recommends syncing all tables and columns from Facebook to ensure comprehensive data availability. This includes Facebook’s out-of-the-box columns or any custom columns you are using.
- **Collaborate on Data Movement**: If you are using an ETL/ELT tool or working with another team within your organization, sync all columns from the tables listed in the SpotApp.
- **Obtain Credentials**: Acquire credentials and SYSADMIN privileges to connect to your cloud data warehouse. The warehouse must contain the data ThoughtSpot will use to create Answers, Liveboards, and Worksheets.
- **Unique Connection Name**: Each new SpotApp connection name must be unique.
- **Administrator Access to Facebook**: Maintain administrator access to manage Facebook.
- **Access to Facebook Tables**: Ensure access to the following Facebook tables in your cloud data warehouse:
  - `FBADS_CAMPAIGN`
  - `FBADS_AD`
  - `FBADS_AGE_GENDER`
  - `FBADS_CONVERSION`
  - `FBADS_GEO`
  - `FBADS_VIDEO`

Refer to the Facebook Ads SpotApp schema for more details on the data structure and requirements.

## Deploy the SpotApp

After you have downloaded the Zip file and verified its contents, follow these steps:

1. Log into your ThoughtSpot instance and create an Embrace connection to all of the relevant views.
2. Import the TML for the Worksheets and verify that it has all been imported without any errors.
3. Import the TML for the Liveboards and verify that it has all been imported without any errors.
4. You are ready to start searching your data!

For detailed instructions on how to import TML files, refer to the [ThoughtSpot documentation](https://docs.thoughtspot.com/software/latest/tml-import-export-multiple).


