# Create switches and sensors in Home Assistant

When the MQTT client on the GaragePi connects to Home Assistant, switches and sensors will be automatically added in entities.  However, adding them manually will allow better control.

1. You need to modify the **/config/configuration.yaml** file on the Home Assistant machine.  To do this, you need to use an Add-on in Home Assistant. There is more than one way to do that, but I used the Studio Code Server (VS Code) add-on since I am familiar with VS Code.  
    ![HA_Switches](Home_Assistant/images/HA_Switches.png)
2. Go into Studio Code Server and open the **/config/configuration.yaml** file and add the following to the end:

    ``` ansible
    #MQTT Switches 
    #Default payload types are used 
    mqtt:
      switch:
        - state_topic: "home/garage/output/switch23"
          command_topic: "home/garage/output/switch23/set_on_ms"
          availability_topic: "home/garage/status"
          name: "Garage Door F150"
          state_on: "ON"
          state_off: "OFF"
          payload_on: 500
          payload_off: OFF
          optimistic: false
          qos: 0
          retain: false
        - state_topic: "home/garage/output/switch24"
          command_topic: "home/garage/output/switch24/set_on_ms"
          availability_topic: "home/garage/status"
          name: "Garage Door F150 Light"
          state_on: "ON"
          state_off: "OFF"
          payload_on: 500
          payload_off: OFF
          optimistic: false
          qos: 0
          retain: false
        - state_topic: "home/garage/output/switch25"
          command_topic: "home/garage/output/switch25/set_on_ms"
          availability_topic: "home/garage/status"
          name: "Garage Door Fusion"
          state_on: "ON"
          state_off: "OFF"
          payload_on: 500
          payload_off: OFF
          optimistic: false
          qos: 0
          retain: false
        - state_topic: "home/garage/output/switch26"
          command_topic: "home/garage/output/switch26/set_on_ms"
          availability_topic: "home/garage/status"
          name: "Garage Door Fusion Light"
          state_on: "ON"
          state_off: "OFF"
          payload_on: 500
          payload_off: OFF
          optimistic: false
          qos: 0
          retain: false
      binary_sensor:
        - name: "Garage Door Fusion"
          state_topic: "home/garage/input/sensor21"
          payload_on: "ON"
          payload_off: "OFF"
          availability_topic: "home/garage/status"
          payload_available: "online"
          payload_not_available: "offline"
          qos: 0
          device_class: garage_door
          force_update: true
        - name: "Garage Door F150"
          state_topic: "home/garage/input/sensor17"
          payload_on: "ON"
          payload_off: "OFF"
          availability_topic: "home/garage/status"
          payload_available: "online"
          payload_not_available: "offline"
          qos: 0
          device_class: garage_door
          force_update: true
          ````

Once this is completed, you can go and add a Dasboard under "Overview" and set it up as you would like.  
![HA_Switches2](Home_Assistant/images/HA_Switches2.png)
