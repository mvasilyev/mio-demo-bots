# Message.io HipChat Weather Add-On

## API Keys

For this to work you'll need 2 API keys.

1. Forecast API key, get it @ https://darksky.net/dev/
2. Google geolocation API key, get it @ https://developers.google.com/maps/documentation/geolocation/get-api-key

Place those keys in .env file as "forecastAPIKey" and "googleAPIKey" respectively.

## Configuration

You will also need to change "localBaseUrl" in config.json. Use your Glitch app url. This application's one is `https://mio-hipchat-weather.glitch.me` (don't add trailing slash at the end).

## Boarding on your HipChat

After all set up, go to your HipChat Group Integration settings @ `https://<your-group-name>.hipchat.com/addons/` and scroll down to "Install an integration from a descriptor URL" link.

Paste descriptor link there, for this app it would be `https://mio-hipchat-weather.glitch.me/atlassian-connect.json`, replace base URL to yours.

Clisk "Approve", and all done!

You now can send message 
> /weather zipcode

in any room your Add-on installed it and get weather forecast for this area.