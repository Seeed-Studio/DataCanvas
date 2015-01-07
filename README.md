# Sense Your City - Seeeduino Setup Instructions

##### Open the package, lay out all the items on the table in front of you. 

You should have the following:

* 1 [Seeeduino](http://www.seeedstudio.com/wiki/Seeeduino_v3.0)

* 1 [Grove Base-Shield](http://www.seeedstudio.com/wiki/Grove_-_Base_Shield_V1.3)

* 6 Grove Sensors (and cables):

    * [Digital Light Sensor ](http://www.seeedstudio.com/wiki/Grove_-_Light_Sensor)

    * [Sound Sensor](http://www.seeedstudio.com/wiki/index.php?title=Twig_-_Sound_Sensor) 

    * [Temperature & Humidity](http://www.seeedstudio.com/wiki/Grove_-_Temperature_and_Humidity_Sensor_Pro) 

    * [Air Quality Sensor](http://www.seeedstudio.com/wiki/Grove_-_Air_Quality_Sensor)

    * [UV Sensor](http://www.seeedstudio.com/wiki/Grove_-_UV_Sensor) 

    * [Dust Sensor  ](http://www.seeedstudio.com/wiki/Grove_-_Dust_sensor)

* 1 Plastic Housing

* 1 Micro USB Cable

##### Plug the Grove Base Shield into the Seeeduino.

The black colored base shield fits perfectly on top of the red Seeeduino. Make a circuit sandwich.

![image alt text](/images/image_0.jpg)

##### Find the switch on the Grove Base Shield and make sure it is switched to "5V" side.

This means that we will be powering all sensors with 5 Volts of electricity. 

##### Plug a cable into each of the Grove sensors.

The cable only fits one way so don’t force anything. The connectors on the cables fit the sockets on the sensors, so they should fit perfectly together. One thing to bear in mind is the colors of the wires correspond to the white writing on the sensor boards. The red wire is always connected to VCC - which supplies power, while the black wire is always connected to GND.

##### Once all the sensors are connected to cables, plug the other ends into the Grove Shield.

Each sensor has a specific, labelled port that we will plug it into. 

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


We have three different types of sensors. Some sensors are Analog, hence the "A" labeled ports.  Analog sensors output a voltage between 0V and 5V, and we use that output to deduce the physical input to the sensor. Some sensors are Digital, hence the “D” labelled ports. Digital sensors output data in 1’s and 0’s that computers can easily understand. Finally, some sensors communicate over I2C, which is another way that sensors can transduce physical information and communicate it to computers efficiently. For more on this topic, there are some [great resources](https://learn.sparkfun.com/tutorials/analog-vs-digital) all over the web. 

##### Plug the micro USB cable into the Seeeduino.

The small end of the USB cable goes into the red Seeeduino. Later on, we will plug the other end into our computer to program our node. Once our sensor is finished, we will plug the USB cable into an adapter and power outlet. 

 

# Install the sensor in the case

##### Once all of the electronic parts are connected, we are ready to install everything into the housing. 

For this part you might want to have some extra tools on hand. You don’t *need* any extra tools but I’m going to use some tape and velcro. The top of the housing has a tab with three small holes. The very bottom of the housing has two large holes. This case will protect our electronics from water and weather, but will also allow our sensors to measure the environment outside the case, through the two large holes on the bottom. 

*Note: To secure the sensors in place and affix them to the case, I used a bit of **[dual lock adhesiv*e](http://www.amazon.com/Clear-Dual-Lock-Velcro-Adhesive/dp/B00EEDWSC2)* to keep all the parts in place. You can also use velcro, or, if in a bind, electrical tape.*

![image alt text](/images/image_1.jpg)

##### First, put the Seeeduino inside of the box. 

The letters "A0...A1...A2....A3" on the black Grove Shield should be facing downwards towards the bottom of the case. 

##### Feed the micro USB cable through the left hole in the bottom of the case and plug it into the Seeeduino. 

##### Using adhesive (tape, velcro, dual-lock, etc), secure the Air Quality Sensor all the way on the left so it hovers just above the hole. 

Space is pretty limited in the case, so make sure the sensor is all the way to the left, the printed circuit board will be touching the plastic case.  

##### Secure the Temperature and Humidity Sensor next to the right of the Air Quality Sensor, in the middle of the case.

##### Secure the Dust Sensor on the right side of the case so it hovers over the right hole. 

Make sure the metallic part of the Dust Sensor is pointing towards the top of the case. 

##### Secure the Sound Sensor right above the Temperature and Humidity Sensor in the middle of the case. 

It should be facing upwards towards the top of the case (where the tab with three holes is located). Make sure you leave enough clearance so you can slide the back of the case on. You can see where it slides on, there is a small ridge. The white connector at the end of the jumper cable should be below the ridge where the case slides on. 

##### Feed the cables for the UV and Light sensors through the notches on the bottom of the case, and attach both sensors to the case so they are facing down. 

The sensors are shaped so can put them together like a puzzle, you can tape them together with a single piece of adhesive and attach them to the case. 

![image alt text](/images/image_2.jpg)

##### Run the antenna outside of the left hole on the bottom of the box, peel off the adhesive backing, and secure it to the case. 

The antenna is the green circuit board hanging freely from the Seeeduino. Once you attach it, your box will look like a smiling robot, how cute. 

##### Once all of the sensors are in place. Slide on the top of the case on. 

If the case does not slide on easily, you will need to tidy up your wires and make sure that the UV and Light sensors’ jumper cables fit in the notches. If the wires are a mess you can fold them and tape them together, or to parts of the case, so that it looks neater fits better. If you several pieces of colored tape to do this, it will be easier to identify which wire is which incase you need to troubleshoot. 

##### Use a wire tie, string, or tape to attach the USB cable to the middle tab at the top of the case.

The sensor will should be able to hang vertically from the USB cable. We don’t want it to turn upside down and expose the vulnerable sensors on the outside of the case to water or the elements, so make sure the USB cable is well secured between two of the holes. I also taped the cable to the back of the sensor as well.  

** **![image alt text](/images/image_3.jpg)

##### Add some pizzazz to your sensor by decorating the cover of your sensor node.

The cover is your own blank canvas, draw some futuristic abstract weather patterns, or merely right your name. Just make sure you add some pizzazz, everyone loves pizzazz. 

# Program the sensor node. 

##### Before getting started, download the code resources [here](https://github.com/taurindb/datacanvas/archive/master.zip). 

You will also need to acquire a private key from Localdata, which will be assigned to you individually. Each sensor has its own unique Public ID and Private Key so that we can identify all unique data streams, we will also incorporate GPS coordinates, to plot all the sensors on a map.  

![image alt text](/images/image_4.png)

##### Download and install Arduino 1.5.8 software from [http://arduino.cc/en/Main/Software](http://arduino.cc/en/Main/Software).

Windows has an easy installer. For the Mac OS X version, drag the app to your applications folder, I had most success with the Mac OS X Zip file for Java 6, Arduino prompted me to install a version of Java 6 - I did so and had no problems after doing so. 

 ![image alt text](/images/image_5.png)

##### Plug your sensor node into a computer with the USB cable.

The sensor needs two things: power and a connection to the internet. Make sure it is placed within range of your Wifi router (maybe 50 ft or so). The first time you turn it on you will configure it to connect to your own Wifi network. If you change the location of your sensor, or your Wifi network settings (such as your password), you will need to reset and reconfigure your Seeeduino. 

##### Connect to the Seeeduino.

After a few moments, check your wifi settings and look for an available network containing the word "Seeeduino" that’s your Seeeduino network, select it and connect to it. If you do not see any network named Seeeduino try one or all of the following: Unplug and replug your USB cable, wait a moment for the network to show up. Move closer to your wi-fi router. If after repeated tries you do not see any networks, you can plug an Ethernet cable into the Seeeduino and connect it to your wifi router, which will guarantee that your sensor is connected to your network. 

##### Log in to the Seeeduino, when prompted for a password enter "seeeduino."

In a web browser, go to the following address: [192.168.240.1](http://192.168.240.1). This is the default IP address of your Seeeduino, in the next step you will give it a name, which will allow you to connect to it by directing your web browser to your_name_here.local

  ![image alt text](/images/image_6.png)

….

##### Configure the Seeeduino to access your own wifi network.

Give your board a name, something catchy, anything that you will remember. Create a password that is at least 8 characters. Select your Wifi Network from the list of "Detected Wireless Networks," enter your Wifi network’s password. If you ever move your Seeeduino to another wifi network you will need to repeat this process, and change the Wireless Parameters accordingly. 

 ** **![image alt text](/images/image_7.png)

##### Click the "Configure and Restart" button

The Seeeduino will restart and log on to your wireless network. If you had to plug your sensor directly into a router with an Ethernet cable earlier, you should now be able to remove it. 

##### ![image alt text](/images/image_8.png)

##### Disconnect your computer from the Seeeduino wireless network and connect your computer to your usual wifi network. 

##### Once connected to your usual Wifi network, open a web browser and go to [192.168.240.1](http://192.168.240.1).

You should see the same Arduino Yun interface as before, this time on your own wifi network. This means your Seeeduino has properly connected to your wifi network. w00t! 

##### Open the sense_your_city.ino file. 

It should open in the Arduino IDE (Integrated Development Environment).

![image alt text](/images/image_9.png)

##### Add the libraries in your sense_your_city folder to your local Arduino Library.

You can do this two ways. The easiest way is to copy the two folders located in *sense_your_city/libraries* to your Arduino library folder. On OS X the local Arduino library is located at */Users/yourusername/Documents/Arduino/libraries. *

![image alt text](/images/image_10.png)

 

##### The standard way to add libraries is by using the "Add Library…" function found in the “Sketch” menu in the Arduino IDE.

Go to Sketch > Import Library… > Add Library…   ![image alt text](/images/image_11.png)

##### Add both of the folders included in the *sense_your_city/libraries* to you Arduino Library.

Select each folder individually and click "Choose."

![image alt text](/images/image_12.png)

If the library was added, the Arduino IDE will display that it was successful.

  ![image alt text](/images/image_13.png)

##### Confirm that your computer is configured for your board.

Go to Tools > Board > Arduino Yún 

![image alt text](/images/image_14.png)

 Next go to Tools >  Port > /dev/tty.usbmodem (Arduino Yún)

![image alt text](/images/image_15.png)

##### Make the necessary modifications to the sense_your_city.ino file.

First, copy your user ID and private key into the space provided. 

##### ![image alt text](/images/image_16.png)

##### Add your GPS Coordinates

Go to [mygeoposition.com](http://mygeoposition.com/) and enter the address where the sensornode will be installed. Click the "Calculate geodata" button. Click the “Copy (x,y)” button to copy your GPS coordinates to paste into the Arduino IDE. 

![image alt text](/images/image_17.png)

##### Reverse GPS Coordinates.

After pasting you coordinates, make sure to reverse them so longitude is first and latitude is second.

##### ![image alt text](/images/image_18.png)

##### Verify and upload the code.

Click the check button to verify that the code modifications you made are OK. Next, click the play button to upload your code to the Seeeduino Cloud.

![image alt text](/images/image_19.png)

##### Open the serial monitor, to make sure the connection is working. 

Goto Tools > Serial Monitor. If everything is working, you will see new window that contains incoming communication from the Seeeduino, including verification that you are uploading online. 

![image alt text](/images/image_20.png)

##### Check the server to verify that your code is uploading.  

In a web browser, go to the following address: [https://localdata-sensors.herokuapp.com/api/sources/USER_ID_GOES_HERE/entries?startIndex=0&count=1000 ](https://localdata-sensors.herokuapp.com/api/sources/USER_ID_GOES_HERE/entries?startIndex=0&count=100000)

Be sure to change USER_ID_GOES_HERE to the user ID you received. Press your browser’s reload button several times over the course of several minutes to make sure data is uploading online. Data should be uploading about every 30 seconds or so. If everything is working, do a super funky celebration dance.  

![image alt text](/images/image_21.png)

# Node Installation

After we have confirmed that our sensor is successfully uploading data to the web, we are ready to install it outside.

##### Unplug the Seeeduino’s USB cable from your computer and plug it into USB adapter that will plug into a power outlet.

You can use any standard USB port to supply your sensor with power, just make sure the Seeeduino is always powered. You can tell if the Seeeduino is powered by look into the holes on the bottom hole of your housing. You should see the tiny lights blinking.

##### Hang your sensor outside by the USB cord.

At Gray Area, I used a utility clip to secure the USB cord to a ledge outside. Perhaps the best way to hang your sensor is to secure the USB cord to an object inside your dwelling and hang the sensor out your window. At SEEED Studios, the sensor hung outside our office window, the USB cable was secured and clipped to a desk inside. There are many ingenious ways to make sure that your node does not fall down to the ground and cause a tragic accident.

![image alt text](/images/image_22.png)![image alt text](/images/image_23.png)

##### Once your sensor is installed, double check to make sure it is still uploading data online. 

Check the [Localdata link](https://localdata-sensors.herokuapp.com/api/sources/USER_ID_GOES_HERE/entries?startIndex=0&count=1000) to make sure data is still posting to our servers. If your sensor node is not uploading data, it is probably too far away from your wifi router. Try moving the sensor node closer to the router and turn the power off and on to reset it. 

##### (Funky) Victory Dance

If you have verified that your sensor is up and running, do a celebratory victory dance. Go to your kitchen and make yourself the most delicious sandwich you’ve eaten all day. You did my friend, you really did it. Now it’s time for us to make some use of this data - follow along with the project at DataCanvas.org to see how artists, developers, and enthusiasts are turning this environmental data into meaningful media. Be a part of the conversation at [https://www.facebook.com/groups/datacanvas/](https://www.facebook.com/groups/datacanvas/).

# Troubleshooting:

If you encounter any problems connecting your sensor to your wifi network: hold the button on the top left hand corner (opposite the ethernet port) of the Seeeduino to reset it to its factory settings. Consult the "Program Your Sensor" section on how to reconfigure your wifi settings. 

