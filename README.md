# Volkswagen We Connect ID
Volkswagen We Connect ID sensor provides statistics from the Volkswagen ID API thru ~~[WeConnect-python lib](https://pypi.org/project/weconnect/)~~ [a modified Version of WeConnect-python lib](https://pypi.org/project/weconnect-cupra-daern/0.49.20/).

## Contributors
This is based on the work of many people.
This repo evolved over the following repositories:
- [https://github.com/mitch-dc/volkswagen_we_connect_id](https://github.com/mitch-dc/volkswagen_we_connect_id) - basic toolset
- [https://github.com/alangibson/volkswagen_we_connect_id](https://github.com/alangibson/volkswagen_we_connect_id) - initial adaptation for the Cupra Born
- [https://github.com/daernsinstantfortress/volkswagen_we_connect_id](https://github.com/daernsinstantfortress/volkswagen_we_connect_id) - further enhancements for the Cupra Born

**This component will set up the following platforms.**

Platform | Description
-- | --
`sensor` | Show information from your Volkswagen ID car.
`button` | Start climatization in your Volkswagen ID car.

![image](https://user-images.githubusercontent.com/15835274/149675681-a0c6804c-3179-4fd3-ad74-ab489c8986dd.png)


## Installation

### HACS
The easiest way to add this to your Homeassistant installation is using [HACS](https://custom-components.github.io/hacs/) and add this repository as a custom repository. And then follow the instructions under [Configuration](#configuration) below.

### Manual

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
2. If you do not have a `custom_components` directory (folder) there, you need to create it.
3. In the `custom_components` directory (folder) create a new folder called `volkswagen_we_connect_id`.
4. Download _all_ the files from the `custom_components/volkswagen_we_connect_id/` directory (folder) in this repository.
5. Place the files you downloaded in the new directory (folder) you created.
6. Follow the instructions under [Configuration](#configuration) below.

Using your HA configuration directory (folder) as a starting point you should now also have this:

```text
custom_components/volkswagen_we_connect_id/__init__.py
custom_components/volkswagen_we_connect_id/manifest.json
custom_components/volkswagen_we_connect_id/sensor.py
.. etc
```

##  Configuration 

It's important that you first use the app, connect the app to the car and use it at least once. 
After that enable the integration on the integration page in Home Assistant with your e-mail and password that you use to login into the app. Wait a couple of seconds and 1 or more devices (your cars) with entities will show up. 

## Tested Cars

* Volkswagen ID.3
* Volkswagen ID.4
* Cupra Born

## Requirements

Home Assistant Core *2022.7.0* or higher
