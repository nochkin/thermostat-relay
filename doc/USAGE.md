# Usage

## General introduction
The Thermostat Relay Board (the Relay Board) is a bridge between line voltage heating/cooling system (normally operates at 120V or 240V AC) and a low voltage thermostat (operates at 24 VAC).
Source repository: https://github.com/nochkin/thermostat-relay

Compatible low voltage smart thermostats are, but not limited to:
* Ecobee (all generations).
* Google Nest (all generations). In case when 3-stage fan is being used, a Nest Learning thermostat must be used due to additional connections supporting it.
* Other WiFi-based low voltage smart thermostats.
A thermostat must provide separate connections for heat and cool, and additional optional connections for fan.

A fully populated Relay Board is capable of controlling Cooling, Heating and 3-stage Fan. But the board can be built using some of the features depending on the requirements.

## Relay Board layout
The Relay Board consists of two logical parts:
* Low voltage. This side takes control signals from the connected low voltage thermostat and sends control signals to correspondent relays.
* High voltage. This side controls high voltage lines of the existing heating/cooling system or/and fan depending on the configuration.

## Connection
> [!CAUTION]
> There is a high voltage which can be dangerous when not handled properly. Make sure you know what you are doing when working with a high line voltage.

The schematic diagram using Nest thermostat as example is shown below:

![Connection diagram](../images/thermostat-relay5-connection.png)

## Nest wiring
In order to able to use 3-stage fan, the setup should have a thermostat which has enough connections (i.e. Nest Learning thermostat).
In case of the initial configuration of Nest thermostat, the configuration must be done using the Pro Setup to assign additional connections for the fan.
The final configuration should look like this:

![Nest wiring](../images/nest-connection.png)
| Connection | Function |
| --- | --- |
| Y1 | Cool |
| W1 | Heat |
| G | Regular fan (low speed) |
| Y2 | Fan G2 (medium speed) |
| * | Fan G3 (high speed) |
| Rh | 24V AC (Power) |
| C | 24V AC (Common) |

In the Pro setup is may be neccessary to activate the Fan signal when heating or cooling.

