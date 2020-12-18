# Home Assistant Blueprints
This repo contains my Home Assistant Blueprints.
As you might see, I heavily depend on light profiles, as this is easier to main, a light profile contains color (x,y), brightness and transition. You can image adding all these parameters to a blueprint will make them more complex.

If you think anything is wrong with the blueprint, feel free to create an issue.

## Changelog
**V2 - December 18, 2020**
 - Rename all blueprints, making them more understandable, also added a better description to all of them.
 - motion-activated_light_profiles.yaml
	 - Replaces brightness drop by light profiles
 - zigbee2mqtt_hue_smart_button_bed_light_button.yaml
	 - Added day/night time
	 - Added light profile for day/night time

**V1 - December 17, 2020**
- Hue scenes in light_profiles.csv (create this file next to your configuration.yaml)
- Motion-activated Light, like Hue - _Drop brightness when no movement is detected, so the light doesn't turn off fully_
- MQTT - Hue smart button (press and hold) - _Trigger action(s) when pressing or holding the Hue smart button_
- MQTT - Hue smart button (press and hold) bedlampje - _Similar to the previous, automation I use often for a smart button on the nightstand (press night stand lamp on/off, hold ceiling light on/off)_