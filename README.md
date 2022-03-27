1. This webpage has textboxes for inputting the host and port. (requirement 1)

2. There is an "Start" button whenever the user presses that button the "disabled" attribute of the above textboxes will set to true that will remain till the users press the "End" button. On "Start" button press the connection establishment process will be started and the user will be notified when it is connected to the broker. (requirement 2)


3. There is a "disconnected" flag that identifies whether disconnection is because of the user's choice or the connection broke. In case it is the latter it reconnects to the broker with setting the timeout. (requirement 3)

4. There is a textbox and button to send lat, lng and temperature to the subscribed topic and the text will be parsed and sent in geojson format. (requirement 4)

5. There is a textbox and button to subscribe to a topic. (requirement 5)

6. "Share my status" button, as you can see in the video when the it pressed in android, shares the user's current location as well as a randomly generated value for temperature between -40 and 60. The message will be parsed and sent in geojson format. (requirement 5)

7. The map on the bottom of the page will show the location through a pin point that will be red in case the temperature is [30,60], green for [10,30), blue when [-40,10) and black otherwise. A popup will be shown in case the user clicks on the pinpoint and says 'The temperature in this location: X' the X will be the value of temperature sent by the users' client. (requirement 6)

8. In the video the received message from the client is visible in the MQTTX application. (requirement 7)

9. The android emulator in the video show how it get the location and re random number for the temperature and send it to the broker to be show in the subscribed browsers as well as the MQTTX application. (requirement 8)
