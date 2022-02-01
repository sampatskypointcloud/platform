# Permissions

## Platform supports 4 different roles:
1. **Viewer**: Permission to view an instance.
2. **Contributor**: Permission to contribute to the platform post admin permissions.
3. **Instance Admin**: Permission to view, edit and manage current instance.
4. **Tenant Admin**: Permission to view, edit and manage current tenant and all of its instances. 
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PlatformPermissions.png?raw=true)

### Permissive actions for a Viewer
1. Explore insight on the Home Page.
2. Within the Data section of the platform, a viewer can:
    - View the Dataflows that are established within your tenant and instance, including the state and the latest update.
    - View and filter data Entities.
    - View and explore data mapping and criteria associated with the map and match steps within Stitch process.
    - Explore data entities that will display in customer profiles in the Timelines.
    - Review data Relationships for your source and target entities.
3. Within the Privacy section of the platform, a viewer can:
    - View your Data and PII Maps
    - Search and filter established Data Process Activities and view your Consent Flags.
    - Search and filter the Data Subject Request queue and review the Run History.
4. Search and filter customer profiles using the Profiles page.
5. View and explore Profile Details including Customer Profiles, Timeline and Metrics.
6. Explore and export entities using the Entities page.
7. View the status of system processes using the System page.
8. Export Audiences from the **Actions** > **Export** page to either a *.CSV file* or to an Export destination.

### Permissive Actions for a Contributor
1. All permissions available to the Viewer.
2. Load and transform data using the Data sources page.
3. Complete the Data Unification sections (Map, Match, and Merge) which result in the unified customer profile entity.
4. Define Relationships and Activities.
5. Create Audiences using the Insights > Audiences page.
6. Create metrics using the Action > Metrics page.
7. Manage configuration and enrich customer profiles from the Enrichment page (for first party enrichments only).

### Permissive Actions for Administrator
1. All permissions available to the Contributor.
2. Change settings on the **Settings** > **Platform** > **Users** , including the working language and refresh schedules for your system processes.
3. View and add users and specify roles using the Security page.
4. Set up and Configure Audience destinations using the Export destinations page.
5. Add and use the Power Apps connector to create apps with SkyPoint Cloud data.

**Note**
1. Permissions availed to the tenant administrator are only limited to the particular tenant and all of its instances.
2. Permissions availed to the instance administrator are only limited to a particular instance and **not to** any other instances present in the same tenant.
