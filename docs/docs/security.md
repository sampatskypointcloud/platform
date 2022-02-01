# Users

We align to the NIST 800-207 standard for Zero Trust. This is the most vendor neutral, comprehensive standards, not just for government entities, but for any organization. It also encompasses other elements from organizations like Forrester’s ZTX and Gartner’s CARTA.
 
This section is one of the key features for any platform as it ensures a secure and safe environment to work on data that is sensitive in all aspects. To provide security, there are certain roles defined to ensure that every user gets access to only those sections of the platform which they actually require preventing unncessary access to anyone.

User has option to Create user,  Invite user, Assign role, Unlink user and Delete user.
On the platform users can be invited by email and can be assigned the required role to access the SkyPoint platform.

Every row in the Users list view corresponds to a single user and every column has some specific entity related to that user. Some important column attributes are:
1. Name: Name of the user with the email address.
2. Source: Account which was used for Login
3. Type: Default is *User*.
4. Role: The assigned role to that particular user.
5. Status: *Active* if the user is currently a part of the tenant and *Inactive* if the user is currently blocked for the tenant.
6. Multi-Tenant: *Yes* if the user is currently given access to more than one tenant and *No* if the user is currently given access to only one tenant.
7. Action: This is an option when you want to quickly delete, unlink or block a user. To perform any of the three actions, click on the 3 dot icon and select the action you want to perform.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PlatformUsers.png?raw=true)

## Steps to Create a new User
1. Click on *Create Users* written on top of the page. A small window will pop up on top of the page.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/createuser.PNG?raw=true)
2. Select the role which you want to assign the user.
3. Fill all the details of the user under the specific fields and click on **Save**.

## Steps to Invite a User
1. Click on *Invite Users* written on top of the page. A small window will pop up on the right side of the page.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/inviteuser.PNG?raw=true)
2. Select the type of role you want to assign. You will see the various roles listed in the dropdown menu.
3. Fill in the email ids for the users whom you want to invite and assign the particular role.
4. Click on **Save** to complete the assignment process. The user will be assigned with that particular role and the entry will be made in the details table.

## Steps to Assign a Role to a user
1. Click on *Assign Role* written on top of the page. A small window will pop up on the right side of the page.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/assignrole.PNG?raw=true)
2. Select the type of role you want to assign. You will see the various roles listed in the dropdown menu.
3. Search for the user whom you want to assign the particular role.
4. Click on **Save** to complete the assignment process. The user will be assigned with that particular role and the entry will be made in the details table.

## Steps to Unlink User
1. Click on the checkbox on the side of the user which you want to unlink.
2. You will see that the *Unlink users* button on top of the page will be enabled. Click on it to unlink the user/s.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PlatformUsersUnlink.png?raw=true)

## Steps to Delete User
1. Click on the checkbox on the side of the user which you want to delete.
2. You will see that the *Delete users* button on top of the page will be enabled. Click on it to delete the user/s.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PlatformUsersUnlink.png?raw=true)

## All Invited Users and their Acceptance Status
When a user is invited on this platform with certain roles assigned to him/her, a track record gets feed on into this table with certarin attributes for every user details. Some of the details are:
1. Email: Email address of the user who got invited.
2. Role: The designated role assigned to the user.
3. Send Date: The date and time on which the invitation request was sent.
4. Resend Date: The date and time on which the invitation request was resent.
5. Status: *Accepted* if the user accepted the invitation, *Pending* if the user's has not yet accepted the invitation and *Expired* if the user was not able to accept the invitation whthin 24hrs.
6. Accepted Date: The date and time when the invitation was accepted.
7. Invited By: The designated person who invited the user.
8. Action: If, for some reasons the user was not able to accept the invitation within 24hrs, the platform provides a  feature where you can resend the invitation just by clicking on the 3 dot icon below the action column.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PlatformInvitedUsers.png?raw=true)