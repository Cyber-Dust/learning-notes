# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS
[CLick here to read](http://diveinto.html5doctor.com/storage.html)
## Diving In
Native client applications are superior over web applications

Values may be stored in INI files, XML files,
## Brief History of Local Storage Hacks Before HTML5
uerData allows web pages to store up to 64kb of data per domain

Flash cookies or Local Shared Objects= store up to 100kb of data per domain
## Introducing HTML5 Storage
HTML5 sotrage is a way for web pages to store named key/value pairs locally witihin the client web browser

HTML5 STORAGE SUPPORT
IE	FIREFOX	SAFARI	CHROME	OPERA	IPHONE	ANDROID
8.0+	3.5+	4.0+	4.0+	10.5+	2.0+	2.0+

CHECK FOR HTML5 STORAGE:

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```
or use Modernizr

```
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```
## Using HTML5 Storage
THe named key stored is a string

use `parseInt()` or `parseFloat()` to put into JS datatype 

## Tracking Changes to the HTML5 Storage Area
![H](Screen Shot 2021-05-19 at 3.45.44 AM.png)
## Limitations in Current Browsers
No browser supports any mechanism for web devs to request more storage space.

