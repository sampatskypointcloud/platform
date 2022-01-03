# Azure Blob Storage

In order to allow SkyPoint access to your Azure Blob Storage account, you'll need:

1. **Storage Account Name**
2. **Account Key**
3. **Storage Path**

## Steps to Import Data Using Azure Blob

1. Navigate to **Data** > **Dataflows** and click on *Add Dataflow* button present on top right side of the platform.
2. Fill in the name of the connector and click on **Next**.
3. You will see all the different types of connectors present infront of you. In the search bar present on top right, type Azure Blob Storage and select the Azure Blob Storage connector.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/azureblobconnect.PNG?raw=true)

4. Next, fill in the display name and type in a breif description about the connector in the ***general section*** and then go to ***Connector Section*** to configure the connector with our platform.
5. Enter all the necessary details and click on **Connect**. It might take some time to finish up, depending upon the data size.
6. Once its completed, you will be able to see the imported entities below the Connect button.
7. Once you select the **Storage path** you will see a notification *Data loaded successfuly*.
    - Data from the source will be loaded to the table with headers **File Name**, **Entity Name**, **Datetime Format**, **Delimiter**, **First Row as Header**, **Advacned Settings**.
        - **File Name**<br>
        The file name will be the name of file which exist in the source of **Azure Data Lake Storage Gen2**.
        - **Entity Name**<br>
        **Entity Name** is the unique name that is created for the data collected from the source.
        - **Datetime Format**<br>
        There are a number of **Datatime Format** is available and SkyPoint CDP is set to automatically detect the **Datetime Format**.
        - **Delimiter**<br>
        **Delimiter** is the key that is used for setting up a boundary or a separator of veriables in the data imported. Currently the available seperators are, *Comma (,)*, *Semicolon (;)*, *Pipe (|)*, *Tab (\t)*, *Start of Heading (\u0001)* and *No Delimiter*".
        - **First Row as Header**<br>
        This is a checkbox, which call the first row as Header for the table sheet we are importing. The system will automatically collect the data according to the Header Contents.
        - **Advacned Settings**<br>
        Advanced Settings will allow you to fine tune the import process with minute details.
    - **Advanced Settings**<br>
    When you click on the **Advanced Settings** link, you will see a pop-up window with certain additional information. All these informations are key factors of the source data and how it is organized. If you are getting any errors, please check with the data source for these additional information.
    - **Compression Type**<br>
    Compression type in **Advanced Settings** is the method that is used for compressing the details from the source, Azure Data Lake Storage Gen2. (To identify what is the compression methods that's used, please check with your credentials.)
    - **Row Delimiter**<br>
    The data stream will have a seperator that identify the boundaries of it's flow. If there were any different separator is used in it, that information need to be changed to get more accuracy in data ingestion.
    - **Encoding**<br>
    Since the data is coming in data stream there is always a kind of encoding used for decyphering it. If any seperate value of mentioned in the encoding process, you may need to select the appropriate encoding. Default encoding is **UTF-8**.
    - **Escape Character**<br>
    An escape character is a particular case of metacharacters. Which given an identification of sequence start or end. You can manually select the **Escape Character** from the dropdown.
        - \"/" **Forward Slash**
        - "\\" **Backshlash**
        - **No Escape Character**
    - **Quote Character**<br>
    There are three **Quote Character** types are mentioned in the advanced **Quote Character** dropdown.
        - (") **Double Quote**
        - (') **Single Quote**
        - **No Quote Character**

8. Follow [this](https://skypointcdpdocs.z22.web.core.windows.net/docs/dataflows.html) to get a better understanding of how to input data. This will be beneficial for data processsing as the data will be stored in a convenient manner. 
9. As the data gets integrated, we will be able to see the number of entities present in that dataflow. On successful completion of the process, the status of the dataflow will be a green check denoting that the data has been integrated and can now be taken into further usages.

10. In entities, we will be able to see the names of the different entities present in the data, the number of records present in each entity, entity type(**default: Custom**) and many more. There are filters present on top of every column which gives user the ability to search a particular entity based on some criteria. By clicking on a particular entity, we can get its details like the **attributes** defining all the different attributes present in the data with their datatypes. To know more about the entities, visit [here](https://skypointcdpdocs.z22.web.core.windows.net/docs/entities.html)

11. Next, based on the requirements, the data can be processed using the Stitch operation offered on our Platform. The data that has been collected in the previous processes is now ready for some mapping. For that, we provide the **Stitch** option that helps the user to map different entities and find correation between entities and create a cumulative entity with maximum information on the data. The Stich involves three different types of actions which helps in refining the data. They are:
    - Map: Mapping involves correlating different entities in a dataflow using specific feature attributes so as to produce a more extractable data-form.
    - Match: After successful completion of Map, we are ready to match the entities. The match phase specifies how to combine your datasets into a cumulative customer profile dataset. 
    - Merge: The final phase of Stitch is Merge where we choose and exclude attributes to merge within or mapped and matched data. Some of the attrbiutes are automatically merged.

To know more about Stitch, click [here](https://skypointcdpdocs.z22.web.core.windows.net/docs/stitch.html)