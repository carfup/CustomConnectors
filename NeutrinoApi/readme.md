# Neutrino API
A complete set of actions around Data tools, WWW, Telephony, Geolocation, Security and Networking, E-Commerce and Imaging.

## Publisher: Clément Olivier

## Prerequisites
You need to have a Neutrino API account. You can [sign up](https://www.neutrinoapi.com/signup/) for free.

## Supported Operations
The connector supports the following operations:
* `Image Resize`: Resize an image and output as either JPEG or PNG.
* `Image Watermark`: Watermark one image with another image.
* `HTML Render`: Render HTML content to PDF, JPG or PNG.
* `QR Code`: Generate a QR code as a PNG image.
* `Phone Playback`: Make an automated call to any valid phone number and playback an audio message.
* `SMS Verify (premium)`: Send a unique security code to any mobile device via SMS.
* `HLR Lookup (premium)`: Connect to the global mobile cellular network and retrieve the status of a mobile device.
* `SMS Message (premium)`: Make an automated call to any valid phone number and playback a unique security code.
* `Phone Verify (premium)`: Create a new contact list.
* `Verify Security Code`: Check if a security code sent via SMS Verify or Phone Verify is valid.
* `Phone Validate`: Parse, validate and get location information about a phone number.
* `Email Validate`: Parse, validate and clean an email address.
* `Email Verify`: SMTP based email address verification.
* `UA Lookup`: Parse, validate and get detailed user-agent information from a user agent string or from client hint fields.
* `Bad Word Filter`: Detect bad words, swear words and profanity in a given text.
* `IP Blocklist Download`: This API is a direct feed to our IP blocklist data.
* `IP Blocklist`: The IP Blocklist API will detect potentially malicious or dangerous IP addresses.
* `IP Probe`: Analyze and extract provider information for an IP address.
* `Host Reputation`: Check the reputation of an IP address, domain name or URL against a comprehensive list of blacklists and blocklists.
* `Geocode Address`: Geocode an address, partial address or just the name of a place.
* `IP Info`: Get location information about an IP address and do reverse DNS (PTR) lookups.
* `Geocode Reverse`: Convert a geographic coordinate (latitude and longitude) into a real world address.
* `Convert`: A powerful unit conversion tool.
* `BIN Lookup`: Perform a BIN (Bank Identification Number) or IIN (Issuer Identification Number) lookup.
* `BIN List Download (premium)`: Download our entire BIN database for direct use on your own systems.
* `URL Info`: Parse, analyze and retrieve content from the supplied URL.
* `HTML Clean`: Clean and sanitize untrusted HTML.
* `Browser Bot`: Browser bot can extract content, interact with keyboard and mouse events, and execute JavaScript on a website.

## Obtaining Credentials
### Neutrino side
From the [main account page](https://www.neutrinoapi.com/account/main/), you can grab the User Id and Root Key.
For more keys, please visit the [API Keys page](https://www.neutrinoapi.com/account/keys/), to add or revoke API Keys.

### Custom connector side
Once you are configuring the connector on the Power Platform.

The API requires two parameters sent to the header in order to authenticate the user.
As of today, a custom connector can allow only one parameter at a time.

My decision was then to : 

* You will have to use the **API Key** in order to validate the security stage in the process.
* You will have to pass the **User Id** as parameter to each actions.

## Getting Started
Visit Neutrino [REST API reference](https://www.neutrinoapi.com/api/api-basics/) documentations page for further details. 

## API Limit & Premium
Within the Free tier, you have access to almost all actions with a dedicated number of calls allowed per day.

Some actions in the connector actions have a "(premium)" info, this means that with the Free tier of the API, you won't be able to use this particular action.

For ugrade to higher tier, please visit the [Plans page](https://www.neutrinoapi.com/plans/)

## Deployment Instructions
Import the swagger file in target Power Apps environment.
