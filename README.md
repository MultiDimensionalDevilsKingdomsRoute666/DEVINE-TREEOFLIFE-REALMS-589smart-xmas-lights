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

Set up an MQTT broker, run the Node.js server and Pi client code with `npm install` and then `node`, and build the Android app from `clients/`.

## Credit

The original work is by [mcodetrail/smart-xmas-lights](https://github.com/mcodetrail/smart-xmas-lights).

