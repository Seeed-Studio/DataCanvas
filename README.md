![image alt text](/images/image_0.png)  
#Sense Your City Sensor Instructions 

##What’s in the box:

You should have the following:

* 1 [Seeeduino](http://www.seeedstudio.com/wiki/Seeeduino_v3.0)
* 1 [Grove Base-Shield](http://www.seeedstudio.com/wiki/Grove_-_Base_Shield_V1.3)
* 6 Grove Sensors (with jumper cables):
    * [Digital Light Sensor ](http://www.seeedstudio.com/wiki/Grove_-_Light_Sensor)
    * [Sound Sensor](http://www.seeedstudio.com/wiki/index.php?title=Twig_-_Sound_Sensor) 
    * [Temperature & Humidity](http://www.seeedstudio.com/wiki/Grove_-_Temperature_and_Humidity_Sensor_Pro) 
    * [Air Quality Sensor](http://www.seeedstudio.com/wiki/Grove_-_Air_Quality_Sensor)
    * [UV Sensor](http://www.seeedstudio.com/wiki/Grove_-_UV_Sensor) 
    * [Dust Sensor  ](http://www.seeedstudio.com/wiki/Grove_-_Dust_sensor)
* 1 Weather Resistant Sensor Housing 
* 1 Micro USB Cable           

![image alt text](/images/image_1.png)    

##I. Sensor Assembly   

1. Plug the Grove Base Shield into the Seeeduino. The black Grove base shield fits perfectly on top of the red Seeeduino. Do not too push too hard on the Grove base—even when it is plugged in completely there is some space between the two boards.

2. Find the switch on the Grove Base Shield and make sure it is switched to "5V." This indicates that we will be powering all sensors with five volts of electricity.

3. Plug a jumper cable into each of the Grove sensors.The cable only fits one way so don’t force anything.
      ![image alt text](/images/image_2.png)

4. Once all the sensors are connected to cables, plug the other ends into the Grove Shield. Each sensor has a specific, labelled port that we will plug it into. See the chart below for reference.   

6. We have three different types of sensors. Some sensors are Analog, hence the "A" labeled ports. Analog sensors output a voltage between 0V and 5V, and we use that output to deduce the physical input to the sensor. Some sensors of our sensors are Digital, hence the “D” labelled ports. Digital sensors output data in 1’s and 0’s that computers, such as our Seeeduino, can easily understand. Finally, some sensors communicate over I2C, which allows bidirectional communication between the sensor and the computer.

7. Plug the micro USB cable into the Seeeduino. The small end of the Micro USB cable goes into the red Seeeduino. Later on, we will plug the other end into our computer to program our Seeeduino.

<table>
  <tr>
    <td>Sensor</td>
    <td>Port</td>
  </tr>
  <tr>
    <td>Digital Light Sensor </td>
    <td>I2C</td>
  </tr>
  <tr>
    <td>Sound Sensor </td>
    <td>A0</td>
  </tr>
  <tr>
    <td>Temperature & Humidity Sensor</td>
    <td>D4</td>
  </tr>
  <tr>
    <td>Air Quality Sensor</td>
    <td>A1</td>
  </tr>
  <tr>
    <td>UV Sensor </td>
    <td>A2</td>
  </tr>
  <tr>
    <td>Dust Sensor </td>
    <td>D7</td>
  </tr>
</table> 

##II. Install the sensor in the case     
   ![image alt text](/images/image_3.png)

For this part, you might want to use some Velcro, 3M Dual Lock, or adhesive tape to keep your sensors in place. You don’t need any of these supplies, but they will make your housing more secure and neat. For your reference, the top of the plastic housing has a tab with three small holes, the bottom of the housing has two large holes. This housing will protect our electronics from water and weather, but will also allow our sensors to measure the environment outside the case, through the two large holes on the bottom.

1. Put the Seeeduino inside of the box. The letters "A0...A1...A2....A3" on the black Grove Shield should be facing downwards towards the bottom of the case. Feed the micro USB cable through the left hole in the bottom of the case and plug it into the Seeeduino.

2. Using adhesive (tape, velcro, Dual Lock, etc), secure the Air Quality Sensor all the way on the left so it hovers just above the hole. Space is pretty limited in the case, so make sure the sensor is all the way to the left, the printed circuit board will be touching the plastic case.

3. Secure the Temperature and Humidity Sensor to the right of the Air Quality Sensor, in the middle of the case.

4. Secure the Dust Sensor on the right side of the case so it hovers over the bottom right hole. Make sure the metallic part of the Dust Sensor is pointing towards the top of the case.

5. Secure the Sound Sensor right above the Temperature and Humidity Sensor in the middle of the case. It should be facing upwards towards the top of the case (where the tab with three holes is located). Take note of the small ridge that goes around the inside of the case, this is where the cover slides on. Make sure you leave enough clearance so you can slide the front cover of the case on. The white connector at the end of the jumper cable connected to the sound sensor should be below the ridge where the case slides on.

6. Feed the cables for the UV and Light sensors through the notches on the bottom of the case, and attach both sensors to the case so they are facing down. The circuit boards for these sensors are shaped so you can put them together like a puzzle. Connect the two sensors and attach them to the case.

7. Find the antenna—it’s the circuit board hanging freely from the Seeeduino, peel off the adhesive backing and attach it to the inside of the case. 

8. Once all of the sensors are in place, double check that all of the white connectors are securely plugged in. Slide on the front cover of the housing. If the case does not slide on easily, you will need to tidy up your wires. Make sure that the UV and Light sensors’ jumper cables fit in the notches on the bottom of the housing. If the wires inside the housing are a mess, you can fold them and tape them together, or to parts of the case, so that they look neater and fit better. If possible, use several different colors of tape to do this, so that it will be easier to identify which wire is which incase you need to troubleshoot. 
   
 ![image alt text](/images/image_4.png)

9. Use a wire tie, string, or tape to attach the USB cable to the middle tab at the top of the case. The sensor will should be able to hang vertically from the USB cable. We don’t want it to turn upside down and expose the vulnerable sensors on the outside of the case to water or harsh weather. Make sure the USB cable is well secured between two of the three holes. For extra precaution, you can tape the Micro USB cable to the back of the senso 

##III. Program the sensor node     
   ![image alt text](/images/image_5.png)

1. Before getting started, download the code resources at: [https://github.com/Seeed-Studio/DataCanvas/archive/master.zip](https://github.com/Seeed-Studio/DataCanvas/archive/master.zip)

2. Go to: [http://localdata.github.io/data-canvas-signup/get-started](http://localdata.github.io/data-canvas-signup/get-started) to register your sensor and acquire a private key from Localdata. Each sensor has its own unique Public ID and Private Key so that we can identify all unique data streams, we will also incorporate GPS coordinates, to plot all the sensors on a map.

3. Download and install the Arduino 1.5.8 IDE from http://arduino.cc/en/Main/Software. Windows has an easy installer. For Mac OS X, download the "Zip file for Java 6" version and drag the app to your applications folder. If you are prompted to install Java 6, follow the steps necessary to do so before continuing.

4. Plug your sensor node into a computer with the USB cable.

5. The Seeeduino Cloud needs two things: USB power (5V) and a wifi connection to the Internet. Make sure the Seeeduino is placed within range of your Wifi router (about 50 ft or so). The first time you plug in your Seeeduino, you will configure it to connect to your own Wifi network. If you change the location of your sensor, or your personal Wifi network settings, you will need to reset and reconfigure your Seeeduino.

6. After plugging in the Seeeduino, wait a moment and then check your wifi settings. Look for an available network nearby called something like "Seeeduino-XXXXXXXX" - that’s your Seeeduino’s private network, select it and connect to it.

7. Open a web browser and go to the following address: 192.168.240.1 — This is the default IP address of your Seeeduino, where you will always be able to find it (as long as you are on the same network). When prompted for a password enter "seeeduino" and click “Log In.”       

8. Give your board a catchy name, something that you will remember. Create a password that is at least eight characters. Select your Wifi network from the list of "Detected Wireless Networks," enter your Wifi network’s password.         

     `**Note**: If you move your Seeeduino to another wifi network or encounter problems connecting to wifi, you will need to reset the Seeeduino’s wifi processor. The reset button for WiFi is located on the top left corner of the Seeeduino, opposite the USB connector. You can reset the Seeeduino’s network configuration by pressing the Wifi reset button for longer longer than 5 seconds, but less than 30, which will reboot the AR9331 wifi processor.  Unplug and replug the Seeeduino to reset it. Wait a minute or more for the WiFi configuration to reset. The Seeeduino will once again start its own Wifi network "Seeeduino-XXXXXXXXXXXX." Check your computer’s wifi settings and log on to the Seeeduino’s network, go to 192.168.240.1 in a browser, and configure the Seeeduino with the new network settings. If after completing these steps you are still having trouble accessing the Seeeduino, you will want to do a factory reset. To reset the Seeeduino to its default state: hold the Wifi reset button for more than 30 seconds, unplug and replug the Seeeduino, and wait a minute for it to boot up. After a factory reset the computer will be completely wiped--you will need to reupload any arduino code and reconfigure all Wifi settings.`

9. Click the "Configure and Restart" button. The Seeeduino will restart and connect to your personal wireless network.         

10. Disconnect your computer from the "Seeeduino-XXXXXXXXXXXX" wireless network and connect your computer to your personal wireless network.

11. Once connected, direct your web browser to: yourseeduinoscatchyname.local. You should see the same Arduino interface as before, but this time on your own wireless network. You can also direct your browser to the Seeeduino’s default IP address: 192.168.240.1.

12. Locate the code resources you downloaded in Step 1 and open the sense_your_city.ino. It should open within the Arduino IDE.  
    ![image alt text](/images/image_6.png)

13. Add the libraries in your sense_your_city folder to your local Arduino Library. The easiest way to do this is to directly copy the two folders located in sense_your_city/libraries to your Arduino’s local library folder. On OS X the local Arduino library is located at /Users/yourusername/Documents/Arduino/libraries.  
    ![image alt text](/images/image_7.png)

14. The more common way to add libraries is to use the "Add Library..." function found in the “Sketch” menu in the Arduino IDE. Go to Sketch > Import Library... > Add Library... 
    ![image alt text](/images/image_8.png)

15. Individually add both of the libraries located in the sense_your_city folder by selecting each folder individually and clicking "Choose." Go to Sketch > Import Library... > Add Library... to ensure that the libraries have been added successfully. You will also see message in the black console at the bottom of the Arduino IDE indicating success or that an error has occurred.  
    ![image alt text](/images/image_9.png)

16. Confirm that the Arduino IDE is configured for your board. Go to Tools > Board > Arduino Yún.  
     ![image alt text](/images/image_10.png)   

17. Confirm the correct communication Port. Go to Tools > Port > /dev/tty.usbmodemXXXX (Arduino Yún). Now, your Arduino IDE is properly configured to program your Seeeduino.  
     ![image alt text](/images/image_11.png)

18. Make some necessary modifications to the sense_your_city.ino code. Insert the user ID and private key sent to you by Localdata in the space provided between the quotation marks at the top of the code.  
     ![image alt text](/images/image_12.png)

19. Calculate your sensor’s GPS location by going to mygeoposition.com and entering the address where your sensor is installed. Click the "Calculate geodata" button. Click the “Copy (x,y)” button to copy your GPS coordinates and paste them into the Arduino IDE.     
     ![image alt text](/images/image_13.png)

20. After pasting your coordinates, **make sure to reverse them so longitude is first and latitude is second.**  
     ![image alt text](/images/image_14.png)      

21. Click the check button at the top of the sense_your_city window to verify that the code modifications you made are OK. Next, click the play button to upload your code to the Seeeduino.  
     ![image alt text](/images/image_15.png)

22. Go to Tools > Serial Monitor to open the serial monitor and make sure that everything is working.... If it is, you will see new window that contains incoming communication from the Seeeduino, including verification that you are uploading online — "Posting Data!"  
     ![image alt text](/images/image_16.png)

23. Finally, check the Localdata site to verify that your code is uploading. In a web browser, go to the following address. 

[http://localdata-sensors.herokuapp.com/api/v1/sources/USER_ID_GOES_HERE/entries?startIndex=0&count=5&sort=desc](http://localdata-sensors.herokuapp.com/api/v1/sources/USER_ID_GOES_HERE/entries?startIndex=0&count=5&sort=desc)

Be sure to change YOUR_USER_ID_GOES_HERE to the user ID you received from Localdata. Press your browser’s reload button several times over the course of several minutes to make sure data is uploading online. Data should be uploading about every 30 seconds or so. If everything is working, do a super funky victory dance!                 

##IV. Node Installation
   ![image alt text](/images/image_17.png)

After we have confirmed that our sensor is successfully uploading data to the web, we are ready to install it outside. Place the sensor somewhere interesting - a busy street corner, near a public transit station, next to a public park, etc. Make sure the sensor is always safe from harsh weather conditions. If terrible weather is in the local forecast, it is probably a good idea to unplug or move your sensor somewhere safer. If you do decide to move your sensor, don’t forget to reconfigure the wireless settings and make sure to update your new GPS coordinates in the sense_your_city.ino Arduino code.

1. Unplug the Seeeduino’s USB cable from your computer and power the sensor from a power outlet. You can also use any standard USB port to supply your sensor with power, just make sure the Seeeduino is always powered and check on it from time to time. You can tell if the Seeeduino is powered by looking into the bottom holes of your housing. You should always see some LEDs blinking inside the case.

2. Install your sensor outside, hanging it from the USB cord. You may want to use a utility clip to secure the USB cord to a ledge, or perhaps the best way to hang your sensor is to secure the USB cord to an object inside your dwelling and hang the sensor out your window. At SEEED, the sensor hangs from an office window, the USB cable was secured and wrapped around a table leg inside. There are many ingenious methods to make sure that your node does not fall down to the ground and cause a tragic, tragic accident—choose one of them.  
     ![image alt text](/images/image_18.png)

3. Once your sensor is installed, double check to make sure it is still uploading data online. Go to the URL in Step 25 to make sure data is still posting to the Localdata servers. If your sensor is not uploading data, it is probably too far away from your wifi router. Try moving the sensor closer to the wireless router. Unplug the USB cable from the power outlet to reset the Seeeduino.

If you have verified that your sensor is up and running, do a celebratory victory dance, make it extra funky. Congratulations, you are now ready to Sense Your City!

Follow along with the project at DataCanvas.org to see how artists, developers, and enthusiasts are turning this environmental data into meaningful media. Be a part of the conversation, ask questions, and post photos at [https://www.facebook.com/groups/datacanvas/](https://www.facebook.com/groups/datacanvas/) and stay tuned!


Troubleshooting:          

If you have any questions or run into roadblocks, check the FAQ at [http://datacanvas.org/sense-your-city/ ](http://datacanvas.org/sense-your-city/)

You can also post questions in the Facebook group listed above.
