# Local Storage

Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

## LOCAL STORAGE HACKS BEFORE HTML5

* Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.

userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.

* In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain.

* By 2006, with the advent of ExternalInterface in Flash 8, accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker dojox.storage. Flash gives each domain 100 KB of storage “for free.” Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).

* In 2007, Google launched Gears

* By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.

## INTRODUCING HTML5 STORAGE

it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually).

From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object.

USING HTML5 STORAGE

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

TRACKING CHANGES TO THE HTML5 STORAGE AREA
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)

`if (window.addEventListener) {`
  `window.addEventListener("storage", handle_storage, false);`
`} else {`
  `window.attachEvent("onstorage", handle_storage);`
`};``
The handle_storage callback function will be called with a StorageEvent object, except in Internet Explorer where the event object is stored in window.event.

`function handle_storage(e) {`
` if (!e) { e = window.event; }`
`}`


## STORAGEEVENT OBJECT

|PROPER  |	TYPE|                            	DESCRIPTION|
|-------------|--------------|----------------------------------|
|key|	string|	the named key that was added, removed, or modified|
|oldValue	|any|	the previous value (now overwritten), or null if a new item was added|
|newValue	|any|	the new value, or null if an item was removed|
|url*|	string|	the page which called a method that triggered this change|

### The resources used on this reading

1. <http://diveinto.html5doctor.com/storage.html>

2. <https://www.w3schools.com/jsref/prop_win_localstorage.asp>