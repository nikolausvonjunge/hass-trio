# WIP to enhance Pontos Base in order to also read Syr Trio 2524
Will raise a PR on the original project once it works

# hass-pontos

[![GitHub Release](https://img.shields.io/github/release/sangvikh/hass-pontos.svg?style=flat)](https://github.com/sangvikh/hass-pontos/releases)
[![hassfest](https://img.shields.io/github/actions/workflow/status/sangvikh/hass-pontos/hassfest.yaml?branch=master&label=hassfest)](https://github.com/sangvikh/hass-pontos/actions/workflows/hassfest.yaml)
[![HACS](https://img.shields.io/github/actions/workflow/status/sangvikh/hass-pontos/validate.yaml?branch=master&label=HACS)](https://github.com/sangvikh/hass-pontos/actions/workflows/validate.yaml)

HACS integration for Hansgrohe Pontos

## Features

* Adds sensors for water consumption, water pressure, water temperature +++
* Opening/Closing of water valve
* Clearing alarms

## Installation

Installation via HACS is the recommended method

### HACS
Note: This integration is not yet included in HACS

1. Install HACS if you haven't already (see [installation guide](https://hacs.xyz/docs/configuration/basic/)).
2. Add custom repository https://github.com/sangvikh/hass-pontos as "Integration" in the settings tab of HACS.
3. Find and install Hansgrohe Pontos integration in HACS's "Integrations" tab.
4. Restart Home Assistant.
5. Go to your integrations page, click Add Integration and look for Hansgrohe Pontos.
6. Set up sensor using the IP address of your pontos, fixed ip is recommended.

### Manual installation

1. Clone repository or download as zip
2. Move the custom_components/hass_pontos folder to the custom_components directory of your Home Assistant installation
3. Restart Home Assistant.
5. Go to your integrations page, click Add Integration and look for Hansgrohe Pontos.
6. Set up sensor using the IP address of your pontos, fixed ip is recommended.

### Restful integration
The sensors and services can be added using restful integration. This is a bit limited and not recommended.

1. Copy the contents of restful.yaml into the configuration.yaml of your Home Assistant integration.
2. Find and replace IP address with the address of your Pontos.
3. Restart Home Assistant.

# TODO

- [x] Add services
- [x] Add water valve button
- [x] Add profile selection
- [ ] Read profile names
- [ ] Update sensors on service calls
- [x] Select active profile
- [ ] Include in HACS
