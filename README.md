# EKS Vehicle Speed Restriction

This lightweight FiveM script enforces maximum speed limits on specified vehicles by model name. Perfect for realism-based servers where certain vehicles (e.g., police, utility, or civilian) must follow fixed speed caps.

## Features

* Configurable max speed per vehicle model
* Easy-to-edit `config.lua` for speed limits (in MPH)
* Automatically throttles speed if the limit is exceeded
* Optimized for performance with low tick usage

## Installation

1. Drag and drop the folder into your `resources/` directory
2. Add the following to your `server.cfg`:

ensure EKS_SpeedLimiter

3. Open `config.lua` and define your vehicle speed limits:

Config.SpeedLimits = {
    [`adder`] = 80,
    [`sultan`] = 60,
    [`police`] = 90,
    [`t20`] = 70,
}

4. Start your server. The script will automatically apply speed limits when a player is driving one of the defined vehicles.

## Notes

* Speeds are set in **MPH**
* Vehicles not listed in the config are unaffected
* Script uses `SetVehicleForwardSpeed` to gently reduce speed � customizable for stricter behavior if needed

## Support

For assistance or custom enhancements, open a ticket with EKS:
https://discord.gg/busQ9w6dqa
