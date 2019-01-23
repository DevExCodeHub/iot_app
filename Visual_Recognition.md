# Analyze pictures using IBM watson and Node Red.
----------------------------------------------------------------------------------------------------

## Overview
Analyzing pictures became easier recently by using IBM Watson Visual Recognition service. The service will analyze a picture and give you all objects inside the picture with the percentage of accuracy. This project is a sample of visual recognition web app to analyze pictures and detect objects. 

## Learning Objectives
After completing this project, you will understand how to;
- [Create IBM Node-RED](#Create-IBM-Node-RED)
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


### Create IBM Node-RED
To create and configur Node-RED app, go to your IBM Cloud account and click Catalog then choice Starter Kits from the lift side then choice Node-RED Starter as shown in the following figure.

![`Create_node_red`](images/Create_node_red.png)



After that, Fill-out the fields to create IoT Platform:
- App name: has to be unique in the IBM cloud domain.
- Host name: will be filled out automatically based on the App name.

click on Create 
![`Translator`](images/4.png)

Then, wait seconds until shows the application shows Running and click on Visit App URL

![`Translator`](images/5.png)

After that, for first time, it will ask you to setup the username and password. Please follow the instruction to secure your editor so only authorized users can access it. 

<img src="images/6.png" width="50%" height="40%" >

Then, click on "Go to your Node-RED flow editor".

![`Translator`](images/7.png)

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

