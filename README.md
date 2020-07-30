# TravelBetter - Getting there Greener

[![License](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![Slack](https://img.shields.io/badge/Join-Slack-blue)](https://callforcode.org/slack) [![Website](https://img.shields.io/badge/View-Website-blue)](https://code-and-response.github.io/Project-Sample/)

A basic GitHub repository example for Call for Code submissions and those projects that join the Code and Response initiative. Not all sections or files are required. You can make this as simple or as in-depth as you need.

*Read this in other languages: [English](README.md), [한국어](README.ko.md), [português](README.pt_br.md).*

## Contents

1. [Short description](#short-description)
1. [Demo video](#demo-video)
1. [The architecture](#the-architecture)
1. [Sequence Diagram](#sequence-diagram)
1. [Long description](#long-description)
1. [Project roadmap](#project-roadmap)
1. [Getting started](#getting-started)
1. [Running the tests](#running-the-tests)
1. [Live demo](#live-demo)
1. [Built with](#built-with)
1. [Contributing](#contributing)
1. [Versioning](#versioning)
1. [Authors](#authors)
1. [License](#license)
1. [Acknowledgments](#acknowledgments)

## Short description
Application to easily motivate and reward people for making greener transportation choices. 

### What's the problem?

Global warming refers to the steady temperature rise on our earth. Both land and oceans are warmer now than they were when record-keeping began, in 1880. The U.S. Energy Information Administration states that greenhouse gases are gases that keep heat in the earth’s atmosphere. Although greenhouse gases do occur naturally, human activity contributes a great deal to greenhouse gas emissions. Your carbon footprint — or your impact on the environment — measures the greenhouse gases that you are responsible for creating. Common activities like using electricity and driving a car emit those gases. Usually, the bulk of an individual’s carbon footprint will come from transportation, housing, and food. OR:
Your carbon footprint — or your impact on the environment — measures the greenhouse gases that you are responsible for creating. Common activities like using electricity and driving a car emit those gases. Existing programs to help guide people in reducing their carbon footprint are cumbersome and unrewarding for a majority of people. 

### How can technology help?

While scientists and environmentalists are working on building solutions to reduce global warming, technologists can build solutions to make people more carbon aware and provide simple and easy ways to reduce it. Technology can motivate people to make better choices in order to reduce their personal carbon footprint. 

### The idea

Our idea is make people aware of the carbon impact of their transportation choices, provide greener alternatives, and offer rewards for choosing more environmentally friendly options. OR:
Our solution is to reward people for making better choices when they commute. The simplicity will entice more people to make green choices and, in turn, produce a positive impact on an individual’s carbon footprint. 

## Demo video

[![Watch the video](https://github.com/Code-and-Response/Liquid-Prep/blob/master/images/IBM-interview-video-image.png)](https://youtu.be/vOgCOoy_Bx0)

## The architecture

![Architecture](architecture.JPG)

1. The user opens app on ios device. Home page loads with an option to search transportation between **to** and **from** location.
2. App will track transportaion option used.
3. Reward user for choosing environment friendly transportation uses.
4. User's activity history will be stored in couchDB on Cloudant.

## Long description

[More detail is available here]  https://docs.google.com/document/d/1FS9JgiJnzqeq37P7SOzykA6unKFmfhaZGWISB468fQg/edit

## Project roadmap

![Roadmap](roadmap.jpg)

## Getting started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Setting up the development environment

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

```
# Initiate the project as an expo compatible react-native project
expo init
# install all dependecy 
yarn
```

End with an example of getting some data out of the system or using it for a little demo

## Testing the Application on iOS/Android

Run the following command to build and start the app. 

```
# Start the app using Metro server. (Learn Metro Server: https://docs.expo.io/workflow/how-expo-works/)
expo start
```

There are two methods to test the app. Firstly, using installed simulator on your computer. Secondly, using Expo app on your iOS/Android device. We recommend the latter for the ease of use. For that, you have to install Expo from Appstore/Google Play Store. 

The latest command will run the project and will open a new tab in your browser called Metro Bundler. Metro Bundler interface will show a barcode on your screen. Scan the barcode with your camera/other app. Scanned barcode will pop a notification badge, clicking that will switch you to the App hosted in Expo. 

### Testing the API using Swagger

[PREETI's WORK]
Explain what these tests test and why, if you were using something like `mocha` for instance

```bash
npm install mocha --save-dev
vi test/test.js
./node_modules/mocha/bin/mocha
```

### And coding style tests

Explain what these tests test and why, if you chose `eslint` for example

```bash
npm install eslint --save-dev
npx eslint --init
npx eslint sample-file.js
```

## Live demo

You can find a running system to test at [callforcode.mybluemix.net](http://callforcode.mybluemix.net/)

## Built with

* [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
* [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logic
* [IBM API Connect](https://cloud.ibm.com/catalog?search=api%20connect#search_results) - The web framework used
* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency management
* [Springboot](https://start.spring.io/) - Used to generate backend user , activity CRUD APIs

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

* **Joel Conybear**
* **Lauren Colalillo**
* **Mutugi**
* **Preeti Gupta**
* **Rakib Shahriar**


See also the list of [contributors](https://github.com/Code-and-Response/Project-Sample/graphs/contributors) who participated in this project.

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).
