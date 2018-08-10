# iOT-Project
Starting date - 22-07-18
Project Name - Smart ODC solution with proximity navigation
Beacon Notes :
Beacons : 
- Beacon is a small bluetooth radio transmitter.
- It repeatedly transmits a single signal that other devices can see.
- It broadcast a radio signal that is made up of a combination of letters and numbers
  numbers transmitted on a regular interval of approximately 1/10th of a second. 
- A Bluetooth-equipped device like a smartphone can see a beacon once it's in
  range.
- Beacons may include accelerometer, temperature sensors or unique add-ons but all of
  them have on thing in common - THEY TRANSMIT A SIGNAL.

wHAT SIGNAL CONSIST OF :
- It's not throwing just any old message into the air. It's tranmitting a unique
  ID number that tells a listening device which beacon it's next to.
- It's like a code name.

HOW CAN I INTERACT WITH BEACONS :
- All of the beacons will have certain IDs.
- These IDs will be registered in mobile app.
- that means smartphone app can immediately recognize that the upcoming ID 
  is important and that it's from that particular beacon.
- The ID, however has little meaning on its own; it's entirely up to an app or other
  program to recognize what it means.

HOW DO BEACONS CONNECT TO THE WEB:
-Bluetooth provide the infrastructure for the entire beacon ecosytem.
- Bluetooth is a standard for sending data over short distances, a wireless technology.

WHY DO WE SAY "BLE BEACONS":
-BLE : bluetooth low energy. It's power-efficient version of bluetooth.
-BLE's low energy needs are vital to beacons, as it allows them to run for
 years on tiny coin-cell batteries.

HOW DOES A BEACON COMMNUNICATE:
- The beacons sends out its ID numbers about ten times every second(sometimes
more, sometimes less, depending on its settings)
- A nearby Bluetoothe-enabled device, like your phone, picks up that signal.
- When a dedicated app recognize it, it links it to a action or piece of content
stored in the cloud and displays it to the user.
- You can “teach” your app how to react to a beacon signal by developing using third-party tools.

COULDN'T THE BEACON DATA JUST BE HARDCODED INTO THE APP? WHY GO THROUGH THE
CLOUD? IT SOUND SO UNNECESSAry :
 - Keeping content on the cloud makes your app light.
 - If beacon information changes You don't have to re-code your app.

Types of beacons :
- Ibeacons
  : beacon begins with introduction of ibeacon
 :transmit very small bits of data 
- Eddystone
 : in came in 2015 by google.

BEACONS SPECS :
Battery life - 18-24 months.
Supported format - eddystone/ibeacon
interval - how often can beacon transmit its message.
TX power - The transmission powerdescribe how far a beacon can transmit data
4 mtr to 50-90 mtr.
Packets : A beacon packet is the data it transmits. This just describe the kind of information it
is able to transmit.for example . iBeacon contains one packet while Eddystone
has three separate ones.
Sensors : Now, beacons are coming out with extra capabilities. They may include accelerometers, light or movement sensors.
NFC/RFID : Beacons are still very new. For some users, it’s highly important that legacy technologies (like NFC and RFID tags) and beacons work together
Price : Beacons can cost as little as $5. Will such a cheap beacon be worth it? Well, that really depends on what you want, but many users will find that ultra-cheap beacons simply don’t get the job done. Expect one ordinary beacon to run $15-25.


Beacons are already being used for:

Tracking: One of the beacons’ more practical use cases is something many of us would never have guessed. In manufacturing and transport, managers need to know exactly where goods are at any given time. By attaching beacons, they can always have that information. In fact, they can even see the information from previous days or weeks.
Navigation: Creating accurate “GPS for indoor navigation” is a popular beacon use case. What Google Maps does for the outdoors, beacons can do for the indoors. They can tell you where you are and where you’re going in a museum, festival, or train station.
Interaction: Beacons can make reactions automated and trigger events. When you enter a room, the projector starts. It sends notifications or acts as a loyalty card. If you make a purchase at your local cafe, beacons help the app register that you were there. On your tenth entry, you get a free latte—awesome!
Security: Whether it’s making sure patients don’t go in the wrong wing or alerting factory workers to dangerous changes, beacons can automatically send notifications (either to app users or property owners) about a safety issue. Beacons can also be paired with geofencing to add an extra layer to data security.
Analysis: Data is one of the biggest tools at a company’s disposal. Beacons help generate data on where customers are going or where common problems occur on an assembly line. The online platform can store information on which beacons are being triggered and how users are interacting with them.

Requirements : 
 - USB plugs

IDEA - Multilanguage support in app.
  - If your will keep on standing at a particular location for more than particular
 time we can show him other info.
 ---------------------------------------------------------------------------------------------------------------------------------------
 ADDIION ON - 10/8/2018
 TITLE : Skybeacon/Proximity app study
 HOW TO CONFIGURE BEACONS :
1 – Before configure you must provision it to set frame type, broadcast interval and power level.
2 – You must use software provided by your beacon manufacturer to do this.
3 – To advertise a data or URL attachment you can use Eddystone-UID or Eddystone-EID frame types.
	URL – Eddystone-UID
•	Lets you advertise a URL(http/https)
•	Designed to interact with physical web
•	They don’t support app intent or app install URLS
•	When using this frame you can register the beacon with google.
•	Nearby notifications and physical web require HTTPS URLS.
	Frame – Eddystone-EID
•	Lets you decide who can access your beacons
•	Access can be handled using encryption key.

4 – With E-UID or E-EID :
•	Associate one or more data or URL attachments with a beacon.
•	Remotely update beacons attachments.
•	Monitor beacon using beacons dashboard.
5 – Register your beacon using Beacon tools app.
•	To register the beacon – launch the app and select google developer project you want to use.
o	Position your device near the beacon, you will see list of beacons.
o	Select beacon you want to register and then tap register beacon.
o	The beacon should come in registered tab
6 – Add an attachment 
•	Use Google beacon dashboard (recommended) : 
•	Use beacon tools app
•	Use beacon proximity API.
USE GOOGLE BEACON DASHBOARD :



SKYLAB BEACONS :
VERSION – VG01
1.	Bluetooth chip -  nRF51822 Bluetooth chip
2.	Battery – CR2477 button battery
3.	VG01 internal PCB board has a burning port , a pair of UART serial port.
4.	Docs link - http://www.skylabmodule.com/beacon-virgo/
Features : 
1.	Low power consumption
2.	Small, lightweight
3.	Advertising range upto 70m
4.	RoHS compliance(lead free)
5.	FCC , CE compliance
Application
1.	Indoor positioning
2.	Information push
3.	Identification
4.	WeChat shake
MAPPING YOUR VENUE ON MAP : 
-	ESTIMOTE – guide for using and development - https://developer.estimote.com/indoor/map-your-location/
-	Quora link - https://www.quora.com/I-have-ordered-BLE-Bluetooth-beacons-with-Eddystone-for-Android-to-develop-an-indoor-navigation-application-What-should-I-do-next-Im-confused-on-how-to-make-a-map-for-my-library-and-how-to-integrate-it-with-beacons-Can-anyone-help-me-or-suggest-any-ideas
-	Positioning link - https://proximi.io/
-	
LINKS :
Battery : https://www.amazon.in/s/ref=nb_sb_noss?url=search-alias%3Daps&field-keywords=battery+cr2477&tag=yhooinkenshoo-21&ascsubtag=b2f2a42f-ea75-4744-807a-b523e21d0331
Beacon App link : https://community.estimote.com/hc/en-us/articles/210530428-Getting-started-with-Estimote-beacons-and-APIs









