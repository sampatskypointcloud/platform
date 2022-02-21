# Overview
SkyPoint is an industry leading customer data platform (CDP), zero trust data privacy vault, privacy compliance automation, analytics and AI for customer centric brands in several industries including healthcare, retail, hospitality, entertainment and financial services.   

## SkyPoint platform has the following products:

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Products.png?raw=true)

1.	**SkyPoint Dataflow** : Data import via integrations, data quality, data transformations to Common Data Model (CDM) entities and semantic data labeling. 
2. **SkyPoint Resolve** : Machine learning and rule based customer identity resolution & management.
3. **SkyPoint Profile** : 360-degree view of the customer including profile, timelines and enrichment capabalities. 
4. **SkyPoint Predict** : Predict customer needs from unified data, ML models built in and ability to integrate custom models.
5. **SkyPoint Vault** :  Zero trust data privacy vaults deliver security, compliance and governance via a simple API. 
6. **SkyPoint Empower** : Customer consent management and effortless compliance with global privacy laws (CCPA, GDPR).
7. **SkyPoint Activate** : Capabilities including audiences, metrics, export and API developer portal. 
8. **SkyPoint Automate** : Automate workflows, build power apps, build dashboards using SkyPoint Power BI, Power App, Power Automate and Teams connectors.

## SkyPoint platform architecture:

SkyPoint platform is architected as a a multi-tenant SaaS platform where, each customer is a tenant, and each tenant having one or more instances.
 
 ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Multitenant.png?raw=true)
 
## How SkyPoint helps in deriving business decissions using in-built Prediction models.
 
SkyPoint platform has multiple prediction models which can be used to predict the customer behavior based on customer's interactions over a period of time. These can be used to derive business decissions.
 
 ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Predictions.png?raw=true)
 

## **SkyPoint platform glossary**

- **Tenants** : Each customer is called a Tenant.
- **Instances** : You can consider them as subsidiaries of a single client. As soon as you create an account on the platform, a default instance is created for you namely Sandbox.
- **Dataflows (Integrations - Import)** : It allows you to ingest data from all your sources, transform and load into the data lake complying with the Common Data Model (CDM).
- **Datavaults** : Zero trust data privacy vault with compliance to Common Data Model (CDM).
- **Channels** : They are the visitor touchpoints that you want to monitor with SkyPointCloud.
- **Entities** : Each data source ingested from the dataflows is added as an entity in the entity section. Entities are further added from Stitch Process which is the Profile entity, from Audiences , from Enrichment and from Metrics.
- **Stitch** : Data Processing is performed in this section. It consists of 3 sub-sections: Map, Match & Merge.
  - *Map* : It defines the profile data in your entities by choosing the profile attributes, primary key, and types (datatypes defined by SkyPoint Cloud).
  - *Match* : It identifies the unique profiles in your entities by matching records based on certain rules.
  - *Merge* : It creates an entity of profile records by combining duplicate attributes and removing attributes you don’t need.
- **Timelines** : It depicts the entire customer's journey consisting timeline details of  specific entities and attributes in the customer profiles 
- **Relationships** : It is used to create associations/relationships between entities which can be further used when creating Audiences and Metrics.
- **Custom Models** : The feature allows the user to bring their own machine learning model and utilize the data from SkyPoint Studio to get the quality score.
- **Profiles** : Profiles depict unified customers. Multilple entities ingested are stitched together with Identity resolution and ML model to generate a 360 view of unique customers. 
- **Audiences** : It is a group of profiles characterized by a defined set of attributes based filters. You can schedule audiences to be auto-updated every day or update them manually for onetime use.
- **Metrics** : Helps in tracking the performance of an organizations by providing insights such as business metrices, profile metrices and profile attribute. 
- **Data Maps** : Mapping different entities in a meaningful manner to formulate better insights with the data.  It also provides an easier and powerful way to process, manage and secure the data with minimal complexity.
- **Data Subject Requests** : This allows the customer to create a new Data subject request and shows the DSRs that are currently in review.
- **Export** : It exports the entities to several destinations  using export connectors provided by the platform.
- **Platform** : It consists of notifications, schedule, instance, product, activity stream.
  - *Tenant* : It displays all the basic details of the tenant with all the services assigned to it.
  - *Instance* : It displays the various details of the instance such as Tenant Name, Tenant website URL, Tenant identifier, Instance name, Instance identifier.
  - *Notifications* : It shows the notifications about dataflows and background processes. This sub-section helps to cover the area where we need to check the status of an iteration.
  - *Schedule* : It allows you to set a schedule to refresh all dataflows and autorun platform processes for the selected instance.
  - *Activity Stream* : It displays all the activity which was performed in the application.

