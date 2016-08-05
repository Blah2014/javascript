# javascript
javascript related stuff

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
