# Change Log

## 5.0.0

* Add support for Frame TVs
* Add Power switch for Frame TVs
* Add Art Mode switch for Frame TVs
* Use events for initialise elements and status changes
* Refresh all accessories when state of TV changes

For more informations regarding Frame Support please follow this link: https://git.io/JOII1


## 4.4.1

* Fix bug that destroy storage because of multiple savings in the same time

## 4.4.0

* Cleanup unused Keys from config
* Accept multiple commands as string separated by comma
* Update config schema for Config Ui X settings interface
* If TV responds to ping, check the PowerState value if TV supports it
* Implement a caching method for requests so we don't stress the TVs
* Added error message when failing to fetch installed applications
* Stylized the response for installed applications output
* Reinitialize remote after TV informations where fetched
* Remove sleeping mode when turning off the device if TV supports PowerState

## 4.3.7

* Use POST method to open applications

## 4.3.6

* Update Readme
* Add funding option for Config Ui X
* Replace deprecated package

## 4.3.4

* Add error message when TV is off and is trying to fetch installed apps
* Fix warning message from Homebridge 1.3.0

## 4.3.0

* Add support for WoL settings
* @mxdanger helped us with adding option to customize the settings from Config UI X interface!

## 4.2.1

* Fix open Apple TV application
* Add Mute Characteristic for volume
* Add a new method to display installed apps

## 4.2.0

* Bug fixing
* Group switches with the main accessory since from iOS 13.2 you have the option to show them separately.

## 4.1.0

* Bug fixing
* Compatible with iOS 13.

## 4.0.0

* Bug fixing
* New method for declaring accessories.

**IMPORTANT!** With this release the TVs will be declared as external accessories.
Updating from v3 to v4 will require you to add the TVs in Home app again.

This is required because HomeKit expects only one TV per bridge and now every TV will act as a bridge.

You can read how to add the TV in [Step 6 from Configuration page](https://github.com/tavicu/homebridge-samsung-tizen/wiki/Installation#6-adding-the-tv-to-home-app)

## 3.1.3

* Never fail custom switches for better working with automations

## 3.1.1

* Fix a bug that didn't display installed apps when running `tizen-apps`
* Improvements of how accessories are created

## 3.1.0

* Bug fixing
* Change default settings for `refresh` option
* Option to change remote keys mapping

## 3.0.0

* Use the new iOS 12.2 support for `Television` as accessory type
* Option to add inputs for TV with the new iOS 12.2 feature
* Control TV from Remote Control Center
* Save the token automaticaly on the server
* More options for `refresh` in real time
* Better logging in debug mode
* New method to check if TV is active
* Option to hold a command key for a time

## 2.1.0

* Option to open applications with a switch
* New support to update the switches with state in real time