CordovaCallNumberPlugin
=======================

Call a number directly from your cordova application.



## Installation

``` 
cordova plugin add https://github.com/8bhsolutions/CordovaCallNumberPlugin.git
```

## Remove

``` bash
cordova plugin remove 8bhsolutions-cordova-plugin-power-button-listener
```

Use the plugin in your JS file:
``` javascript
window.plugins.CallNumber.callNumber(onSuccess, onError, number, bypassAppChooser);
```

**number:** *String;* phone number to call (e.g. "1234567890")

**bypassAppChooser:** *boolean;* true if you always wish to bypass the app chooser if user has multiple applications installed that can handle calls

Make sure to create onSuccess and onError call back functions.

Example:
``` java
function onSuccess(result){
  console.log("Success:"+result);
}

function onError(result) {
  console.log("Error:"+result);
}
```
