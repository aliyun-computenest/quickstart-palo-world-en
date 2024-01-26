Palworld is a new survival game developed by Pocketpair. The game became extremely popular overnight, hitting 2 million concurrent players. However, Pocketpair's servers are struggling to keep up with the large number of players. To solve this issue, Pocketpair allows players to set up dedicated servers, which offers the following advantages:

(1) greater stability to reduce the risk of crashes or downtime;
(2) easy adjustment of the server player count to 4, 12, or 32 players; 
(3) control over server settings to allow for customization of gameplay elements, rules, and mods, creating a tailored experience for the gaming community.

This topic describes how to establish a dedicated server for Palworld in Alibaba Cloud with a few clicks. You only need to configure the settings on the page as prompted. Then, the system will automatically create an ECS instance, configure the port and firewall, and install the game environment. The whole process takes only 2 to 3 minutes with no coding involved.

# Create an ECS instance
## Step 1: Go to the Palworld multiplayer server introduction page
(1) Log on to the Alibaba Cloud International site (alibabacloud.com). 
(2) Visit the Palworld multiplayer server introduction page at https://developer.aliyun.com/topic/ecs/huanshou and click Deploy Now on the right side.
![image](https://yqintl.alicdn.com/013f2f1ff7f585aab3a9dcf94a657be1ffd65ffd.png)
Most required settings, including the network protocol and port (UDP protocol and port 8211), are pre-configured.
## Step 2: Configure the ECS instance
On the Create Service Instance page, configure the following parameters:
(1) **Service Instance Name**: Enter the instance name. We recommend that you use the default name.
(2) **Region**: Select the region where you want to deploy the ECS instance. We recommend that you use the default value, which is the city closest to you.
(3) **Pay Period Unit and Period**: Select a subscription duration for the ECS instance. We recommend that you specify three months as the subscription duration.
(4) **Select the ECS instance specifications**. Higher specifications result in a smoother gaming experience. Palworld is a memory-intensive game. We recommend that you specify 4vCPU 16GiB or higher specifications for your ECS instance. 4vCPU 16GiB is recommenced by Pocketpair, developer of the game. For more information, visit https://tech.palworldgame.com/dedicated-server-guide. We recommend that you set the **Internet Charge Type** parameter to **Pay-by-bandwidth**. The pay-by-bandwidth metering method does not impose limits on the bandwidth, which reduces latency and provides a better gaming experience.
![image](https://yqintl.alicdn.com/a63c0b2e6d6fd973a1c1a7a4cfb9c8777c60e21a.png)
(5) **Instance Password**: Enter a password for the ECS instance. The password is required when you log on to the ECS instance.
(6) **Availability Zone**: Select the zone in which the ECS instance resides. We recommend that you use the default zone.
After you complete the configurations, click Next: Confirm Order to submit the order.
## Step 3: Purchase the service
In the Terms of Service section, read and select the check box to agree to the terms of service and then click Create Now to complete the payment.
![image](https://yqintl.alicdn.com/34c26339a349a6a9014ebc0f2c69de214c83f440.png)
If the Submitted message appears, it indicates that the ECS instance was created successfully. You can click View Service to view the instance.
![image](https://yqintl.alicdn.com/224fa8750b59c5e3c959910c04cecd020bc7a1eb.png)
![image](https://yqintl.alicdn.com/68367bea7fcc29ee4a157baf50e47842c2161b09.png)
## Step 4: Obtain the IP address of the ECS instance
The ECS instance can be created in less than a minute. When the status of the instance changes to **Deployed**, click the ID of the instance to go to the instance details page.
In this step, the Palworld server installation program is preloaded in the image of the ECS instance that you created.
![image](https://yqintl.alicdn.com/b4ee975799d37bb962ea76883edccdfd04966a7f.png)
On the Overview tab, the IP address of the ECS instance is displayed in the Service Addresses field, which will be used for subsequent configuration
![image](https://yqintl.alicdn.com/3718beafdf8a5e9fa6ef6afa20cb2aec5b31e2e9.png)
# Start a multiplayer game
(1) Launch Palworld and select Join Multiplayer Game from the main menu.
![image](https://yqintl.alicdn.com/b9d4c06ec0f815e26b33c849086ba24654b75cf4.png)
Enter the IP address obtained in Sub-step 4 of Step 1 in the text box at the bottom of the page and click **Connect**.
![image](https://yqintl.alicdn.com/e0381ce945286da7507118997bf4c1abe395223f.png)
You are now ready to play!
![image](https://yqintl.alicdn.com/dde619ca572e82d11b10545c730139dd919a2c24.png)
An out-of-memory issue may occur during the running of the game. A quick solution to mitigate the impact of this issue is to regularly restart your server. We recommend that you create a scheduled task in the Alibaba Cloud Manage Console to automatically restart your ECS instance during off-peak hours.
