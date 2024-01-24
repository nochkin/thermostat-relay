# Usage

## General introduction
The Thermostat Relay Board (the Thermostat Board) bridges line voltage heating/cooling system and low voltage thermostats which can be used with 24 VAC systems.

Compatible low voltage smart thermostats are, but not limited to:
* Ecobee (all generations)
* Google Nest (all generations)
* Other WiFi-based low voltage smart thermostats

Compatible line voltage cooling/heating systems are those which are controlled by line voltage which can be 120V AC or 240V AC.

The fully populated board is capable of controlling Cooling, Heating and 3-stage Fan. But the board can be built using some of the features depending on the requirements.

## Board layout
The Thermostat Board consists of two logical parts:
* Low voltage. This side takes control signals from the connected low voltage thermostat and sends control signals to correspondent relays.
* High voltage. This side controls high voltage lines of the existing heating/cooling system or/and fan depending on the configuration.
