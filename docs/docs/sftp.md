# SFTP(Simple File Transfer Protocol)

SFTP Dataflow enables to integrate data from different sources.
To integrate SFTP Connector, below details are to be configured:
- Host
- Port
- Host Key Fingerprint
- Username
- Password
- Storage path

###### Steps to configuration.

## Step 01 - Connection Estabilishment

1.	Navigate to **Data** > **Dataflows click** on *+ Add Dataflows*
	<img width="940" alt="Image 1" src="https://user-images.githubusercontent.com/96232751/147831573-fdd5319f-5362-4cc5-93ac-bfb76f9538f1.PNG">

2. Under **Select Dataflow name**, mention the connector name.

<img width="715" alt="2" src="https://user-images.githubusercontent.com/96232751/147831843-41334a6d-794a-4436-854a-ff762d40e84e.PNG">

3. From **Choose Connector**, click the connector name **SFTP**. 

<img width="934" alt="3" src="https://user-images.githubusercontent.com/96232751/147831829-3f6c7b93-f84d-40aa-906a-a348962e49f3.PNG">


you will be directed to configuration set up a below.

4.	**Under General**, below the *Dataflow Name*, enter the name of the connector and mention the description about the connector (optional) and click on Save.

<img width="607" alt="4" src="https://user-images.githubusercontent.com/96232751/147831862-f4e21be6-c74e-4a32-87f6-170bd461c2a3.PNG">


5. Click on **Connector**, which is right next to *General*. Under Configuration, mention the details as required and click on connect.
- Host
- Port
- Host Key Fingerprint
- Username
- Password

<img width="557" alt="5" src="https://user-images.githubusercontent.com/96232751/147831886-7372b39e-7281-4e1d-9e67-3502087a77ed.PNG">


## Step 02 - Access Source Data
**In order to allow SkyPoint access to your SFTP account, you'll need the following details:**
- **Host**
- **Port**
- **Host Key Fingerprint**
- **Username**
- **Password**
- **Storage path**
    - Select the folder you would like to download the data from the source.
    - Click **Save**.
    - Once you select the **Storage path** you will see a notification *Data loaded successfuly*.
    - Data from the source will be loaded to the table with headers **File Name**, **Entity Name**, **Datetime Format**, **Delimiter**, 
    - **First Row as Header**, **Advanced Settings**.
        - **File Name**<br>
        The file name will be the name of the file which exist in the source of **SFTP**.
        - **Entity Name**<br>
        **Entity Name** is the unique name that is created for the data collected from the source.
        - **Datetime Format**<br>
        There are various formats for **Datatime Format** available in the SkyPoint platform, and SkyPoint CDP is set to automatically detect the **Datetime Format**.
        - **Delimiter**<br>
        **Delimiter** is the key that is used for setting up a boundary or a separator of veriables in the data imported. Currently the available seperators are, *Comma (,)*, *Semicolon (;)*, *Pipe (|)*, *Tab (\t)*, *Start of Heading (\u0001)* and *No Delimiter*".
        - **First Row as Header**<br>
        This is a checkbox, which calls the first row as Header for the table sheet we are importing. The system will automatically collect the data according to the Header Contents.
        - **Advanced Settings**<br>
        Advanced Settings will allow you to fine tune the import process with minute details.
- **Advanced Settings**
    <br>When you click on the **Advanced Settings** link, you will see a pop-up window with certain additional information. All these informations are key factors of the source data and how it is organized. If you see any error notification, please check with the data source for these additional information.
    - **Compression Type**<br>
    Compression type in **Advanced Settings** is the method that is used for compressing the details from the source, SFTP. (To identify what is the compression methods that's used, please check with your credentials.)
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
## Step 03 - *Action* Button.
Action button includes specific actions on the imported lists.
- **Show All**<br>
When you select **Show All** dropdown, the list will show all the files available in the folder.
- **Show Selected**<br>
Once you click on the **Show Selected** option, the list will show only the selected files from all of the data in the folder.
- **Select All**<br>
With one click you can **Select All** the files in that list imported form selceted folder.
- **Clear All**<br>
If you don't want to get all the folders selected, with just one click of the **Clear All** button all the selections will be removed form the selection.
## Step 04 - Save
- Click **Save** Button.
    - You will be taken to the Dataflow page.

## Files Supported for SFTP
- Comma Separated File - **.csv**
- Data File - **.dat**
- Database File - **.db** or **.dbf**
- Linux/Unix Tarball File Archive - **.tar**
- Log File = **.log**
- Microsoft Access Database File - **.mdb**
- Save File - **.sav**
- SQL Database File - **.sql**
- XML File - **.xml**
