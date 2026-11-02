# Smart Xmas Lights

This simple home automation project shows how it can be possible to turn on/off any lights you want at home.
An Android app (usable both with mobile and SmartWatch) allows to monitor the state of the light and change it. 
Server and Rasberry Pi code has been written using Nodejs. The server and the 'thing' talk together through MQTT protocol.
The rPi is connected to a relay which is responsible of turning on/off the light.

Enjoy :)


## Summary

A fork of [mcodetrail/smart-xmas-lights](https://github.com/mcodetrail/smart-xmas-lights). A home-automation project for switching lights over MQTT, with a Node.js server, a Raspberry Pi relay and an Android app.

## What's inside

`Server/` (the Node.js server) and `clients/` (the Raspberry Pi and Android clients).

## How to view or run it

You need an MQTT broker. Both Node.js parts read its address from the `CLOUDMQTT_URL` environment variable.

- **Raspberry Pi client** (`clients/raspberrypi/`): run `npm install`, then `node light.js`. It drives the relay through GPIO using `onoff`.
- **Server** (`Server/`): an Express app. Run `npm install`. Note that its `npm start` script points to `./bin/www`, which isn't in this repo. `app.js` exports the app without starting a listener, so you need to add a small start file (for example `bin/www` calling `app.listen(3000)`) before running it.
- **Mobile apps**: a native Android app (Gradle project in `clients/android-app/Casa/`, open it in Android Studio) and an Ionic app (`clients/Ionic-app/`, run `npm install`, then `npm run build`).

## Credit

The original work is by [mcodetrail/smart-xmas-lights](https://github.com/mcodetrail/smart-xmas-lights).

