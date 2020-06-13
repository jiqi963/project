---
layout: post
title: Changed the Password For Database Again
---

## Ticket

[Ticket](https://gitlab.com/iotop/sensitive/-/issues/16) Database password exposed again, I have changed it.

## Different Situation

I have work with Bee and Bex to changed the password before, but it need access the OP network, not by Cixrix, it ask Microsoft Remote Desktop, because I need to import the private key to Putty.

But, my OP computer has down, I asked Rob which said have some system error and not easy to fix by the time.

Whatever，I need to change the password to keep our database safe. So I heve been to OP at the weekend to do that.

## How

After we work together Bee have written the step on the [Wiki page](https://gitlab.com/iotop/sensitive/-/wikis/Update%20Database%20Password)

- Using .ppk to connect to staging server
- Updating phpMyAdmin Password
- Affected files / servers

The first two steps same with last time, also I need to change affected file this time(Bex have done this last time)

- We have different `.env` files stored in Sensitive repository, such as Orokouni and room-sensor. 

- Kate server have a ingest file named `connect.int.php`, so TTN can send data to our DB server.

- Ice Rink ingest `connect.inc.php` on Sensitive folder as well as in development server.


