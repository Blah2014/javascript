# javascript
javascript related stuff

***Please donate if you are using this repo***

***Note:*** If you found this project helpful please give this repo a star.

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C2HFZWSUPV47Q" target="_blank">
  <img src="https://raw.githubusercontent.com/Blah2014/phonegap-inmobi-plugin/gh-pages/images/BuymeaCoffee.png" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!" />
</a>

<a href="http://traderhub.info" target="_blank">
  <img src="http://traderhub.info/images/AD.jpg" border="0" name="submit" alt="TraderHub - daily stock picks, market signals, stock picking service" />
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
