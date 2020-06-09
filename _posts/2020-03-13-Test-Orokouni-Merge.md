---
layout: post
title: Test Orokouni Merge Request
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
To run a local version of the app, can set up a local environment with Anaconda Navigator.

Once you've downloaded and installed Anaconda Navigator, Open it up and go to the Environments Tab

[ana1](https://raw.githubusercontent.com/jiqi963/project/master/img/ana1.png)