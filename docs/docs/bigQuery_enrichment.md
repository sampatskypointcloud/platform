# **Big Query Enrichment**

BigQuery is a data warehousing solution provided by Google Cloud.

**Data**   **enrichment**  is the process of combining first party data from internal sources with disparate data from other internal systems or third-party data from external sources.

**Enriched**  data is an asset for any organization because it becomes more useful and insightful.

Enrichment supplements your customer data with data from external sources including SkyPoint and other partners by creating enrichments from connectors to enrich your data.

**Step 01 – Go to Enrichment and choose BigQuery**

**BigQuery Enrichment** enrich your data with location information like standardized addresses, latitude, longitude.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Enrichment.png?raw=true)




- Click on BigQuery – Enrich My Data at the top right of the screen.

- Read the disclaimer and proceed by clicking next.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Step1-%20Overview.png?raw=true)




**Step 02 – Connect**

Select the connection you would like to use for enrichment.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Step%202-%20Connect.png?raw=true)



- Select the connection for enrichment and click  **Next**.
- Or add new Connection by providing the details – Display Name, ProjectID, Email, Key File.
- Creating connection allows Customer Insights environment to share data with another service.
- To create a connection, provide login details for BigQuery Service Account and Verify.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Create%20connection.png?raw=true)




- **Email** – (obtained from Google console. Available at **IAM-Service Accounts** )
- **Project ID** – (obtained from Google console)
- **Key File (JSON) –** (downloaded from BigQuery service account)
- **Password** – (Service account password)



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Service%20Account.png?raw=true)




- **Generate the JSON file:**

Login to BigQuery using the service account details.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Key%20Creation.png?raw=true)



- Click **Create Key.**
- Select the format as JSON and click on Create. Once the creation is completed, it will be downloaded and the same can be uploaded while creating the connection to BigQuery. This file contains configuration details.




![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Select_key_format.png?raw=true)



- This will start a download of .json or .p12 file based on your choice.
- Save the file.

**Step 03 – Required Data**

Provide necessary information:

- **Customer data set:** Choose a data set containing customer profiles you want to enrich.

Eg: Select the Customer data set and choose the entity containing the addresses you want to enrich.

- **Big Query Data:** Choose a data set containing customer profiles related data from BigQuery.

- Click **Next**.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Step%203-%20Required%20Data.png?raw=true)




**Step 04 – Attribute Mapping**

- Map your field names to the corresponding BigQuery table fields to get the data based on mapped fields and click **Next**.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Step%204-%20Attribute%20Mapping.png?raw=true)




**Step 05 – Review and Run**

- Review all details and click **Next**.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Step%205-%20Review.png?raw=true)




- **Entity:**

The below details are displayed in Entity.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Entity_BigQuery.png?raw=true)



Below is the attribute for Sandbox2345 instance. Attributes and Data can be viewed and downloaded here.



![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Entity_download.png?raw=true)

