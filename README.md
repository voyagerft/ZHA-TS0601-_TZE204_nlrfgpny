<img width="1027" alt="Schermata 2024-03-22 alle 10 09 30" src="https://github.com/voyagerft/ZHA-TS0601-_TZE204_nlrfgpny/assets/1532553/6cb15478-474d-4d90-8485-2797c099b512">
# ZHA-TS0601-_TZE204_nlrfgpny
Problem: 
Siren Tuya TS0601-_TZE204_nlrfgpny does not expose entities on ZHA

Solution,custom quirks: (only on/off)

Home Assistant
create a "custom_zha_quirks" folder in config/
add the following code to configuration.yaml
zha:
enable_quirks: true
custom_quirks_path: config/custom_zha_quirks/

upload the attached files to the config/custom_zha_quirks/ folder
init.py and ts601_siren.py

Delete the siren from the Zigbee devices, if previously configured and restart Home Assistant

Perform the Zigbee pairing again with the siren and the switch will come out

I remind everyone that it works exclusively with TS0601 _TZE204_nlrfgpny

If you help me I could insert volume level and melody
