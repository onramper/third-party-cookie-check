# third-party-cookie-check

This is used to check if third pardty cookies enabled on the browser. This will try to create a temparary cookie in the app domain and give the status as an event message. Web app should listen to the event to get the cookie status.

``` 
window.addEventListener(
      "message",
      function listen(event) {
        if (event.data === "3pcSupported" || event.data === "3pcUnsupported") {
         // add you logic here
        }
      },
      false
    );
```
