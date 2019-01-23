# Analyze pictures using IBM watson and Node Red.
----------------------------------------------------------------------------------------------------

## Overview
Analyzing pictures became easier recently by using IBM Watson Visual Recognition service. The service will analyze a picture and give you all objects inside the picture with the percentage of accuracy. This project is a sample of visual recognition web app to analyze pictures and detect objects. 

## Learning Objectives
After completing this project, you will understand how to;
- Use Node-RED.
- [Create IBM Watson Visual Recognition](#Create-IBM-Watson-Visual-Recognition)
- [Create the flow](#Create-the-flow)
- [Configure IBM Watson Visual Recognition on Node-RED](#Configure-IBM-Watson-Visual-Recognition-on-Node-RED)

## Prerequisites
In order to complete this project, you will need the following prerequisites:
- [IBM Cloud](http://ibm.biz/iot-cloud-signup) account - sign up if you don't have an account yet.
- [Node-RED starter](https://console.bluemix.net/catalog/starters/node-red-starter)
- [IBM Watson Visual Recognition](https://console.bluemix.net/catalog/services/visual-recognition) service.


## Estimated Time
- Create IBM Watson Visual Recognition should take less than 3 minutes.
- Creating and configure your Node-RED application on IBM Cloud should take less than 10 minutes.
- Developing the complete application on Node-RED should take a maximum 10 minutes.
- Overall the time for completing this project should take approximately 25 minutes.

### Create IBM Watson Visual Recognition

Open your IBM Cloud account then **click** on _Catalog_ --> _AI_ --> _Visual Recognition_ 
![`watson_visual_recognition1`](images/watson_visual_recognition1.png)

Type a unique service name then click **Create**.

![`watson_visual_recognition2`](images/watson_visual_recognition2.png)

After creating the service, **save the credentials and keep them safe**.

![`watson_visual_recognition5`](images/watson_visual_recognition5.png)


 
### Create the flow. 


Copy the code form the [visual recognition flow](visual_recognition_flow.json) and import it into _IBM Cloud Node-RED_ clipboard:



![`Import_flow`](images/Import_flow.png)


Your flow should look like the following figure. 


![`watson_visual_recognition3`](images/watson_visual_recognition3.png)

### Configure IBM Watson Visual Recognition on Node-RED

Double click on the visual recognition node then fill the following; API Key, Service Endpoint, and choose Classify an image on Detect. 

Finally, click on Deploy button in the upper right.

To see your application, go to ```[yourdomain] /upload ```

![`watson_visual_recognition6`](images/watson_visual_recognition6.png)

**_Congratulations!! You've successfully integrated a watson service using Node-RED_**

