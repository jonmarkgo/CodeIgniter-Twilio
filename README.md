======================================
Twilio CodeIgniter Library

by Ben Edmunds
======================================

A basic Twilio REST API CodeIgniter library wrapper using the PHP class provided by Twilio.



SETUP:
Just drop the files in their appropriate folders (ie "libraries/twilio.php" goes in your "libraries" folder) and add your settings in the "config/twilio.php" file.


NOTES:
All calls to the rest class are routed through the library class, so for example:

instead of:
$client = new TwilioRestClient($AccountSid, $AuthToken);
$response = $client->request("/$ApiVersion/Accounts/$AccountSid/Calls", "POST", $data); 

you would do something like:
$this->load->library('twilio');
$this->twilio->request("/$ApiVersion/Accounts/$AccountSid/Calls", "POST", $data);




-Ben Edmunds
 ben.edmunds@gmail.com
 @benedmunds 
[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/19a2e5150dc9d7adfb27579856152f82 "githalytics.com")](http://githalytics.com/jonmarkgo/CodeIgniter-Twilio)
