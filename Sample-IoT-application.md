# Send email alerts from an IoT Device and display the data collected in real-time using Node Red.
----------------------------------------------------------------------------------------------------

### Create your Application on IBM Cloud

1. Create an account or Log in to IBM Cloud [Click Here](ibm.biz/home-automation-workshop).

2. Click on Catalog > Boilerplates > Internet of Things Platform Starter.

![1](https://user-images.githubusercontent.com/36006325/41722508-d6156ecc-7579-11e8-98f0-b399b3b9fbb9.png)

3. Enter a name for your application. Name must be unique. Then, click Create.

![2](https://user-images.githubusercontent.com/36006325/41722563-fea70a4e-7579-11e8-85ab-461f60a198af.png)

4. When your app is running, select the app URL or type it into the browser to open the Node-RED flow editor

![4](https://user-images.githubusercontent.com/36006325/41722643-2f775700-757a-11e8-9093-5e5d935a4d03.png)

You should see Flow 1 running on IBM Cloud with a virtual thermometer. For now, you’ll work with the flow in the red square as shown below:

![5](https://user-images.githubusercontent.com/36006325/41722728-62b73de2-757a-11e8-96d4-30735890518f.png)

### Connect Virtual sensor to your Application

1. After you start your Internet of Things Platform Starter instance, click the following link to connect a temperature simulator to the IBM IoT app In node as shown in blue in Flow 1: http://ibm.biz/iotsensor

![6](https://user-images.githubusercontent.com/36006325/41722880-bf506506-757a-11e8-9498-6dbb0ea4e139.png)

2. Copy the value in the upper-right corner of the virtual thermometer. In the image above, the value is 03075c7af9d9.

3. In the flow editor, double-click the IBM IoT App In node.

![7](https://user-images.githubusercontent.com/36006325/41722940-e8979a10-757a-11e8-8e47-7f8b47cfda17.png)

4. Paste the ID of the sensor into Device Id field. Click Done and then deploy the flow.

![8](https://user-images.githubusercontent.com/36006325/41723004-1060550a-757b-11e8-91b7-f3517a81b036.png)

5. Go to the virtual sensor and increase the temperature to 41° C or more.
In the flow editor, note that the flow has three green output debug nodes that show flow data in the debug pane.

6. Disconnect the top green Debug output payload node in the top flow by clicking the connecting line and pressing Delete on your keyboard. Disconnect the device data node on the bottom flow as shown in the following image. Then, click Deploy.

You might need to scroll down in the debug pane to see the simplified view of temperatures.

![9](https://user-images.githubusercontent.com/36006325/41723228-91197186-757b-11e8-987c-f2c08365f4ba.png)

### Add Email notifications to your flow

You’ll need an Email account.

1. In the flow editor under social, drag a email out node onto the canvas under the cpu status node so that you can notify others when the CPU temperature exceeds 40° Celsius.

2. Click the connecting port of the danger node on the right and connect it to the Email (email out) node.

3. Double-click the Email node to edit its information.

4. Click the pencil icon to edit and associate the Email node with the Email account of your choice.

5. Click Done and then deploy the Node-RED flow.
Whenever the temperature exceeds 40° Celsius, an email is sent. 

### Display data collected in real-time

1. Click on the hamburger menu on the top right corner

2. Click on Manage Palette

3. Click on the install tab

4. Search for 'node-red-dashboard'

5. Click on Install

6. In the flow editor under dashboard, drag the chart node onto the canvas above the temp node so that you can display the temperature data as it is collected.

7. Click the connecting port of the temp node on the right and connect it to the chart node.

8. Double-click the chart node to edit its information.

9. Once all the information has been entered, click on Deploy.

10. Next click on the dashboard tab on the right pane and click on the link-out icon which will direct you to the Node-Red Dashboard consisting of the chart displayed.

As the temperature of the sensor changes, you can see the changes reflect on the chart.

----------------------------------------------------------------------------------------------------------------------------------------------------
