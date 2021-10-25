# Release Notes v1.1

- These release notes provide information about new features and updates that are included in skypointcloud application.
    

## Release 2110 : October 22
build:

### Resolved Issues:
1.Data, Insights and Actions get selected together on UI, only one should be shown as selected
2.Platform Level : Configured Audiences Not showing Up In Audience Page : Error 500
3.Unwanted text if0/00 is displayed on menu bar in place of sidebar collapse option

#### Feature Updates: 

**Customer 360**:

- **Persist unique ID from previous run for Full refresh when running ML match**: The feature provisions that the same unique ID's are used in case of full refresh for ML match.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/FullWithPersistentId.png?raw=true)

- **Enrichment for customer profiles using SFTP**: Enrich the profiles with data from SFTP now. The funtionality needs connection details, path to the SFTP file, user profile which needs to be enriched and attribute mapping between the user profile and the SFTP file. Save the enrichment created and hit Run. Currently, only csv file format is supported for SFTP enrichment.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/SFTP.png?raw=true)

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileSelectionSFTP.png?raw=true)

- **UI changes for Dashboard** - UI for dashboard has been modified using fluent UI. Changes can be seen in the side bar, the headers, the cards section and the activity stream. Changes for the Graph section are in progress.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/FluentUIDashboard.png?raw=true)

- **UI changes for Settings** - Settings section view has been modified using Fluent UI.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Settings.png?raw=true)

- **Cleanse your data by eliminating redundant records**: New feature has been added to remove the duplicate rows before mapping process. Steps to follow:
1. Select the list of attributes to be considered under "Column Type".
2. Record to keep has 3 options:
    a. Most Recent (takes only date and int format in "Based on field")
    b. Least Recent ( takes only date and int format in "Based on field")
    c. Most Filled ("Based on field" remains disabled)
3. Save and Run the Map process in order to see the source and unique record counts

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/recordToKeep.png?raw=true)

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/MostRecent.png?raw=true)

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/DuplicateRecords.png?raw=true)

- **Export on Schedule**: Three types of schedulers have been enabled for export.
1. On every system refresh
2. Every day
3. Every Week
Different time zones and timing can also be selected.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ExportOption.png?raw=true)

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ExportScheduler.png?raw=true)

- **Create a new Instance from existing one**: Copy from existing instance funtionality takes care of copying the configurations for dataflow, enrichment, entity, timelines, metrics, audience, association, stitch and export.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/CopyInstance.png?raw=true)

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/copiedfeatures.png?raw=true)

- **Instance Management history option**: History has been enabled for Instances.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/InstanceHistory.png?raw=true)

- **FHIR Connector Support**: Support to import data from FHIR has been enabled in Dataflow. 
