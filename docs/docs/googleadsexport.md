# Google Ads Manager

Export lets you to export the cdm files to Google Ads Manager.

## Steps to Export
1. Navigate to **Active** > **Export**. You will see all the differenet categories of storages that can be used for export.

2. Go to **destimations** and click on ***Add Export** if the export connect is not there in the export gallery
3. Fill up the name and the display name of the export and click on the dropdown column to select one of the type options. Here we select Google Ads.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/GoogleAdsManager_export.PNG)

4. Fill up the **Customer ID** and **Developer Token** and then click on **Authenticate Google Ads**. It will open a pop up where you will be asked to sign in using your Google Ads Account.
5. **Note** : In order to get the customer ID, sign in to the google ads portal and click on your profile icon present on the top right of the window. There will be a XXX-XXX-XXXX format number visible there, which will be your **customer ID**. To get your **developer token**, you need to sign in to the manager google ads account, and navigate to **Tools & Settings** > **API Center** and get the developer token from there. If not present, you can create a new one too from the same destination. 
5. Once you enter all required credentials and authenticate your account, click on **Next**. You will be able to see all the CDM data available infront of you entity wise. Choose all the entities that you will need to export.
6. Click on **Save**. Your export will be saved. You can run it now and the entities will be exported.
If the export connector- Google Ads manager is already present in the export gallery then click on setup.
Fill the details- Name, Display name, Customer ID, Developer Token.
Click Next.

Here all CDM data will be available Entity wise.
 - Select the enities from the list to be exported
 - Click Create and then click on three dot button and select Run.
 - The export will be started.
