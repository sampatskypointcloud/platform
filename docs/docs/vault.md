# Vault
SkyPoint Vault separates and secures data in a zero-trust vault that integrates with applications through a simple API or SQL. Connected to the Microsoft Power Platform, anyone (not just developers) creates and runs applications and workflows to safely accelerate the business.

## Vault
In this section, contains a tabular representation of all the created vault with their information.     
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultList.png?raw=true)

Some of them are:
1. Display name: Display name of the vault. 
2. Name: Name of the vault.
3. Type: Type of the vault (Customer/Health Care/Payment).
4. Entities: Total number of entities in the vault.
5. Status: Status of the vault.
6. Created Date: Created Date of the vault.
7. Updated Date: Updated Date of the vault.
8. Actions: Click on actions to Edit or Remove the vault.

## Steps to create a vault
1. Navigate to **Vault** and click on **Add datavault**.          
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/NewVault.png?raw=true)
2. Enter the display name of the vault.
3. Enter the name of the vault.
4. Select type of the vault (Customer/Health Care/Payment).
5. Enter the description of the vault.
6. Click on **Save**.

## Steps to view entities
Navigate to **Vault** and click on **Display name** of the vault.                        
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityList.png?raw=true)

Some of them are:
1. Entity: Display name of the entity. 
2. Name: Name of the entity.
3. Type: Type of the entity (Activity/Custom/Standard).
4. Customizable: Is entity enable for customization.
5. Tags: Tags of the entity.
6. Actions: Click on actions to Edit or Remove the entity.

## Steps to create entity
1. Navigate to **Vault** > click on **Display name** of the vault > Click on **New entity**.                     
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultNewEntity.png?raw=true)
2. Enter the display name of the entity.
3. Enter the plural display name of the entity.
4. Enter the name of the entity.
5. Enter the primary column display name of the entity.
6. Enter the primary column name of the entity.
7. Check/Uncheck to enable customization of the entity.
8. Enter the description of the entity.
9. Select entity type (Activity/Custom/Standard).
10. Click on **Create**.

## Steps to view entity attributes
Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name**                             
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityAttributes.png?raw=true)

Some of them are:
1. Entity: Display name of the attribute. 
2. Name: Name of the attribute. 
3. Data Type: Data type of the attribute.
4. Type: Type of the attribute.
5. Customizable: Is attribute is Customizable.
6. Required: Is attribute is required.
7. Searchable: Is attribute is searchable.

## Steps to create attribute
1. Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name** > click on **New attribute**        
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityNewAttribute.png?raw=true)
2. Enter the display name of the attribute.
3. Enter the name of the attribute.
4. Select the data type of the attribute.
5. Select the attribute type.
6. Enter the description of the attribute.
7. Check/Uncheck option from more setting (Required/Searchable/Filterable/Sortable/Customizable/Enable Security/Enable Auditing).
8. Click on **Create**.

## Steps to view entity relationships
Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name** > click on **Relationships** tab.   
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityRelationships.png?raw=true)

Some of them are:
1. Relationship name: Display relationship name of the entity. 
2. From enity: Display the from entity name.
3. To entity: Display the to entity name.
4. Relationship type: Display the relationship type (Many To One/One To Many/Many To Many).
5. From attribute: Display the from attribute name.
6. To attribute: Display the to attribute name.
7. Actions: Click on actions to Edit or Remove the relationship.

## Steps to create relationship
1. Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name** > click on **Relationships** tab > Click on **New relationship** > Click on **Many-to-One/One-to-Many/Many-to-many**                          
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityNewRelationship.png?raw=true)
2. Select the related entity.
3. Enter the display name of the relationship.
4. Enter the relationship name.
5. Enter the description of the relationship.
6. Click on **Create**.

## Steps to create entity key
1. Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name** > click on **Keys** tab > Click on **New key**                                                                                                   
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityNewKey.png?raw=true)
2. Enter the display name of the entity key.
3. Enter the name of the entity key.
4. Select the data type of the key.
5. Enter the description of the key.
6. Checked attributes those required of the key.
7. Click on **Create**.

## Steps to view entity data
Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name** > click on **Data** tab               
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityDatas.png?raw=true)
1. A tabular representation of the entity data.
2. Actions: Click on actions to Edit or Remove the record.

## Step to create entity data
1. Navigate to **Vault** > click on **Display name** of the vault > Click on **Entity name** > click on **Data** tab > Click on **New record**                                                                                                     
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultEntityNewData.png?raw=true)
2. Fill the detail and click on **Save** 

## Steps to view choices
Navigate to **Vault** and click on **Display name** of the vault > Click on **Choices** tab.                       
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultChoiceList.png?raw=true)

Some of them are:
1. Display Name: Display name of the choice. 
2. Name: Name of the choice. 
3. Type: Type of the choice.
4. Customizable: Is choice is Customizable.
5. Actions: Click on actions to Edit or Remove the choice.

## Step to create choice
1. Navigate to **Vault** and click on **Display name** of the vault > Click on **Choices** tab > Click on **New choice**          
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/VaultNewChoice.png?raw=true)
2. Enter the display name of choice.
3. Enter the name of the choice.
4. Select the type of the choice.
5. Enter the description of the choice.
6. Check/Uncheck to enable customization of the choice.
7. Add items you want for the choice.
8. Click on **Create**.
