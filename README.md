# babyMonitor

Using a Tessel micro controller and the climate modules to monitor the temperature in the cradle. Set a threshold value when to get a push to your mobile device.

Create an account at pushbullet.com.
On settings click the "Create access token". Make sure you save the token to use in the script (or elsewhere).
Download pushbullet app on your phone or table (both android and iphone availiable, and also as a chrome plugin), log in with the sam credentials as give at pushbullet.com.
I haven't figured out how to get the device ID from the user interface at pushbullet.com but you can run the following code

var PushBullet = require('pushbullet');
var pusher = new PushBullet('<YOUR_ACCESS_TOKEN>');

pusher.devices(function(error, response) {
	console.log(response);  // response is the JSON response from the API
});

In the output (JSON) you can find your devive ID.

Try it. It is simple
