# Xiaomi Five UV Lamp

This is a custom component for home assistant to add support of Xiaomi Five UV lamp, as a workaround because it isn't supported by Miio/HA out of the box yet.

Please follow the instructions on [Retrieving the Access Token](https://home-assistant.io/components/xiaomi/#retrieving-the-access-token) to get the API token to use in the configuration.yaml file.

## Install

You can install this custom component by adding this repository ([https://github.com/gamaraan/xiaomi_five_uv_lamp_component](https://github.com/gamaraan/xiaomi_five_uv_lamp_component/)) to [HACS](https://hacs.xyz/) in the settings menu of HACS first. You will find the custom component in the integration menu afterwards, look for 'Xiaomi Five UV Lamp'. Alternatively, you can install it manually by copying the custom_component folder to your Home Assistant configuration folder.

## Setup

```yaml
# configuration.yaml

switch:
  - platform: xiaomi_five_uvc_lamp
    name: <entity name>
    host: <Lamp IP address>
    token: <Token>
