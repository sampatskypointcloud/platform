# Session Defaults

Session lifetimes are an important part of authentication for balancing security and the number of times users are prompted for their credentials.

When users authenticate, a session is established. For the duration of the session, users wont need to re-authenticate. Sessions can expire when users are inactive, when they close the browser or tab, or when their authentication token expires for other reasons. SkyPoint Studio allows the user to manage these timeouts inside the tenant through session settings.

**Session Defaults**.

**Note** : The user also gets a warning on the screen through a pop up that has a dynamic countdown to notify the user about the timeout.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/TimeoutSession.PNG?raw=true)

## Steps to Set Up a Session Default

1. Login to the platform and navigate to **Settings** > **Platform**.
2. Go to **Session Defaults**. By default it is turned off.
3. Click on the toggle switch to activate the session expiration section.
4. Fill in all the details required.
    - **Maximum Session Length** : The duration after which the user will be logged out automatically and asked for login again.
    - **Duration of inactivity before timeout** : The duration of inactivity after which the user will be logged out and asked to login again.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PlatformSessionSettings.png?raw=true)
