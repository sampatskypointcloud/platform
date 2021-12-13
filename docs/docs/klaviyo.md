# Klaviyo Setup Guide
Follow our setup guide to connect **Klaviyo** to  **SkyPoint**.

## Step 01 - Add Dataflow

- Click on **Add Dataflow** on the right top corner of the screen.
    - Enter a Name. (Name starts with a letter and only **Letters** and **Numbers** are allowed. No Spcaes)
    - Click **Next**.
    - You will be directed to choose a **Connector**.
    
    ![image](https://user-images.githubusercontent.com/93347291/145803521-0e588f2a-5a6b-4daa-bb85-3cedea5e403c.png)

## Step 02 - Access Source Data 
**In order to allow SkyPoint access to your Klaviyo account for data ingest, you'll need the following details:**

General Tab
- Please enter display name and Description. Both are not mandatory feilds.
- Click on save

![image](https://user-images.githubusercontent.com/93347291/145804467-a2b9677b-533f-48ad-b790-d3fafa12cd8a.png)

Connector Tab
- Enter the API key and click on connect button 
![image](https://user-images.githubusercontent.com/93347291/145805156-82902799-2ef6-4cfc-80f9-2a54ba733b08.png)
   
   - Upon clicking the Connect button, it will validate your credentials, if it is successful you will see a notification **Data loaded successfully** else it will show the error that login has failed.

   - Upon successful connection, platform will show the names of all entities ready to be ingested from Klaviyo like **Lists, Campaigns and Metrices**  with headers like Name, Type, Purpose etc. You will also see a message "Data loaded sucessfully" 

## How to Obtain API Key from Klaviyo
Perform the following steps to retrieve the API Key:

1. Log in to **Klaviyo** ( Please request customer to provide you required access to Klaviyo)
2. Go to **Account>>Settings**
3. Click on **API Key**


## Step 03 - Select Entities
1. Use the checkbox to select the entities that needs to be ingested
2. Use pagination to naviagte to next page and select additional entitities
3. Click on the save button. This completes your configuration

## Step 04 - Run Data Ingestion

-	Use the breadcrumb to navigate backt to the dataflow page.
-   You should see Klviyo dataflow already created 
-   Click on the three dots under Actions as shown in the image below 
-   ![image](https://user-images.githubusercontent.com/93347291/145807139-c5dc3958-4e92-44ac-9ad9-8b1d34a33f93.png)
-   Chose Run from the context menu and kick the data ingestion process on.
-	Upon successful run three entities will be created named klaviyo_metrices from all Metrices, klaviyo_lists from all Lists and klaviyo_campaigns from all Campaigns.


