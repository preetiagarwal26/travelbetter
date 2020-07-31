## React Native project

### Setting up the development environment

**Front End**
Please run the following commands from your computer's terminal/powershell.

```bash
# Check your Node.js installation. If you do not have Node.js, please install it from https://nodejs.org/en/download/
node -v
# If you don't have expo-cli yet, get it
npm i -g expo-cli

### Get your own Google API Key

* Travel-Better application uses 6 APIs related to Google Maps services. To pursue API access, please get your own Google API key. 
* To pursue a Google API key, please visit: https://console.developers.google.com/. In case you are unable to do it, you can request us for key through email: shahriar025@gmail.com
* For more information please visit: https://developers.google.com/maps/gmp-get-started

The app requires the following Google APIs to be activated: 
* Directions API
* Geocoding API
* Geolocation API
* Maps SDK for iOS
* Places API
* Distance Matrix API

### Installing the app codebase

Clone this repository and open the directory your text editor.

Before running the app, open the `screens/TravelCenterScreen.tsx` and enter the Google API Key in the placeholder variable `GOOGLE_API_KEY`

Run the app, in your terminal run the following commands
```
# install all dependecies
yarn

# Start the application
yarn start

## Running the app on your device
You can run the application on your physical device or an emulator
To run on your physical device, follow the instructions on this page: https://reactnative.dev/docs/running-on-device 
To run the device using an emulator on follow the instructions here: https://reactnative.dev/docs/0.60/getting-started
```