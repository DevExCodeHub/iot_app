# Check your heart pulse & body temperature and send an alerts when it goes danger from an IoT Device and display the data collected in real-time using Node Red.
----------------------------------------------------------------------------------------------------


## Overview
Checking your heart pulse & body temperature is important. This application will semulate these prosess and show you how important and easy to do it by using Node-RED.

## Learning Objectives
After completing this project, you will understand how to;
- Use Node-RED.
- [Create Node-red](#Create-Node-red)
- [Create the flow](#Create-the-flow)
- [Add Email notifications to your flow](#Add-Email-notifications-to-your-flow)

## Prerequisites
In order to complete this project, you will need the following prerequisites:
- [IBM Cloud](http://ibm.biz/iot-cloud-signup) account - sign up if you don't have an account yet.
- [Node-RED starter](https://console.bluemix.net/catalog/starters/node-red-starter)
- [IBM Watson Visual Recognition](https://console.bluemix.net/catalog/services/visual-recognition) service.


## Estimated Time
- Creating and configure your Node-RED application on IBM Cloud should take less than 10 minutes.
- Developing the complete application on Node-RED should take a maximum 5 minutes.
- Overall the time for completing this project should take approximately 15 minutes.




### Create Node-RED
To create and configur Node-RED app, go to your IBM Cloud account and click Catalog then choice Starter Kits from the lift side then choice Node-RED Starter as shown in the following figure.

![`Create_node_red`](images/Create_node_red.png)



After that, Fill-out the fields to create IoT Platform:
- App name: has to be unique in the IBM cloud domain.
- Host name: will be filled out automatically based on the App name.

click on Create 
![`4`](images/4.png)

Then, wait seconds until shows the application shows Running and click on Visit App URL

![`5`](images/5.png)

After that, for first time, it will ask you to setup the username and password. Please follow the instruction to secure your editor so only authorized users can access it. 


![`6`](images/6.png)

Then, click on "Go to your Node-RED flow editor".

![`7`](images/7.png)


 
### Create the flow. 



Copy the code form the [check-up IoT application flow](check-up_IoT_application_flow.json) and import it into _IBM Cloud Node-RED_ clipboard:



![`Import_flow`](images/Import_flow.png)


Your flow should look like the following figure. 


![`check-up_flow`](images/check-up_flow.png)

In the first part of the flow. you will see node called 'Device payload' this node is used to simulate a data got from heart pulse sensor & body temperature sensor to your Application. 

And in the second part of this application, is to get these data and send an alart if something happened wrong. 



Finally, click on **Deploy** button in the upper right and click to 'Send Data' node to see the result. 




**_Congratulations!!_**




### Add Email notifications to your flow

You’ll need an Email account.

1. In the flow editor under social, drag a email out node onto the canvas under the cpu status node so that you can notify others when the CPU temperature exceeds 40° Celsius.

2. Click the connecting port of the danger node on the right and connect it to the Email (email out) node.

3. Double-click the Email node to edit its information.

4. Click the pencil icon to edit and associate the Email node with the Email account of your choice.

5. Click Done and then deploy the Node-RED flow.

Whenever there a danger situation, an email is sent. 



----------------------------------------------------------------------------------------------------------------------------------------------------
