# Data Flows
Data flow is the first step in integrating various data sources to SkyPoint cloud platform to create customer/patient segmentation, profiles, Audiences and Metrics. This can be accomplished using prebuilt or custom build connectors. The platform already supports 200+ connectors that allows ingestion of data from different data sources with more under various stages of development.
The data connectors move data from a selected data source to Skypoint Customer 360 or Patient 360 through a series of filtering, formatting, and transformation process which is aligned to Common Data model (CDM) and FHIR standards respectively

## Following functions performed by connector includes:
-	Understanding the data source schema, attributes
-	Data transformation
-	Data ingestion
-	Data extraction

### Add Dataflow
1. Click on **Add Dataflow** on the right top corner of the screen.
    - Enter a Name. (Name starts with a letter and only **Letters** and **Numbers** are allowed. No Spcaes)
    - Click **Next**.
    - You will be directed to choose a **Connector**.

### Chosing a Connector
1. Choose a **Connector** listed.
    - You can fiter the list of connectors with respect to the following categories.
      - **All Categories**
      - **Azure**
      - **Database**
      - **File**
      - **Generic Protocol**
      - **NoSQL**
      - **Services and Apps**
    ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/chooseconnector.PNG?raw=true)

### Providing Credentials
1. You will be prompted to enter the following details with respect to the connectors selected. In general section, fill in the display name and the description of the connector and click on **SAVE**. Then go to Connector and follow the instructions.
    - **Amazon S3**
        ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/connects3.PNG?raw=true)
        - **Access key ID** (Check with Amazon S3 source credentials.)
        - **Secret Access Key**
        **S3 Bucket**<br>
        (Select the folder you want download the data from the source)<br>
        Click **Save**<br>
        Once you selcet the S3 Bucket you will see a notification *Data loaded successfuly*
    - **Dynamic365**
        ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/connect.PNG?raw=true)
        - **Username** (Check with Amazon S3 source credentials.)
        - **password**
        - **clienid**
        - **clientsecret**
        - **domain url**

### Connection
Click on Connect

### Saving
Click Save

### Run
After the connection is established, go to the ellipsis under the column name "action" on the right corner of the dataflow row, click and choose start to ingest all the entities.

### Status
After the connection is established and the run operation has also been performed, as a user, you need to know whether everything was successfully processed or not. For that, our platform provides a status column where you can check whether the data was imported correctly or not. The green tick under the status section indicates that the data has been imported and the connection has been established successfully.

### Other Connector Process
Independent method to know more about all other connector process please click [HERE](connectors.md)
