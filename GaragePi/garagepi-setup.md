# Install/Configure Raspberry Pi for GaragePi

## Install and configure Raspberry Pi OS Lite

1. Download and install Imager from [raspberrypi.org](https://www.raspberrypi.com/software).
2. Insert the SD card you want to use for your GaragePi into your computer
  - 8GB or 16GB should be plenty big enough for this.
3. Once Imager is installed, launch it.
  - Note: I am doing this on Ubuntu, but it should be similar on MacOS and Windows
  - ![Imager](./images/Imager.png)
4. Click the **CHOOSE OS** button
  - ![GaragePi1](./images/GaragePi1.png)
5. Click the **Raspberry Pi OS (other)** option in the list
  - ![GaragePi2](./images/GaragePi2.png)
6. Click the **Rasberry Pi OS Lite (32-bit)** option in the list
  - ![GaragePi2a](./images/GaragePi2a.png)
7. Click the **CHOOSE STORA...** button
  - ![GaragePi3](./images/GaragePi3.png)
8. Click the SD card you inserted in step 2
  - ![GaragePi4](./images/GaragePi4.png)
9. Click the **Gear Cog** button
  - ![GaragePi5](./images/GaragePi5.png)
10. Fill out the items in the following images to fit your environment and then click the **SAVE** button.
  - It is important to set all of this up now as it will make it where you don't need to change the configuration once you put it into your RPi.  Make sure you enable SSH, set a username and password, and make note of the username and password as you will need that to SSH into the device.
  - ![GaragePi6](./images/GaragePi6.png)
  - ![GaragePi7](./images/GaragePi7.png)
  - ![GaragePi8](./images/GaragePi8.png)
  - ![GaragePi9](./images/GaragePi9.png)
11. Click the **WRITE** button
  - ![GaragePi10](./images/GaragePi10.png)
12. Click the **YES** button to confirm you want to continue and erase anything that may exist on the SD card
  - ![GaragePi11](./images/GaragePi11.png)
13. It will take a few minutes for the process to complete.
  - ![GaragePi12](./images/GaragePi12.png)
14. Once it has completed, remove the SD card from your computer and click the **CONTINUE** button
  - ![GaragePi13](./images/GaragePi13.png)
15. Close out of Imager on your computer
16. Put the SD card into your RPi

## Setting up MQTT on the GaragePi

