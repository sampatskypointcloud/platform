# What's new in the SkyPoint platform

We're excited to announce our newest updates and releases! This article summarizes public preview features, general availability enhancements, and feature updates. To see the long-term feature plans see the bottom of this page.

> [!TIP]
> To submit feature requests and product suggestions, email us at support@skypointcloud.com or use Github issues.

# February 2022 updates

The updates in Fenruary 2022 include new features.

## Sprint 216 Release

### Feature Upadates

#### SkyPoint Profile:

- **Show Enriched attributes in Profile details page** - User can now view the enriched attributes in Profile Details page.
- **Predictive models output added in Profile details page** - User can now view the Prediction about the Profile in Profiles details page.
- **Support Multiple details attributes from Timelines and view in customer Journey in Profile details page** - User can now add multiple( max 3) attributes when creating the timelines. The same will be visible under "Customer Journey" in Profile details page. 

#### SkyPoint Predict:

- **Custom Model added for Single Upload** - Users can now test their own model using the Custom model feature in SkyPoint Studio. Implementation supported for Single data upload in the current release.

#### SkyPoint Automate:

- **Activate section added in Navigation Panel** - Automate section added in Navigation panel in SkyPoint Studio. User can now go to  Power Apps, Power automate, Microsoft Teams, SkyPoint Api from here.

#### SkyPoint Activate:

- **Readable String Support added for Query builder in Audience** - User can now view the readable form of query from Audience query builder which will help in ease of understanding and usage.
- **"Profile All records included" added in Audience Query builder** - There is no requirement to explicitly add Profile entity for saving the Audience. Application will automatically include all records from the Profile and Relate to the entity selected in Query builder of Audience.
- **Select attributes to be downloaded in Audience** - USer can now select the Attributes to be downloaded from the Audience section.
- **Select Attributes to be exported from each entity in Export** - User can now select attributes to be exported fromeach enity in export.

#### SkyPoint Resolve:

- **Cleanup moved before validation in Map process** - Design change implemented to add cleanup before validation in Map process.

#### Settings and Admin

- **Restrict multiple sign up from same email** - User is retricted from multiple sign up with same email in SkyPoint Studio.

# January 2022 updates

The updates in January 2022 include new features and bug fixes.

## Sprint 215 Release

### Resolved Issues: 

#### SkyPoint Resolve:

- **Pagination issue in Merge section** - Pagination issue has been fixed for merge section under stitch.
- **Do not allow user to delete already mapped entity** - User cannot delete already mapped entity now which was leading to inconsistencies.

### Feature Updates

#### SkyPoint Dataflow:

- **Visualize ERD's for Relationships** - ERD's for both user defined and system defined relationships can now be visualized to see the relationships between different entities.
- **Show both User defined and System generated Relationships** - User can now view both the user defined and system defined relationships under Relationships list view.

#### SkyPoint Profile:

- **Create Audience from filtered Profile** - It is now possible to create Audiences from the filtered profile view giving user the ease for Audience creation.

#### SkyPoint Resolve:

- **Intelligent Mapping Support** - Intelligent mapping option has been provided which can be used by the user for semantic mapping where system automatically selects the required semantic traits. While Intelligent mapping is ON, user still can edit the mapping and save.


## Sprint 214 Release


### Feature Updates

#### SkyPoint Dataflow:

- **New connector support for Data Relay** - Data Relay connector has been added to Dataflow > Integrations. The connector takes SFTP and SQL server credentials to connect to the Data Relay. Currently only one time load is supported. Incremental load is not yet supported.
- **Feature to add same Datetime format for all entities** - User can now select the option to add same Datetime format for all the entities required for integration when adding Connector details.

#### SkyPoint Profile:

- **UI changes for Profile card** - UI for Profile card has been modified using Fluent UI.
- **Sorting in Profile card view** - Sorting is now supported in profile card view. All the attributes added in the profile card are available for sorting.

#### SkyPoint Activate:

- **SFTP export destination added** - Export to SFTP location is now supported in SkyPoint Studio.
- **Fluent UI changes for Export** - UI for export has been modified using fluent UI.
- **Fluent UI changes for Audience** - UI for audience has been modified using fluent UI.

#### SkyPoint Predict:

- **Product name to be shown in Production recommendation Model output** - Product Recommendation output now shows product names which previously showed Product Id's.

#### Settings and Administration:

- **Contextual Documentation from SkyPoint Studio** - User is now directed to contextual documentation link based on the current section.
- **Left navigation panel to be in sync with SkyPoint product lines** - Left navigation panel has been modified to reflect the features alignment based on SkyPoint product lines.


# December 2021 Updates

The updates in December 2021 include new features and bug fixes.

## Sprint 213 Release

### Resolved Issues:

#### SkyPoint Predict:
1. Save Option added to Prediction Model configuration. Earlier user could only select "Save and Run".

#### SkyPoint Profile:
1. "Group by" filter has been fixed for entities.

#### SkyPoint Activate:
1. List of exports are now shown in reverse chronological order.

### Feature Updates:

#### SkyPoint Activate:

- **"Select from existing" option in export for File based connectors**-  The Option "Select from existing" in case of exporting File system based connectors has been added. It allows to use the exsiting credentials from dataflow connectors.

#### SkyPoint Resolve:

- **UI changes for Stitch Process** - UI for Stitch involving Map, Rule match, ML match and Merge has been modified using Fluent UI.

## Sprint 212 Release

### Resolved Issues:

#### SkyPoint Dataflow:
1. Created date in Dataflows has been fixed to reflect the created date time instead of showing current date time.

#### SkyPoint Predict:
1. "Preview" text has been removed from Prediction Models.

#### SkyPoint Activate:
1. "Preview" text has been removed from Audience.

#### Settings and Administration:
1. Pipeline failures when running scheduler has been fixed.
2. Issue while disabling the scheduler has been fixed.

### Feature Updates

#### SkyPoint Profile:

- **UI changes for Relationships** - UI for Relationships has been modified using Fluent UI.

#### Settings and Administration:

- **Scheduler Save and Edit Option** - Save is enabled when setting the scheduler for the first time. Once saved, the option to Edit is available.

# November 2021 Updates

The updates in November 2021 include new features and bug fixes.

## Sprint 212A Release

### Resolved Issues:

#### SkyPoint Dataflow:
1. UI issue for Tapin2 connector logo has been fixed.
2. Salesforce Marketing Cloud: User can now download only the required activities. Previously, all activities in the list were downloaded irrespective of the selection.
3. Floating header issue in entities has been fixed.

#### SkyPoint Empower:
1. Data settings tab is now working fine under Privacy Center. The error "Something went wrong" has been fixed.

#### SkyPoint Activate:
1. Decimal type attributes can now be added when creating business metrics.

#### SkyPoint Profile:
1. Navigation issues while transitioning different states during configuring enrichments has been fixed.
2. New Connection in Enrichment can now be saved. "Save" was shown disabled even after successful validation of the connection.
3. Activity Stream in Dashboard now displays activies in reverse chronological order.

## Sprint 211 Release

### Resolved Issues:
1. Pagination has been removed and breadcrumbs have been added on UI in **Dataflow** when adding new connectors.
2. UI issues in entities section have been fixed.
  - Total record count under entities is now visible. 
  - Filter option for Actions has been removed.

### Feature Updates

#### SkyPoint Profile:

- **Big query enrichment possible with only key validation** - Big query enrichment connection can be verified using Key file, project id and email id. There is no requirement to add Json file for validation.

- **UI changes for enrichment** - UI for enrichment has been modified using Fluent UI.

- **UI changes for entities** - UI for entities, attribute and data has been modified using Fluent UI.

#### SkyPoint Dataflow:

- **Tapin2 connector** - Tapin2 connector support has been added in Dataflow section.

- **Label inactive integrations** - Any datasource integrations which are not yet enabled show "Coming Soon" on hover.

#### SkyPoint Predict:

- **SkyPoint Predict**: UI for Prediction has been modified using Fluent UI.

- **UI changes for Custom Models** - UI for custom models has been modified using Fluent UI.

## Sprint 210 Release

### Resolved Issues:
1. UI issue related to incorrect header label for "Actions" under Insights > My Predictions has been fixed.

### Feature Updates
**Customer 360**:

- **Backup functionality for Instances** - Create and Restore Backup feature has been added for Instances. 

- **Associations renamed to Relationships**- UI change for renaming associations to Relationships has been implemented.

# October 2021 Updates 

The updates in October 2021 include new features, performance upgrades, and bug fixes.

## Sprint 210 mid-sprint Release

### Resolved Issues:
1. Skypoint Documentation link on the platform redirects to Overview page now. Previously user could only see Index page.
2. UI issues for Big Query enrichment have been fixed. The count of records enriched and the enriched data values are correctly visible under Entities.
3. UI issues for SFTP enrichment have been fixed. The count of records enriched and the enriched data values are correctly visible under Entities.

### Feature Updates: 

**Customer 360**:

- **UI changes for Timelines** - Timelines section view has been modified using Fluent UI.

- **UI changes for Dashboard widgets** - Widgets on the Dashboard have been  modified using Fluent UI.

- **View Instance Details** - Details for the Instances have been added- Refresh cadence, Organization ID , Security group and Type are available for every Instance. User can further edit to add more fields in Instance details.

- **Reset Functionality for Instances** - Reset functionality has been added under Instances. Three options are available for reset: **CDP data, Datavault data and Privacy center data**. Under CDP, further there are 3 options: 'Reset everything', 'Keep all dataflows', 'Keep all dataflows, settings for stitch and profile entity'.


## Sprint 209 Full Release 

### Resolved Issues:
1.Data, Insights and Actions get selected together on UI, only one should be shown as selected
2.Platform Level : Configured Audiences Not showing Up In Audience Page : Error 500
3.Unwanted text if0/00 is displayed on menu bar in place of sidebar collapse option

### Feature Updates: 

**Customer 360**:

- **Persist unique ID from previous run for Full refresh when running ML match**: The feature provisions that the same unique ID's are used in case of full refresh for ML match.

- **Enrichment for customer profiles using SFTP**: Enrich the profiles with data from SFTP now. The funtionality needs connection details, path to the SFTP file, user profile which needs to be enriched and attribute mapping between the user profile and the SFTP file. Save the enrichment created and hit Run. Currently, only csv file format is supported for SFTP enrichment.

- **UI changes for Dashboard** - UI for dashboard has been modified using fluent UI. Changes can be seen in the side bar, the headers, the cards section and the activity stream. Changes for the Graph section are in progress.

- **UI changes for Settings** - Settings section view has been modified using Fluent UI.

- **Cleanse your data by eliminating redundant records**: New feature has been added to remove the duplicate rows before mapping process. 

- **Export on schedule**: Three types of schedulers have been enabled for export. On every system refresh, every day and every week. Different time zones and timing can also be selected.

- **Create a new Instance from existing one**: Copy from existing instance funtionality takes care of copying the configurations for dataflow, enrichment, entity, timelines, metrics, audience, association, stitch and export.

- **Instance management history option**: History has been enabled for Instances.

- **FHIR Connector Support**: Support to import data from FHIR has been enabled in Dataflow. 
