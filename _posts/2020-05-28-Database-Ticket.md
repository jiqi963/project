---
layout: post
title: Database Ticket
subtitle: Done security ticket
---

I have done two ticket [IoT Kate](https://gitlab.com/iotop/sensitive/-/issues/8) and [Database](https://gitlab.com/iotop/sensitive/-/issues/7).

kate server is easy, mention the team channel meantime update the related file(connect.php).

but Database one is a bit confusing, we can't change the password on GUI page direct. instead, to use Staging server, you can find login info on sensitive repo.

## The main step is:


#### Using .ppk to connect to staging server


* Download the private key from [HERE](https://gitlab.com/iotop/sensitive/-/blob/master/staging-ssh-rsa.ppk)
* Open Putty and go to Connection > SSH > Auth and upload ppk file.
* Go back to session & enter these credentials: hostname/ip: 10.118.24.32 port:3000
* Load session, click 'yes' if prompted by a dialogue box
* Enter 'user' when prompted for username


#### Updating phpMyAdmin Password


- Log into DB server with Using .ppk to connect to staging server instruction.
- Once logged in as user, use ``` mysql -u duniot -p ``` command to login as duniot user.  Copy from sensitive repository and paste current password when prompted.
- Once logged in to MariaDB > mysql will appear, use command show databases to list all databases and use mysql to select mysql table.
- Use select * from user; to display all available users.
- To change password to user, UPDATE mysql.user SET ``` Password=PASSWORD('newpassword') WHERE USER='duniot' ```
- Make sure to tell server to there is a change in mysql table by flush privileges before logging out of DB server.


## Overview


I organized Bee and Bex to help me change my password. This one's quite harder than we thinking, even we have a dinner break, it still takes a long time to fix it. Whatever we have learned how to do it.

![db1](https://raw.githubusercontent.com/jiqi963/project/master/img/db1.png)
![db2](https://raw.githubusercontent.com/jiqi963/project/master/img/db2.png)
