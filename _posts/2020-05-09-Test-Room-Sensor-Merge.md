---
layout: post
title: Test RoomSensor Merge Request
subtitle: Testing in local machine for Bee
---

## Purpose
This is the related [ticket](https://gitlab.com/iotop/orokonui/-/merge_requests/5)

Bee going to merge it to master branch, so I tested it on my machine.

the main different is:

- Removed secret key in settings.py, settingproduction.py.
- Created secrets.py to store SECRET_KEY
- Added .secrets.py in gitignore file
- Updated README.md

## How

I have tested a merge request before, the step almost same, however, this time have a secrets.py file to store the credentials for safety reason.

the file that secrets.py stored in our sensitive repository, you can grep it from [HERE](https://gitlab.com/iotop/sensitive/-/tree/master/Orokonui).

An important thing is after the test the functionality, need to delete the secrets file then merge to master branch, that the reason we separate the credential with the web app.

## Result

After I test, all function work well and I approved it.

![test](https://raw.githubusercontent.com/jiqi963/project/master/img/test.png)
