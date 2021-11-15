# Overview
SkyPoint unifies fragmented customer data from multiple systems and applications into comprehensive “customer 360” profiles and provides business and technology users with the tools to secure, govern, and access that data. 
## Skypoint cloud is a Privacy first customer data platform having following features:

- **Data enhancement** : By ingesting data via 200+ connectors across different domains like healthcare, Ecommerce, Retail and Hospitality etc. and providing valuable data insights. These data insight helps the customer in achieving following:
o	Operational Efficiency
o	Profits
o	Consumerization 
o	Productivity
o	Mitigating Risk 
o	Planning
o	Cost cutting

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Dashboard.png)

- **Data Privacy** : It centered around how data should be collected, stored, managed, and shared with any third parties, as well as compliance with the applicable privacy laws (such as California Consumer Privacy Act- CCPA or General Data Protection Regulation GDPR).

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Domains.jpg)

 Skypoint cloud platform is architected as a a multi-tenant SaaS platform where, each customer is a tenant, and each tenant having one or more instances ensuring data security.
 
 ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Multitenant.png)
 
- Once ingestion is done, the data goes through different processes such as Map, Match, ML match, Merge processes to draw valuable insights and convert the unstructured data into structured data.
Left Navigation bar gives access to some of the key features such as:
  1. Home
  2. Data
  3. Privacy
  4. Insights
  5. Action
  6. Settings

## **Skypoint cloud platform glossary**
- **Tenants** : Each customer is called a Tenant.
- **Instances** : You can consider them as subsidiaries of a single client. As soon as you create an account on our platform, a default instance is created for you namely Sandbox.
- **Dataflows (Integrations - Import)** : It allows you to ingest data from all your sources, transform and load into the data lake complying with the Common Data Model (CDM).
- **Channels** : They are the visitor touchpoints that you want to monitor with SkyPointCloud.
- **Entities** : Individual data sources that are present in the dataflows.
- **Stitch** : Data Processing is performed in this section. It consists of 3 sub-sections: Map, Match & Merge.
  - *Map* : It defines the profile data in your entities by choosing the profile attributes, primary key, and types (datatypes defined by SkyPoint Cloud).
  - *Match* : It identifies the unique profiles in your entities by matching records based on certain rules.
  - *Merge* : It creates an entity of profile records by combining duplicate attributes and removing attributes you don’t need.
- **Timelines** : It depicts the entire customer's journey consisting timeline details of  specific entities and attributes in the customer profiles 
- **Associations** : used to create associations/relationships among  entities.
- **Custom Models** : Helps in Integrating artificial intelligence and machine learning models by deploying them as web service endpoints to utilize unified entities (e.g. predictions on unified customer profile and activities).
- **Profiles** : They are  generated after the entire stitch process is complete. It contains unified unique records.
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

