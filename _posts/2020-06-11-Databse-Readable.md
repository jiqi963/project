---
layout: post
title: Make Data Readable Pn Database
subtitle: data type between Ascii and decimal
---

## Last Ticket for me

#### Work in ingest file

[Ticket](https://gitlab.com/iotop/polykids-project/-/issues/13)

My noise's data in our Database it ascii type

![data](https://raw.githubusercontent.com/jiqi963/project/master/img/data1.png)

To convert ascii to decimal I found a PHP function called ord() — Convert the first byte of a string to a value between 0 and 255

[Function ord](https://www.php.net/manual/en/function.ord.php)

I going to convert it on our ingest file on kate server.

there is a table show how to convert data type for each format

![ASCII](https://raw.githubusercontent.com/jiqi963/project/master/img/ascii.png)

#### Work in Arduino code

Bee has similar situation when she builds the co2 sensor, the same code working in the 32u4 rather than M0 board.

I going to try the code in 32u4