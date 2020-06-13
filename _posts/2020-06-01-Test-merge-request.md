---
layout: post
title: Test RoomSensor Merge Request two
subtitle: Testing in local machine for Bex
---

## Purpose

This is the related [ticket](https://gitlab.com/iotop/room-sensors/-/merge_requests/18)



Bex going to merge it to dev branch, so I tested it on my machine.

the main different is:

- when time packet was sent and displays on front end, solving the issue of incorrect dates & times being shown.

## How

#### Set up virtual environment for your project

Django environment using Anaconda Navigator, download Anaconda and run it.

##### Installing project

- CD into the "webapplication" directory (e.g "Documents\IOT\room-sensors\webapplication").  Run "pip install -r requirements.txt"

- Run "python manage.py migrate" to initially set up the database

![test4](https://raw.githubusercontent.com/jiqi963/project/master/img/test4.png)

##### SQLite3 in Deployment

Download a SQL file (Bex sent this to me) and put it under ` /webapplication/` 

It is important to preload database with all existed devices that will send data to our server or "Sensor query not found" error will appear and data will not be saved in the database, which will fail to display on React. 

##### Change utils.py

`
export const sensorsLink = 'http://localhost:8000/api/sensors/';

export const credsLink = 'http://localhost:8000/api-auth/';

//export const sensorsLink = 'http://10.25.100.164:80/api/sensors/';

//export const credsLink = 'http://10.25.100.164:80/api-auth/';
`

Keypoints is Uncomment the local API host.

## Result

when all things set up, run the commands.

`
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
`

After I test, all function work well and I approved it.

![test](https://raw.githubusercontent.com/jiqi963/project/master/img/test2.png)
