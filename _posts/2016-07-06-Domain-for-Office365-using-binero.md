---
layout: post
title: Connecting a domain to Office 365 using Binero
date: 2015-05-11 17:25:00
categories: [Other]
author: Jimmy Engström
tags: [Office-365]
---
I have used Binero for many years now.
Binero is a Swedish web hosting but I primarily use it for handling my domains.
I have a lot of those and connecting them to Office 365 kan be pretty time consuming (since there is a lot of entries).
The first step is to prove to Office 365 that this is actually your domain.

### 1. Prove it's your domain 

**bold**
*italic*



Domains and websites > DNS
Select yous site in the site selector.
In my case I am going to move ZXBox.com, the first step is to remove all the entries you don't need.
Now you can select Export zone
You will get a file that looks like this:

```
zxbox.com. 3600 IN SOA ns3.binero.se. registry.binero.se. 1467244800 43200 3600 604800 3600
zxbox.com. 86400 IN NS ns3.binero.se.
zxbox.com. 86400 IN NS ns4.binero.se.
zxbox.com. 86400 IN NS ns5.binero.se.
zxbox.com. 86400 IN NS ns6.binero.se.
zxbox.com. 86400 IN NS ns7.binero.se.
awverify 7200 IN CNAME zxbox.azurewebsites.net.
www 7200 IN CNAME zxbox.azurewebsites.net.
```