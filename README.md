# Pako Bots UI (web and phone)

![OSI Certified](https://origami3.com/osi_keyhole_100X100_90ppi.png)

OSI Certified Open Source Software

## Getting started

Before you start, make sure you have a recent version of [NodeJS](http://nodejs.org/) environment *>=6.0* with NPM 3 or Yarn. If building for the phone, please ensure the latest version of the [Cordova](https://cordova.apache.org/#getstarted) installed.

## Building the web application
From the project folder, execute the following commands:

```shell
npm install 
```

This will install all required dependencies, including a local version of Webpack that is going to
build and bundle the app. There is no need to install Webpack globally.

To run the app execute the following command:

```shell
npm serve # or: yarn serve
```

This command starts the webpack development server that serves the build bundles.
You can now browse the skeleton app at http://localhost:8080 (or the next available port, notice the output of the command). Changes in the code
will automatically build and reload the app.

### Running with Hot Module Reload

If you wish to try out the experimental Hot Module Reload, you may run your application with the following command:

```shell
npm start -- webpack.server.hmr
```

### Bundling

To build an optimized, minified production bundle (output to /dist) execute:

```shell
npm run prod
```

## Building the phone application
Before building the phone application ensure the web application is built first.
From the project folder, execute the following commands:

```shell
cordova build
```

### For the masochistic: Apple Deployments :(

Expect to spend an hour or more getting from the desktop to the app store.
Watch email for any messages with bundle errors. There is no history on itunes connect. Why didn't my build show?
info.plist add NSBluetoothPeripheralUsageDescription key
1024x1024 icon and execute npm run icons
Signing key issues. Uncheck the manage signing keys and check it again. Talk about a bug!!
Yeah, not an apple fan :(
