# Analyze real-time images from your computer using Visual Recognition on Node-RED
----------------------------------------------------------------------------------------------------

## Overview
Analyzing pictures became easier recently by using IBM Watson Visual Recognition service. This application will take an image from your computer camera and analyze it to give you the gender of persons and their age with the percentage of accuracy.

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
- Developing the complete application on Node-RED should take a maximum 5 minutes.
- Overall the time for completing this project should take approximately 20 minutes.

### Create IBM Watson Visual Recognition

Open your IBM Cloud account then **click** on _Catalog_ --> _AI_ --> _Visual Recognition_ 
![`watson_visual_recognition1`](images/watson_visual_recognition1.png)

Type a unique service name then click **Create**.

![`watson_visual_recognition2`](images/watson_visual_recognition2.png)

After creating the service, **save the credentials and keep them safe**.

![`watson_visual_recognition5`](images/watson_visual_recognition5.png)


 
### Create the flow. 

If you don't have virtual-tjbot, base64,or DashBoard nodes, select manage palette from the top right menu.

![`Translator`](images/8.jpg)

#### install virtual-tjbot
At the manage palette menu click on the Install tab then search for ```node-red-contrib-virtual-tjbot``` and install it.


![`install_virtual-tjbot`](images/install_virtual-tjbot.png)


#### install dashboard
At the manage palette menu click on the Install tab then search for ```node-red-dashboard``` and install it.

![`node-red-dashboard`](images/install_dashboard.png)

#### install base64
At the manage palette menu click on the Install tab then search for ```node-red-node-base64``` and install it.

![`install_base64`](images/install_base64.png)


Then, close the palette menu.



Copy the code form the [real-time_analyze_image_flow](real-time_analyze_image_flow.json) and import it into _IBM Cloud Node-RED_ clipboard:



![`Import_flow`](images/Import_flow.png)


Your flow should look like the following figure. 


![`real-time_v`](images/real-time_v.png)

### Configure IBM Watson Visual Recognition on Node-RED

Double click on the visual recognition node then fill the following; API Key, Service Endpoint, and choose Classify an image on Detect. 

Finally, click on **Deploy** button in the upper right.

To see your application, go to ```[yourdomain] /ui ```

![`node-red_real-time_ui`](images/node-red_real-time_ui.png)

Click to take picture to start analyzing!!

**_Congratulations!! You've successfully create real-time images analyzing using Node-RED_**

