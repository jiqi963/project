---
layout: post
title: Test Orokouni Merge Request
subtitle: Testing in local machine
---

## Target
This is the related [ticket](https://gitlab.com/iotop/orokonui/-/merge_requests/4)

Bee going to merge it to master branch, so I tested it on my machine.

the main different is:

- Updated python data retrieval array instead of using nested array in the previous version.
- Status is updated according to the most updated data available in database.
- Refresh page every 20 seconds instead of 30 seconds.
- Renamed gates according to type of sensors used as well as location in order to avoid confusion between testing device and deployed device.

## How

### Running a Local Version of the App

To run a local version of the app, can set up a local environment with anaconda navigator.

Once you've downloaded and installed anaconda navigator, Open it up and go to the environments yab

![ana1](https://raw.githubusercontent.com/jiqi963/project/master/img/ana1.png)

### Creating a New Environment

Create a new environment for the web app by clicking the create button at the bottom of the page.

![ana2](https://raw.githubusercontent.com/jiqi963/project/master/img/ana2.png)

### Installing Dependencies

easy to run the command `pip install -r requirements.txt`, it can install all needed package and plugin.

Copy secrets.py file from Orokonui folder and place the file in Projectenv/Project/Project, it is a ingest file which can connect TTN and Database.

finally run command `command: python manageDevelopment.py runserver`

![ana3](https://raw.githubusercontent.com/jiqi963/project/master/img/ana3.png)

![ana4](https://raw.githubusercontent.com/jiqi963/project/master/img/ana4.png)

## Result

After I test, all function work well and I approved it.
