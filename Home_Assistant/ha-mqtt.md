# Install and configure MQTT on Home Assistant

## Setup MQTT

1. Click on **Settings** on the Side bar  
    ![HomeAssistantSettings](./images/HomeAssistant5.png)
2. Click on **Add-ons** in the list of options  
    ![HomeAssistantAdd-ons](./images/HomeAssistant6.png)
3. Click the **ADD-ON Store** button in the bottom right of the window  
    ![HomeAssistantAdd-OnsButton](./images/HomeAssistant7.png)
4. Click in the **Search** field and type **MQTT**
5. Click the **Mosquitto broker** option  
    ![HomeAssistantSearch](./images/HomeAssistant8.png)
6. Click the **INSTALL** link  
    ![HomeAssistantMQTTInstall](./images/HomeAssistant9.png)
7. Once it is finished, click the **START** link  
    ![HomeAssistantMQTTStart](./images/HomeAssistant10.png)
8. It only takes a short moment to start  
    ![HomeAssistantMQTTStarted](./images/HomeAssistant11.png)
9. Now we need to go and create the integration.  Click **Settings** on the Side bar  
    ![HomeAssistantSettings](./images/HomeAssistant5.png)
10. Click **Devices & Services** in the list of options  
    ![HomeAssistantDevices](./images/HomeAssistant12.png)
11. Click the **Configure** button on the "MQTT" integration
    - If the MQTT integration is not there, click the ADD INTEGRATION button in the bottom right, search for MQTT, and follow the prompts to add it  
    ![HomeAssistantMQTTConfigure](./images/HomeAssistant13.png)
12. Click the **SUBMIT** link on the MQTT Broker via Home Assistant add-on dialog  
    ![HomeAssistantMQTTadd-on](./images/HomeAssistant14.png)
13. Click the **FINISH** link on the Success dialog  
    ![HomeAssistantSuccess](./images/HomeAssistant15.png)
14. Click the **Configure** link on the Mosquitto broker integration  
    ![HomeAssistantMosquitto](./images/HomeAssistant16.png)
15. Click the **RE-CONFIGURE MQTT** link under MQTT settings
    - Though Home Assistant already configured MQTT for us, we do not know what the login information is that will need to be used by GaragePi when we set it up.  
    ![HomeAssistantBrokerOptions](./images/HomeAssistant17.png)
16. Click the **EYE** icon to reveal the Password  
    ![HomeAssistantBrokerOptions2](./images/HomeAssistant19.png)
17. Make a note of the Username and Password
    Username: "homeassistant" Password: "page2kaedaecaitei0ooqu8zeiph5jahf3Shee9aedieX2Oophae7rahtheighae" in my case  
    ![HomeAssistantBrokerOptions3](./images/HomeAssistant18.png)
18. Click the **NEXT** link  
19. Scroll down to the bottom of the MQTT Options dialog and click the **SUBMIT** link  
    ![HomeAssistantBrokerOptions3](./images/HomeAssistant20.png)
20. Click the **FINISH** link on the Success dialog  
    ![HomeAssistantSuccess2](./images/HomeAssistant21.png)

We are now done setting up MQTT in Home Assistant.  Move on to configuring the GaragePi
