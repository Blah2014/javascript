# javascript
javascript related stuff

***Please donate if you are using this repo***

***Note:*** If you found this project helpful please give this repo a star.

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C2HFZWSUPV47Q" target="_blank">
  <img src="https://raw.githubusercontent.com/Blah2014/phonegap-inmobi-plugin/gh-pages/images/BuymeaCoffee.png" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!" />
</a>

### Index
* [Load js and css files](#user-content-load-js-and-css-files)
* [Find the largest number contained in a JavaScript array](#user-content-find-the-largest-number-contained-in-a-javascript-array)
* [Find the smallest number contained in a JavaScript array](#user-content-find-the-smallest-number-contained-in-a-javascript-array)
* [Angular 2 cli](#user-content-angular-2-cli)
* [Angular 2 Mobile Toolkit](#user-content-angular-2-mobile-toolkit)
* [html2canvas: Screenshots with JavaScript](#user-content-html2canvas-screenshots-with-javascript)
* [GPU and Web UI Performance: Building an Endless 60fps Scroller](#user-content-gpu-and-web-ui-performance-building-an-endless-60fps-scroller)
* [Mapzen: is an open, sustainable, and accessible mapping platform. Our tools let you display, search, and navigate your world](#user-content-mapzen)
* [Simple Statistics: is a JavaScript library that implements statistical methods](#user-content-simple-statistics)
* [regression.js: linear, exponential, logarithmic, power and polynomial trends](#user-content-regressionjs)
* [Live Code Session - Supercharged](#user-content-live-code-session---supercharged)
* [hello.js: A client-side JavaScript SDK for authenticating with OAuth](#user-content-hellojs)
* [Thorin.js: is the Node.js framework](#user-content-thorinjs)
* [Check if element is visible after scrolling](#user-content-check-if-element-is-visible-after-scrolling)
* [Propeller.js: JavaScript library to rotate elements with mouse or touch gestures](#user-content-propellerjs-javascript-library-to-rotate-elements-with-mouse-or-touch-gestures-supports-inertia-and-stepwise-rotation-optimized-for-better-performance)
* [Stickybits is a lightweight alternative to position: sticky polyfills. It works perfectly for things like sticky headers.](#user-content-stickybits-is-a-lightweight-alternative-to-position-sticky-polyfills-it-works-perfectly-for-things-like-sticky-headers)
* [Sortable](https://github.com/RubaXa/Sortable)
* [Interact.js: drag and drop, resizing and multi-touch gestures with inertia and snapping](https://github.com/taye/interact.js)
* [Gridster.js](https://github.com/dsmorse/gridster.js)
* [Bowser: A Browser detector](https://github.com/lancedikson/bowser)
* [Idle Logout](#idle-logout)

##### OCR: Optical character recognition
* [Ocrad.js Optical Character Recognition in JS](#user-content-ocradjs-optical-character-recognition-in-js)
* [Tesseract.js is a pure Javascript port of the popular Tesseract OCR engine](#user-content-tesseractjs-is-a-pure-javascript-port-of-the-popular-tesseract-ocr-engine)

##### Bootstrap 3
* [Bootstrap 3 Datepicker](#user-content-bootstrap-3-datepicker)

##### Table with fixed headers and first column
* [Codepen example](https://codepen.io/MaxArt2501/pen/qLCmE)
* [fixedTableRC](https://github.com/meetselva/fixed-table-rows-cols)

##### Drag and drop
* [Dragula.js: Drag and drop so simple it hurts](https://github.com/bevacqua/dragula)
* [dom-autoscroller.js](https://github.com/hollowdoor/dom_autoscroller)

### Load js and css files
```javascript
function loadScript(url, callback)
{
    // Adding the script tag to the head as suggested before
    var head = document.getElementsByTagName('head')[0];
    var script = document.createElement('script');
    script.type = 'text/javascript';
    script.src = url;

    // Then bind the event to the callback function.
    // There are several events for cross browser compatibility.
    script.onreadystatechange = callback;
    script.onload = callback;

    // Fire the loading
    head.appendChild(script);
}

var myPrettyCode = function() {

   // Here, do what ever you want
};

loadScript("my_lovely_script.js", myPrettyCode);

function loadjscssfile(filename, filetype) {
    if (filetype == "js") { //if filename is a external JavaScript file
       // alert('called');
        var fileref = document.createElement('script')
        fileref.setAttribute("type", "text/javascript")
        fileref.setAttribute("src", filename)
        alert('called');
    }
    else if (filetype == "css") { //if filename is an external CSS file
        var fileref = document.createElement("link")
        fileref.setAttribute("rel", "stylesheet")
        fileref.setAttribute("type", "text/css")
        fileref.setAttribute("href", filename)
    }
    if (typeof fileref != "undefined")
        document.getElementsByTagName("head")[0].appendChild(fileref)
}
```

### Find the largest number contained in a JavaScript array
```javascrip
var array = [267, 306, 108];
Math.max.apply(Math, array);
Result: 306
```

### Find the smallest number contained in a JavaScript array
```javascrip
var array = [267, 306, 108];
Math.min.apply(Math, array);
Result: 108
```

### Angular 2 cli
[Angular 2 cli](https://cli.angular.io/)

### Angular 2 Mobile Toolkit
[Angular 2 Mobile Toolkit](https://mobile.angular.io/)

### html2canvas: Screenshots with JavaScript
[html2canvas](https://html2canvas.hertzen.com/)

### GPU and Web UI Performance: Building an Endless 60fps Scroller
[GPU and Web UI Performance: Building an Endless 60fps Scroller](https://www.youtube.com/watch?v=VAOPi9C8674)

[scrollerjs.com](http://scrollerjs.com/)

### Mapzen
[Mapzen is an open, sustainable, and accessible mapping platform. Our tools let you display, search, and navigate your world](https://mapzen.com/)

### Simple Statistics
[Simple Statistics is a JavaScript library that implements statistical methods](http://simplestatistics.org/)

### regression.js
[regression.js](https://github.com/Tom-Alexander/regression-js)

### Live Code Session - Supercharged
[YouTube: Supercharged with Paul Lewis & Surma](https://www.youtube.com/playlist?list=PLNYkxOF6rcIBz9ACEQRmO9Lw8PW7vn0lr)

[UI Elements: A collection of UI element samples written with vanilla web platform features](https://github.com/GoogleChrome/ui-element-samples)

### hello.js
A client-side JavaScript SDK for authenticating with OAuth2 (and OAuth1 with a oauth proxy) web services and querying their REST APIs.

[hello.js](https://adodson.com/hello.js/)

### Thorin.js
Thorin.js is the Node.js framework that you can use to easily:
* Boot up a pre-configured web-server, sanitize and validate all your input
* Render static HTML files using a templating engine, compile your less & sass styles
* Integrate centralized logging with loglet.io
* Use secure sessions in your requests, stored in redis, MySQL or file system
* Use already written components for some wide-spread services (Redis, ElasticSearch, Sequelize)
* Use a centralized dispatcher to handle your redux actions via HTTP or WebSockets
* Schedule recurring tasks that may use a redis queue to process events
* Extend the core functionality with use-case specific plugins
* Integrate with sconfig.io's discovery system for microservice discovery & authorization
* And much much more.

[Thorin.js](https://thorinjs.com/)

### Check if element is visible after scrolling
```javascript
function isScrolledIntoView(el) {
    var elemTop = el.getBoundingClientRect().top;
    var elemBottom = el.getBoundingClientRect().bottom;

    var isVisible = (elemTop >= 0) && (elemBottom <= window.innerHeight);
    return isVisible;
}
```

### Propeller.js: JavaScript library to rotate elements with mouse or touch gestures. Supports inertia and stepwise rotation. Optimized for better performance
[Propeller.js](https://github.com/PixelsCommander/Propeller)

### Ocrad.js Optical Character Recognition in JS
[Ocrad.js](https://github.com/antimatter15/ocrad.js)

### Tesseract.js is a pure Javascript port of the popular Tesseract OCR engine
[Tesseract.js](http://tesseract.projectnaptha.com/)

### Bootstrap 3 Datepicker
[Datepicker](https://eonasdan.github.io/bootstrap-datetimepicker/)

### Stickybits is a lightweight alternative to position: sticky polyfills. It works perfectly for things like sticky headers.
[Stickybits](https://github.com/dollarshaveclub/stickybits)

### Idle Logout
```
function idleLogout() {
    var t;
    window.onload = resetTimer;
    window.onmousemove = resetTimer;
    window.onmousedown = resetTimer; // catches touchscreen presses
    window.onclick = resetTimer;     // catches touchpad clicks
    window.onscroll = resetTimer;    // catches scrolling with arrow keys
    window.onkeypress = resetTimer;

    function logout() {
        window.location.href = 'logout.php';
    }

    function resetTimer() {
        clearTimeout(t);
        t = setTimeout(logout, 10000);  // time is in milliseconds
    }
}
idleLogout();
```
