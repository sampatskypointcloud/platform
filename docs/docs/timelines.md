# Timelines

## Timelines
In this section, we show timeline in the different profiles by defining timeline data in your entities. The first half of the section contains a tabular representation of all the created timelines with their information.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileTimelines.png?raw=true)

Some of them are:
1. Icon: Icon of the timeline. 
2. Entity: Corresponds to the entity name that is being used here in the timeline.
3. Source: The connector from which the data was imported.
4. Primary Key: The uniquely identifiable attribute.
5. Event: The event of the timeline.
6. Timestamp: Timestamp field of the timeline.
7. Details: Details fields of the timeline. Maximum 3 fields allowed. 
8. Status : The status of the run command on timeline.
9. Action: Click on **Edit** icon to edit the timeline and Click on **Delete** icon to delete the timeline.

The second half of this section contains a tabular representation of the history regarding all the actions performed in this section.

## Steps to create a Timeline

1. Navigate to **Profile** > **Timelines** and click on **Add timeline**.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileAddTimeline1.png?raw=true)
 - Select the entity for your timeline.
 - Select the primary key of that entity.
 - Select the last updated field of the entity.
 - Click on **Save & Proceed** or click on **Set up relationship** from left menu.
2. Set up relationship.                               
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileAddTimeline2.png?raw=true)
 - Click on **Add relationship** to add relationship.                             
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileAddTimeline3.png?raw=true)
 - Select the field from your timeline entity.
 - Select the customer entity.
 - Select the field from the customer entity.
 - Enter the relationship name.
 - Click on **Apply**.
 - Click on **Save & Proceed** or click on **Define the timeline** from left menu.
3. Define the timeline.                       
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileAddTimeline4.png?raw=true)
 - Select the timestamp for which you want the timeline.
 - Select the event for which you want the timeline.
 - Select the web address for which you want the timeline. (optional).
 - Select detail fields for which you want the timeline. Maximum 3 fields allowed. 
 - Select the icon of the timeline.
 - Click on **Save & Proceed** or click on **Set activity type** from left menu.
4. Set activity type.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileAddTimeline5.png?raw=true)
 - Select activity type **Select from existing** or **Create new**
 - Select the activity type or enter new activity type.
 - Click on **Save & Proceed** or click on **Review** from left menu.
 5. Review.                                            
 ![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileAddTimeline6.png?raw=true)
 - Display detail of the timeline.
 - Click on **Edit** to update any step configuration.
 - Click on **Save & Close** to create the timeline.

## Run timeline
1. Navigate to **Profile** > **Timelines** and click on **Run**.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/ProfileTimelinesRun.png?raw=true)
2. Select refresh type **Full** or **Incremental**.
3. Full refresh: Running a full refresh will update all dataflow and data entities.
4. Incremental refresh: When running an incremental refresh only the data that has changed gets updated. 
5. Click on the **Run**.