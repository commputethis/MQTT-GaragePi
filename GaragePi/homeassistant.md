# Setup Home Assistant

## Install Home Assistant on Raspberry Pi

1. Download and install ["Imager"](https://www.raspberrypi.com/software/) from raspberrypi.com on your computer.
  - I am using a computer running Ubuntu, but it should be similar on MacOS and Windows.
2. Insert your SD card into your computer
  - You may need an adaptor to do this.
3. Open Imager
  - ![Imager](./images/Imager.png)
4. Click the **CHOOSE OS** button
  - ![ChooseOSButton](./images/Imager1.png)
5. Click the **Other specific-purpose OS** option in the list (may need to scroll down to find it)
  - ![ChooseOS](./images/Imager2.png)
6. Click the **Home assistants and home automation** option in the list
  - ![HomeAssistants](./images/Imager3.png)
7. Click the **Home Assistant** option in the list
  - ![HomeAssistant](./images/Imager4.png)
8. Click the **Home Assistant OS** option for the type of Raspberry Pi you are using (I chose the RPi 4/400 option)
  - ![HomeAssistantVersion](./images/Imager5.png)
9. Click the **Internal SD card reader** option in the list (this would be selecting your SD Card to install Home Assistant on to)
  - ![Storage](./images/Imager6.png)
10. Click the **WRITE** button to start writing Home Assistant to your SD card
  - ![WriteButton](./images/Imager7.png)
11. Click the **YES** button to confirm
  - ![Confirm](./images/Imager8.png)
12. This takes a couple minutes depending on your computer.
  - ![Progress](./images/Imager9.png)
13. When it is completed, remove the SD card from the computer and click **CONTINUE**
  - ![Completed](./images/Imager10.png)

## Initial Home Assistant Configuration

1. Place the SD card into your RPi
2. Plugin the RPi to power it on
3. I connected a monitor and network cable to my RPi so I could see what IP address it got so I can configure it from a browser.  The IP address you need will be in the field listed as **IPv4 addresses for eth0** or something similar.  In my case, the IP is shown as 192.168.1.95/24, but we will ignore the /24 and just use 192.168.1.95.
4. Now go to a computer on the same network and open a browser (Chrome, Firefox, MS Edge, etc.)
5. In the Address bar, type **http://192.168.1.95:8123**
  - Note: do not put https, but rather http only
  - The **:8123** at the end signifies the port number we are connecting to.  Without that port listed, you would not be able to access the Home Assistant website.
6. 
