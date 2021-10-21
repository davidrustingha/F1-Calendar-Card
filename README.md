# F1-Calendar-Card
A card for upcoming F1 events

-------------------------------------------------------------
INSTALLATION
-------------------------------------------------------------
To get this card working there's a couple of components you need.

- Google Calendar integration: https://www.home-assistant.io/integrations/calendar.google/
- F1 Calendar by RaceFans: https://calendar.google.com/calendar/embed?src=ekqk1nbdusr1baon1ic42oeeik%40group.calendar.google.com&ctz=Europe/London
- Custom Template Entity Row: https://github.com/thomasloven/lovelace-template-entity-row
- Patience

-------------------------------------------------------------
ORDER OF INSTALLING
-------------------------------------------------------------
To minimize errors in your log file install the components in the following order
- Google Calendar Integration
- Add F1 calendar to HA (use the entry in the google_calendar.yaml file)
- Install Template Entity Row
- Add card.yaml to dashboard

-------------------------------------------------------------
EXAMPLE
-------------------------------------------------------------
![alt text](https://github.com/davidrustingha/F1-Calendar-Card/blob/main/example_f1_card.jpg)
