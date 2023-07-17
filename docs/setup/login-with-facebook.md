---
title:   Configure Firebase
sidebar_label:   Configure Firebase
---

# Configure Firebase
To configure** Firebase** api follow the steps below.


- Log into https://firebase.google.com/ using **email** and **password**.
- Click on **Add Project** and then click **Create New Project** with require information

![OvoyLMS](assets/ovoy/firebase.png)
![OvoyLMS](assets/ovoy/firebase_2.png)
![OvoyLMS](assets/ovoy/firebase_3.png)
![OvoyLMS](assets/ovoy/firebase_4.png)

- Now this credentials have to fill up in **System Setup -> Firebase.**



# Configure login with Facebook

 - Log into https://developers.facebook.com using facebook **email** and **password**.
 - Click on **My App** and then click the **Add New App**.
 - Give the name of the app and then click on **Create App ID**. It will automatically redirect to the App dashboard.
 - Then go to **Settings -> Basic.**
 - Set the **App Domains** and click on **Save Changes**.
 - Get the **App ID** and **App Secret**.
 - Now go to firebase>authentication
   ![Docusaurus Plushie](../../../static/yoori/firbase_6.png)
 - Add your domain to the firebase console
   ![Docusaurus Plushie](../../../static/yoori/firbase_12.png) 
 - Now click on **Add New Provider** and select **Facebook.**
![Docusaurus Plushie](../../../static/yoori/firebase_7.png)
 - Then give the **App ID** and ** App Secret**
   ![Docusaurus Plushie](../../../static/yoori/firebase_8.png)
 - Copy call back url and paste here
   ![Docusaurus Plushie](../../../static/yoori/firebase_9.png)

# login with Google
- just enable the switch button
 ![Docusaurus Plushie](../../../static/yoori/firebase_10.png)

# Configure login with Twitter

- Go to https://developer.twitter.com/en/apps
- Click on **Create An App**.
- Fill in your **application details**.
- After creating the app follow their steps to get **client Id** & **client secret**.
- Then give it to firebase
-  ![Docusaurus Plushie](../../../static/yoori/firebase_12.png)
