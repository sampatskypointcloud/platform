# Stitch Process : MAP

1. After importing the data, we now begin the Map process in the stitch section of our platform as the first step to create a customer profile.
2. Navigate to **Stitch** > **Map** and click on Select Entities.
3. Select the different entities that needs to be mapped.
4. Click on each entity and complete the mapping for the various types of required fields.

![image](https://user-images.githubusercontent.com/93347291/146684641-2aa386f2-7754-46a1-87c3-e263db5b04ff.png)

5. Select the primary key for each entity.
6. System automatically Maps the scemantic labels based on its inbuilt algorithms. All mapped attributes will be displayed in the table Above and all unmapped attributes will be shown in the table below.
7. By manually selecting a scemantic mapping to the unmapped attributes, they will move to the mapped table
8. User can revise the mapping by clicking on the ML Type drop down
9. Clicking on the advanced setting will allow you to configure various data clensing techniques like converting all texts to lower/upper case, remove any white spaces between strings, Replace with a custom value, Replace with a Regex expression, Adding prefix/suffix etc 
10. Click on Save button in the top ribbon. Once application displayes **Saved successfully**, click on the Run button to start the map process.
11. If the user is running the map for the first time, system takes it as a full run. Any further runs , user will have an option to chose between full run or incremental run
12. Chose relevant option from the drop down and click on Run button to kick off the run process

![image](https://user-images.githubusercontent.com/93347291/146685436-e3951839-e0c2-4e67-983e-6b998a9843aa.png)

13. You can click on discard changes button at the top ribbon to discard all the changes from last save
14. Cancel Run button can be used to cancel a Run that is in progress
