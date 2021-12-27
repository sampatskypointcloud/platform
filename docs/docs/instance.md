# Instance

Every tenant can have multiple instances for example sandbox and production. SkyPointCloud Studio enables to have Instance level settings. Changes in one Instance do not impact the other.

## Creating and Editing an Instance:
There are two options available when creating or editing an Instance.
1. **Copy from existing:**  In case of already created Instances, user has the option to select the settings from the available Instance so that user effort for reseting a new Instance are saved.
2. **Create Instance:** User always has the option to add a new Instance. User needs to select Instance properties when adding a new Instance.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/CreateInstance.PNG?raw=true)


## Instance Properties
1. **Instance name:** This is the unique name of the Application instance.
2. **Time zone:** Click on the drop down to select the timezone which the application should use. By Default timezone will be UTC -07:00 Pacific Time.
3. **Language:**  Click on the drop down to select the preferred language. The Default language will be English.
4. **Date and number format:** Click on the drop down to selct the date format. The date format preview will be shown below.The Default value will United States.
5. **Currency:** Can select the currency type by clicking on the drop down. Default value will be US Dollar (USD) $.

Click on **Save** button.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Instances.PNG?raw=true)

## Operations Available for an Instance:

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/InstanceOptions.PNG?raw=true)

1. **Edit:** USer can edit the properties of already created instance and also can select the option to copy from existing instance.
2. **Remove:** User can delete the existing instance. This option will delete entire data set available for the instance. Any settings related to CDP , Privacy or data vault                  will be deleted.
3. **Reset CDP data:** User can delete CDP data from the Instance which will delete the entities related to Profile. User has following options:              
                     a. **Reset everything:** Reset Ingested data from dataflows, Profile settings, Stitch related entities , Audiences, Relationships, Metrics,                                                             Prediction Models, Enrichment, Export settings and scheduler settings.\
                     b. **Keep all dataflow:** Reset everything except the ingested data and related entities.\
                     c. **Keep all dataflow, settings for stitch and profile entity:** Reset everything except ingested data in dataflow, stitch settings and profile entity.                                               
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ResetCDP.PNG?raw=true)
                     
4. **Reset Privacy data:** User can delete privacy data.
5. **Reset datavault data:** User can delete datavault data.
6. **History:** User can view the history for the Instance.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/InstanceHistory.PNG?raw=true)

7. **Backups:** User can create backup or restore from the saved backup.
