# TravelBetter - Getting there Greener

[![License](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![Slack](https://img.shields.io/badge/Join-Slack-blue)](https://callforcode.org/slack) [![Website](https://img.shields.io/badge/View-Website-blue)](https://code-and-response.github.io/Project-Sample/)

A basic GitHub repository example for Call for Code submissions and those projects that join the Code and Response initiative. Not all sections or files are required. You can make this as simple or as in-depth as you need.

## Contents

1. [Short description](#short-description)
1. [Demo video](#demo-video)
1. [The architecture](#the-architecture)
1. [Long description](#long-description)
1. [Project roadmap](#project-roadmap)
1. [Getting started](#getting-started)
1. [Running the tests](#running-the-tests)
1. [Built with](#built-with)
1. [Authors](#authors)
1. [License](#license)
1. [Acknowledgments](#acknowledgments)

## Short description
Application to easily motivate and reward people for making greener transportation choices. 


## Demo video

[![Watch the video] https://www.youtube.com/watch?v=Biz8hGz83Mo 

## The architecture

![Architecture](travel-better-revised-system-architecture.png)

1. The user opens app on ios device. Home page loads with an option to search transportation between **to** and **from** location.
2. App will track transportaion option used.
3. Reward user for choosing environment friendly transportation uses.
4. User's activity history will be stored in couchDB on Cloudant.

## Long description

[More detail is available here]  https://docs.google.com/document/d/e/2PACX-1vQDmkoT82gDPPEZaUrljtuVQABfzWJATySDlQ96wBHufg9_c4cgY1TmJwyC8dA-nW4ZF86pRgwQ7DvV/pub

## Project roadmap

![Roadmap](roadmap.jpg) 

## Getting started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Setting up the development environment

**Front End**
Please run the following commands from your computer's terminal/powershell.

```bash
# Check your Node.js installation. If you do not have Node.js, please install it from https://nodejs.org/en/download/
node -v
# If you don't have expo-cli yet, get it
npm i -g expo-cli
# If you don't have react-native-cli yet, get it
npm i -g react-native-cli
```
Install Visual Studio Code IDE to inspect and run the code. You can find more detailed instruction from here: https://www.youtube.com/watch?v=0-S5a0eXPoc ()

**Back End**
Install maven from https://maven.apache.org/install.html

Create account with IBM Cloud.

Install IBM CLI (Refer to https://cloud.ibm.com/docs/cli?topic=cli-getting-started#overview)

Provision a CouchDB instance using Cloudant (Refer to https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-creating-an-ibm-cloudant-instance-on-ibm-cloud)

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

Clone this repository and open the directory in VSCocde as a react-native project. Open Terminal from the menu of VSCode. In the terminal interface, please run the following commands (on the project root directory). 

**Front End**
```
# Initiate the project as an expo compatible react-native project
expo init
# install all dependecy 
yarn
```

End with an example of getting some data out of the system or using it for a little demo

**Back End**
Modify /user-module/src/main/resources/application.properties with your Cloundant instance details.

Navigate to user-module and perform **mvn clean install**

After clean build, run main class /user-module/src/main/java/com/callforcode/travelbetter/TravelBetterApplication.java

## Testing the Application on iOS/Android

Run the following command to build and start the app. 

```
# Start the app using Metro server. (Learn Metro Server: https://docs.expo.io/workflow/how-expo-works/)
expo start
```

There are two methods to test the app. Firstly, using installed simulator on your computer. Secondly, using Expo app on your iOS/Android device. We recommend the latter for the ease of use. For that, you have to install Expo from Appstore/Google Play Store. 

The latest command will run the project and will open a new tab in your browser called Metro Bundler. Metro Bundler interface will show a barcode on your screen. Scan the barcode with your camera/other app. Scanned barcode will pop a notification badge, clicking that will switch you to the App hosted in Expo. 

### Testing the API using Swagger

Access swagger using http://localhost:8080/swagger-ui.html , after back end application is up and running on local system.

Cloud swagger URL is https://travelbetter.mybluemix.net/swagger-ui.html. Please note this URL has limited availability and may expire by mid-Aug 2020.

### And coding style tests

Explain what these tests test and why, if you chose `eslint` for example

```bash
npm install eslint --save-dev
npx eslint --init
npx eslint sample-file.js
```

## Built with

* [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
* [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logic
* [React Native](https://reactnative.dev/) - The ios/android app framework used
* [Google APIs](https://developers.google.com/apis-explorer) - The location, direction services used
* [Maven](https://maven.apache.org/) - Dependency management
* [Springboot](https://start.spring.io/) - Used to generate backend user , activity CRUD APIs

## Authors

* **Joel Conybear**
* **Lauren Colalillo**
* **Mutugi Mutuma**
* **Preeti Gupta**
* **Rakib Shahriar**

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Thanks to IBM Mentors for helping us through **TravelBetter** journey. Special shout out to **Jean-Georges Perrin**, **Shari Chiara** for being available and resolving issues quickly.
