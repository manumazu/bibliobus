# Bibliobus
[Bibliobus](https://bibliob.us) is a lighting system for bookcases that integrates a method of locating objects by light signal.
The lighting is controlled in Bluetooth via a mobile application connected to an API which contains an index that can be searched remotely.
It allows you to search for and locate objects placed on a support remotely using light.

List of open sources for this project

## Microcontroller Bibus 
The Bluetooth LE controller controls the display of the lights: it receives and processes the messages sent from the mobile app via Bluetooth Low Energy and transmits them to the self-addressable LEDs to light up those associated with the requested positions.

Source code for prototype [Leds display and Bluetooth communication](https://github.com/manumazu/bibus-proto)

## Bibliobus API
The API centralizes data about objects and their location on the shelf. 
It organize the items and authenticate the connection with the Bluetooth controller via the mobile app. 
It is the one that contains the classifying system for information.

Source code for [API project](https://github.com/manumazu/bibliobus-api)

## Test API sample
Sample project for Mobile App which sould act as a relay between the controller and the API that stores the information. The app transmits location information to the lighting system based on the position data. It is also used to reference objects in the index.

Sample project for [testing API](https://github.com/manumazu/bibliobus-demo)

## Biblio Front
[VueJS front project](https://github.com/manumazu/bibliofront) for book index arrangement 

## Biblio Game
[Blockly Project](https://github.com/manumazu/bibliogame) to learn coding with blocks (as Scratch), and play with Bibus module lighting : make loops, conditions, timers ... preview in the browser the result and then display code on leds usinfg mobile app. Fun for kids who want to learn coding. 
