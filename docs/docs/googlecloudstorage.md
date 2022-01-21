# **Google Cloud Storage**

Dataflows allows to integrate all your data sources by ingesting data from the sources, transforming and loading into the data lake in Common Data Model (CDM) schema.

**Step 01 - Add Dataflow**

- Click on **Add dataflows** at the top of the screen.

![image](https://user-images.githubusercontent.com/93347291/145796781-d163203f-1502-4973-8f7f-512690c2280a.png)

  - Enter a Name for the dataflow (name should start with letter and it should contain only letter and numbers, space and special characters are not allowed)
  - Click Next.

![image](https://user-images.githubusercontent.com/93347291/145797129-3d91fdc3-6a29-486d-a254-5717a5a66109.png)


  - Select the connector using the search bar at top right corner of the screen.
  - Click on Google Cloud Storage (S3 API).

![image](https://user-images.githubusercontent.com/93347291/145796240-eb119299-e45c-45de-8b98-f87812400d5d.png)


**Step 02 - Access Source Data**

- In the general tab You will see the data flow name you defined in the first step which is not editable.
- Please enter a display name for the connector. This is not a mandatory feild and can be left empty
- Please enter a description to provide more details about the connector. This is not a mandatory feild and can be left empty
- Clicking on save button will save the details you just entered
- Clicking on Cancel button will take you back to the dataflow page

![image](https://user-images.githubusercontent.com/93347291/145798277-9f72112e-b384-47fb-aa98-7627bbd5d720.png)

Click on connector Tab

Following details are required to establish connection with Google Cloud storage

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/File_loaded.png)

- **Access Key ID** – (obtained from Google Cloud Platform, login using service account)
- **Secret Access Key** – (obtained from GCP, login using service account)
- **Project ID** – (obtained from GCP, login using service account)
- **Service URL –** (obtained from client)
- **Service Account Config File (JSON) –** (downloaded from GCP service account)
- **Storage path** – (obtained from GCP, login using service account)

- Select the folder you want to download the data from the source.
- Click Save.

Client will have to create a service account and the connection details for the service account will be used to login to Google Cloud Platform.

- **How to generate the JSON file mentioned in the previous step:**

Log on to **Google Cloud Platform** using service account credentials, navigate to **Service Accounts** and click on the three dots to locate **Manage Details**.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/GCP_Manage_Details.png?raw=true)

Click on **Manage Details** and find **keys** and **Create New Key**

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Key_creation.png)


Select the format as JSON and click on Create. Once the creation is completed, it will be downloaded and the same can be uploaded to **Service URL** while creating the Dataflow. This file contains configuration details.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/JSON_file.png)

Create roles and assign permissions to the roles which grants access to the buckets -to list and get the buckets.

- **Required Permissions:**

Below mentioned permissions are required for GCS connector to work.

1. storage.objects.get
2. storage.objects.list
3. storage.buckets.list

The first 2 permissions are available in Storage Object Viewer Role.

The 3rd permission can be availed by creating a new Custom Role with only the 3rd permission.

Once you select the Storage path you will see a notification Data loaded successfully.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/Data_Loaded.png)

Data from the source will be loaded to the table with headers File Name, Entity, Name, Datetime Format, Delimiter, First Row as Header, Advanced Settings.

- **File Name:**
The file name will be the name of file which exist in the source of Google Cloud Storage.
- **Entity Name:**
 Entity Name is the unique name that is created for the data collected from the source.
- **Datetime Format:**
 There are several Datetime formats available and SkyPoint CDP is set to automatically detect the Datetime Format.
- **Delimiter:**
 Delimiter is the key that is used for setting up a boundary or a separator of variables in the data imported. Currently the available separators are Comma (,), Semicolon (;), Pipe (|), Tab (\t), Start of Heading (\u0001) and No Delimiter.
- **First Row as Header:**
 A checkbox, which call the first row as Header for the imported table sheet. The system will automatically collect the data according to the Header Contents.
- **Advanced Settings:**
 Advanced Settings will allow you to fine tune the import process with minute details.
 
  ![image](https://user-images.githubusercontent.com/93347291/145802278-1e4872a6-b4da-4a04-9532-411a45c917d8.png)

**Advanced Settings:**

Clicking the Advanced Settings icon opens a pop-up window with additional information - key factors of the source data and how it is organized. For any errors, check the data source for this additional information.

![image](https://user-images.githubusercontent.com/93347291/145800950-7719c28e-4264-4306-85ba-a76e76b7c26f.png)

- **Compression Type:**
Compresses the details from the source, Google Cloud Storage. (To identify what is the compression methods that is used, please check with your credentials.)
- **Row Delimiter:**
The data stream will have a separator that identify the boundaries of its flow. If any different separator is used in it, that information needs to be changed to get more accuracy in data ingestion.
- **Encoding:**
Encoding is used for deciphering data as data is obtained as data stream. If any separate value is mentioned in the encoding process, select the appropriate encoding. Default encoding is UTF-8.
- **Escape Character:**
An escape character is a particular case of metacharacters which givens an identification of sequence start or end. You can manually select the Escape Character from the dropdown.

    - \"/" **Forward Slash**
    - "\\" **Backshlash**
    - **No Escape Character**
- **Quote Character:**
The three Quote Character types in the advanced Quote Character dropdown are:

    - (") **Double Quote**
    - (') **Single Quote**
    - **No Quote Character**

**Step 03 - Save**

- Click Save Button.
- You will be taken to the Dataflow page.
