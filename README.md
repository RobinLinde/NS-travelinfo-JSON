# NS-travelinfo-JSON

Repository containing JSON schema for travel information available inside NS trains.
When connected to `WiFi in de trein` you can access the travel information via the URL `http://portal.nstrein.ns.nl/nstrein:main/travelInfo`, which gives you a JSON response following the schema in this repository.

[Schema file](./schemas/travelinfo.json)

The `examples` folder contains some example data.

## Overview

The data roughly consists of the following types of information:

- **Travel information**: Object containing all other information
- **Station**: Object containing information about a station, such as location, names and code. Used in for destination and in stops.
- **Stop**: Object containing information about a stop, the time, platform, station and delay.
- **Train**: Object containing information about a train at a station, such as the type, number and destinations. Used for showing transfer information for the next station.
- **Disturbance**: Object containing information about a disturbance, such as the type, message and the affected stations. Used for showing disturbances on the route. This is currently not yet fully documented in the schema.

## Not yet documented

- All disturbance types
- Messages about splitting trains
- Some warnings and messages
- Phase?
- Station type
