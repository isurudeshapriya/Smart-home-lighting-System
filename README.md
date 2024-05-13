# Smart-home-lighting-System
#Problem Statement


#Our project is driven by a multi-faceted goal: to design and implement smart lighting system 
that are not only beneficial for the elderly and individuals facing health challenges but also 
cater to the fast-paced lives of busy individuals. These devices offer the unique advantage of 
controlling lights from anywhere, removing the need for physical presence within the house 
and enhancing convenience for all.
The first key objective is to improve the quality of life for the elderly and those dealing with 
illness. These individuals often face mobility issues and daily challenges that can affect their 
independence. By providing remote control over core household lights, our smart lighting 
system offer them an opportunity to maintain their comfort and freedom, regardless of their 
location. This results in a more comfortable and manageable life, reducing the need for 
constant supervision and assistance.
Furthermore, our project recognizes that busy individuals also stand to benefit greatly from 
this technology. In today's fast-paced world, time is a precious commodity, and convenience 
is paramount. Our smart lighting system allow busy individuals to control their home 
environment while on the go, making it easier to switch on and off lights. The system will 
automatically switch on the bulbs when someone enters the room. Moreover, switches can 
be on and off by voice commands.


#Solution and Design Details


Mobile Application: The focal point of our solution is an intuitively designed mobile 
application, acting as the primary control hub for users to manage and oversee their home 
environment remotely. The application offers a user-friendly interface, ensuring accessibility 
for diverse user groups, including the elderly, individuals with health concerns, and those 
leading busy lives. Users can remotely operate lights with this downloadable application, 
compatible with multiple devices. The application’s flexibility allows customization to suit 
individual user preferences. Additionally, integration with the Node-Red platform expands the 
user interface options, enabling further customization and control.


Scheduling: The smart lighting system is seamlessly integrated with Alexa, facilitating 
effortless pre-setting of lighting preferences. Users can customize lighting conditions for 
different periods throughout the day or night, enabling adjustments to ambiance, brightness, 
and color temperature according to individual preferences. This feature is particularly 
beneficial for individuals requiring a consistent and adaptable environment, such as the 
elderly or those with health challenges. Simultaneously, for busy individuals, the system 
simplifies daily routines by automating and adjusting lighting settings through voice 
commands to Alexa-enabled devices.


Sensing (Lighting Control, Alexa Integration): The smart lighting system utilizes sensors 
to detect ambient light levels and harmoniously integrates with Alexa-enabled devices. 
These sensors enable the system to regulate lighting based on real-time data and user 
preferences. Users have the convenience of adjusting brightness, and scheduling using 
voice commands through Alexa, delivering a personalized and convenient lighting 
experience.


Power Unit: This essential component requires power to drive the ESP32 board and other 
indicators. While it can be configured to function with battery power, owing to its direct 
connection to AC current, a rectification circuit is employed to obtain the necessary 5V 
voltage. The circuit reduces the initial 230V AC voltage to 10V and then utilizes a 7805-
voltage regulator to stabilize the output at 5V, ensuring the proper functioning of the device.
Main Unit: This unit serves as the nerve center of the system, receiving and processing data 
transmitted from the mobile application via Wi-Fi. MQTT protocol is used for data 
transmission, with information published and subscribed to in JSON format. The ESP32, 
programmed in C++, manages the temperature sensor and various relays, including devices 
like the Adjustable Delay Timer Switch 5-30V MicroUSB Power. The relays facilitate the 
control of electrical equipment by using a small DC voltage, ensuring efficient and precise 
management
