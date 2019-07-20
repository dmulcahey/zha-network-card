# ZHA Network Card
Custom Lovelace card that displays ZHA network and device information

This is a modified version of https://github.com/custom-cards/flex-table-card This implementation leverages the ZHA websocket API to get ZHA device information instead of using hass.states

## Installation (quick & "dirty")

* Find your homeassistent directory containing your configuration (let's say `~/.homeassistant/`)
* Change into `~/.homeassistant/www` (create the `www` directory, if it is not existing, you then might have to restart HA)
* `$ wget https://raw.githubusercontent.com/dmulcahey/zha-network-card/master/zha-network-card.js` downloads the `.js` file directly where it should reside
* Finally, add the following on top of your UI Lovelace configuration (means either via Config UI or .yaml)
``` yaml
resources:
  - type: js
    url: /local/zha-network-card.js
```
* Verify that it works with one of the examples below

## Configuration

See https://github.com/custom-cards/flex-table-card for configuration options.
