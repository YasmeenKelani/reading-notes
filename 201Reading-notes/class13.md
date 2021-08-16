# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS
* DIVING IN :

- <img src="https://diveinto.html5doctor.com/i/aoc-p.png" alt="summary" width="60"/>   Persistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

- Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:
1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.
* What we really want is:
1. a lot of storage space.
2. on the client.
3. that persists beyond a page refresh.
3. and isn’t transmitted to the server.

<img src="https://www.webfx.com/blog/images/assets/cdn.sixrevisions.com/0182-01_introduction_html5_webstorage_thumbnail.jpg" alt="summary" width="500"/>  

* INTRODUCING HTML5 STORAGE:
- So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

**check for HTML5 Storage**

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```
* HTML5 STORAGE IN ACTION:
* How does it work? Every time a change occurs within the game, we call this function:

```
function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}
```

<img src="https://image2.slideserve.com/4041342/html5-in-action-l.jpg" alt="summary" width="500"/>

For more information please visit [Local Storage for web Application](http://diveinto.html5doctor.com/storage.html).