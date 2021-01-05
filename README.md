- I created a cordova project called clr_plugin and a plugin called RoundTrip and added it to the clr_plugin project.
- In index.js, I added a call to my plugin's roundtrip.js file as shown below:
    window.plugins.RoundTrip.roundTripData("hello world", function(returnText) {
        alert(returnText);
    });
- In the RoundTrip plugin, I added the plugin.xml file and hooked up the roundtrip.js file
- In the RoundTrip plugin, I added the RoundTrip.java class and added the execute function and another function called roundTrip which either returns the expected string or an error
- When I run the app, nothing is being alerted to the screen.  I am thinking that I don't have my plugin.xml set up correctly.  The javascript and java code that I wrote appears as though it would work correctly, but I cannot test it.
- I can put javascript alerts in the plugin's js file to show that I am getting to that file, but I don't think the exec code is firing because of improper declarations in the xml file.
