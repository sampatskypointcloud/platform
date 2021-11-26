# **Big Query Enrichment**

BigQuery is a data warehousing solution provided by Google Cloud.

**Data**   **enrichment**  is the process of combining first party data from internal sources with disparate data from other internal systems or third-party data from external sources.

**Enriched**  data is an asset for any organization because it becomes more useful and insightful.

Enrichment supplements your customer data with data from external sources including SkyPoint and other partners by creating enrichments from connectors to enrich your data.

**Step 01 – Go to Enrichment and choose BigQuery**

**BigQuery Enrichment** enrich your data with location information like standardized addresses, latitude, longitude.



- Click on BigQuery – Enrich My Data at the top right of the screen.

- Read the disclaimer and proceed by clicking next.



**Step 02 – Connect**

Select the connection you would like to use for enrichment.



- Select the connection for enrichment and click  **Next**.
- Or add new Connection by providing the details – Display Name, ProjectID, Email, Key File.
- Creating connection allows Customer Insights environment to share data with another service.
- To create a connection, provide login details for BigQuery Service Account and Verify.



- **Email** – (obtained from Google console. Available at **IAM-Service Accounts** )
- **Project ID** – (obtained from Google console)
- **Key File (JSON) –** (downloaded from BigQuery service account)
- **Password** – (Service account password)



- **Generate the JSON file:**

Login to BigQuery using the service account details.



- Click **Create Key.**
- Select the format as JSON and click on Create. Once the creation is completed, it will be downloaded and the same can be uploaded while creating the connection to BigQuery. This file contains configuration details.



- This will start a download of .json or .p12 file based on your choice.
- Save the file.

**Step 03 – Required Data**

Provide necessary information:

- **Customer data set:** Choose a data set containing customer profiles you want to enrich.

Eg: Select the Customer data set and choose the entity containing the addresses you want to enrich.

- **Big Query Data:** Choose a data set containing customer profiles related data from BigQuery.

- Click **Next**.



**Step 04 – Attribute Mapping**

- Map your field names to the corresponding BigQuery table fields to get the data based on mapped fields and click **Next**.



**Step 05 – Review and Run**

- Review all details and click **Next**.



- **Entity:**

The below details are displayed in Entity.



Below is the attribute for Sandbox2345 instance. Attributes and Data can be viewed and downloaded here.

