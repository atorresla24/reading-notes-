# Class 13 reading notes

## The Past, Present, and Future of Local Storage for Web Applications

Cookies have three downsides:
* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

## A Brief History of Local Storage Hacks before HTML5

**userData** allows web pages to store up to 64kb of data per domain

Trusted domains could hold 10 times that amount (640 kb)

2002 - Flash 6 could store 100 kb of data/domain

2006 - Flash 8 could store 100 kb of data for free and increment in magnitude increase

2007 - Google launched Gears which was able to store unlimited amounts of data/domain

2009 - dojox.storage could auto-detect Adobe Flash, Gears, Adobe AIR, and a prototype of HTML5

HTML5 storage = Local storage = DOM storage

Storage event would be fired everytime a setItem(), removeItem() or clear() was called

### Current HTML limitations:

* % megabytes is storage space by default
* "QUOTA_EXCEED_ERR" is the exception that will get thrown if storage is exceeded 
* More storage is not able to be requested

