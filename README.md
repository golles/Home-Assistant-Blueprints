# Home Assistant Blueprints

[![BuyMeCoffee][buymecoffeebadge]][buymecoffee]

This repo contains my Home Assistant Blueprints.
As you might see, I heavily depend on light profiles, as this is easier to maintain, a light profile contains color (x,y), brightness and transition. You can image adding all these parameters to a blueprint will make them more complex.

If you think anything is wrong with the blueprint, feel free to create an issue.

## Changelog
**May 8, 2022**
	- motion-activated_scenes.yaml
  	- Since the new Philips Hue integration all the Hue scenes are exposed to Home Assistant. From this moment I switched from using light profiles to scenes. This blueprint is created from scratch with a new option to turn lights off when the illuminance is getting above a certain treshold.

**October 10, 2021**
  - motion-activated_light_profiles.yaml
	  - Either check if the illuminance is below the threshold or when the light is on. The Hue motion sensor picks up illuminance quickly and therefor the automation didn't restart due no longer under the threshold.

**July 29, 2021**
	- zigbee2mqtt_aqara_magic_cube.yaml
		- New blueprint for the Aqara Magic Cube.

**May 18, 2021**
 - door-window-climate-control.yaml
	 - Added simple blueprint to switch off a climate entity when a door opens.
 - zigbee2mqtt_hue_smart_button_press_and_hold_actions.yaml
   - Added new blueprint for the hue smart button with press and hold actions.
 - zigbee2mqtt_xiaomi_switch.yaml
   - Added release action.

**March 6, 2021**
 - motion-activated_light_profiles.yaml
	 - Check if a light is still on when dimming it, this fixes an issue that when a light is turned of by the user is not turned on by the automation in dimmed profile.

**Februari 6, 2021**
 - motion-activated_light_profiles.yaml
	 - Adding a cool down period
 - zigbee2mqtt_hue_smart_button_press_and_hold_actions.yaml
	 - Replaced with zigbee2mqtt_xiaomi_switch.yaml

**December 18, 2020**
 - Rename all blueprints, making them more understandable, also added a better description to all of them.
 - motion-activated_light_profiles.yaml
	 - Replaces brightness drop by light profiles
 - zigbee2mqtt_hue_smart_button_bed_light_button.yaml
	 - Added day/night time
	 - Added light profile for day/night time

**December 17, 2020**
- Hue scenes in light_profiles.csv (create this file next to your configuration.yaml)
- Motion-activated Light, like Hue - _Drop brightness when no movement is detected, so the light doesn't turn off fully_
- MQTT - Hue smart button (press and hold) - _Trigger action(s) when pressing or holding the Hue smart button_
- MQTT - Hue smart button (press and hold) bedlampje - _Similar to the previous, automation I use often for a smart button on the nightstand (press night stand lamp on/off, hold ceiling light on/off)_

[buymecoffee]: https://www.buymeacoffee.com/golles
[buymecoffeebadge]: https://img.shields.io/badge/buy%20me%20a%20coffee-donate-yellow.svg?style=for-the-badge
