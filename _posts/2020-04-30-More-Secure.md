---
layout: post
title: More Secure
subtitle: Create the Wiki
---

I have created a Wiki page that include some useful info

# Wiki page

## Analysis impact for each server and project

### Server 

phpMyAdmin
All our application's data stored there, such as:


Room sensor: We use MQTT subscription for this app so no ingest files involved.  Credentials involving this project is in secrets.py file for TTN subscription keys, which will need to be updated once a semester.  To update TTN Access key, visit https://console.thethings.meshed.com.au/applications/op_roomsensors and re-generate Access Keys and replace new key in TTN_PASSWORD under op_roomsensors application.


Orokonui: sensitive information is in .env file and secrets.py.  Updating phpMyAdmin password will require an update of .env file for DB access.


Co2: co2 application is currently not deployed in terms of web application.


Noise


Ice stadium


Kate account: Kate IoT account is where our ingest files are sitting.  Updating phpMyAdmin password will require WINSCP to our kate account to update our connect.inc.php file with the updated DB information so TTN can send data to our DB server.



The impact is high , every time changed the password for the database we also need to reconfigure for each application



IoT Kate Account
connect.int.php. This is our ingest file. it link TTN and database together

The impact is  moderate , It will affect all running application required to transfer data to the database


Kate account: Kate IoT account is where our ingest files are sitting.  Updating phpMyAdmin password will require WINSCP to our kate account to update our connect.inc.php file with the updated DB information so TTN can send data to our DB server.



The Things Network
We use this site to register a new device then get the keys(etc. network, app, device) and config the payload to transfer data to the database.

The impact is low , the ingest file in our kata server rather than here.



Docker
We published some docker files in Docker Hub.

The impact is low , only when people need to publish new docker file we need to log in there

### Application

Room Sensors Web App
Access the site we do not need to log in.

The impact is low, the purpose of logging into the site is only when we need to add a new device.

Room sensor: We use MQTT subscription for this app so no ingest files involved. Credentials involving this project is in secrets.py file for TTN subscription keys, which will need to be updated once a semester. To update TTN Access key, visit https://console.thethings.meshed.com.au/applications/op_roomsensors and re-generate Access Keys and replace new key in TTN_PASSWORD under op_roomsensors application.


Orokonui Web App
We going to change new application

Orokonui: sensitive information is in .env file and secrets.py.  Updating phpMyAdmin password will require an update of .env file for DB access.

### Gateway

Orokonui Gateway (TTN)
To access our gateway, once the gateway setup, we didn't reconfigure it again very often.

The impact is low



RAK Gateways
To access our RAK, once the RAK setup, we didn't reconfigure it again very often.

The impact is low

