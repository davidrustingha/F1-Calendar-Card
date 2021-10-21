# F1-Calendar-Card
A card for upcoming F1 events
Featuring support for Sprint Race weeks and normal race weeks
-------------------------------------------------------------
INSTALLATION
-------------------------------------------------------------
To get this card working there's a couple of components you need.

- Google Calendar integration: https://www.home-assistant.io/integrations/calendar.google/
- F1 Calendar by RaceFans: https://calendar.google.com/calendar/embed?src=ekqk1nbdusr1baon1ic42oeeik%40group.calendar.google.com&ctz=Europe/London
- Custom Template Entity Row: https://github.com/thomasloven/lovelace-template-entity-row
- Custom Text Divider Row: https://github.com/iantrich/text-divider-row
- Patience

-------------------------------------------------------------
ORDER OF INSTALLING
-------------------------------------------------------------
To minimize errors in your log file install the components in the following order
- Google Calendar Integration
- Add F1 calendar to HA (use the entry in the google_calendar.yaml file)
- Add template sensors to your config
- Install Template Entity Row & Text Divider Row
- Add card.yaml to dashboard
- Enjoy!

-------------------------------------------------------------
WHERE TO PLACE TEMPLATE SENSORS
-------------------------------------------------------------
The card relies highly on the template sensors created in step 3 of the installation. People who use !include statements in their configuration.yaml file will be able to paste this directly inside their yaml file, or download the template_sensor.yaml file to their template sensor folder (If you want to learn more about this: https://www.home-assistant.io/docs/configuration/splitting_configuration/)

For people who want to put this inside the configuration.yaml file you need to do the following.

- Add template sensor entry to the config file:
````
template:
  - sensor:
````
- Copy the content inside template_sensor.yaml file and paste under the '- sensor:' entry
- Select all of the code you just copied and hit tab to indent the code under the '- sensor:' entry (works if you use the file editor addon, and also if you use the VSCode addon)
- Check config and reload template entities.
-------------------------------------------------------------
LANGUAGE
-------------------------------------------------------------
Want to use the card in a diffrect language? The following adjustments have to be made

- Change the days and months in the template sensor
- Change the text in the card

And you're done

-------------------------------------------------------------
EXAMPLE
-------------------------------------------------------------
![alt text](https://github.com/davidrustingha/F1-Calendar-Card/blob/main/example_f1_card.jpg)

-------------------------------------------------------------
BUGS OR FEATURE REQUESTS
-------------------------------------------------------------
It will probably happen that you run into some bugs. Please raise an issue for those, so I can get the card as perfect as possible. The same goes for feature requests. You can always add the and if/when I find the time and answer I will implement it!
