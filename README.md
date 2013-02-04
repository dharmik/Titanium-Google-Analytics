# Google Analytics for Titanium Mobile


I started this project by creating a Titanium Module for wrapping the Google Analytics SDK iOS static library. However that effort faild; due to using the sql dynamic library 3.0. I just could not get it working!

So, I rolled out the functionality directly in Titanium.

It works exacly the same by tracking pageviews in a database and periodically sending them to Google Analytics, if and when a network conection is available.

*Note:* To make sure that the database does not get flooded with data it holds a max of 1000 events.
This also helps load when it sends the events to Google. Once the event is sent to Google it is ejected
from the database.

To use: all you need is the Ti.Google.Analytics.js file and follow the examples in the app.js.

*From Google*: You must indicate to your users, either in the application itself or in your 
terms of service, that you reserve the right to anonymously track and report a user's activity 
inside of your app.

I hope some people find this useful.


----------------------------------

Copyright (c) 2010 by Roger Chapman. All Rights Reserved.

This code is licensed under the MIT License. Please
see the LICENSE file for the full license.
