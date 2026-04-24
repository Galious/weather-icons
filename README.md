# weather-icons
Collections of weather icons suitable for epaper displays and compatible with free APIs

## Compatible APIs
First objective is to support the following weather APIs offering a free tier for home usage:
* Pirate Weather
* Visual Crossing

## Devices
The reference epaper device used to test these icons and API is:
* reTerminal E1001 (7.5" monochrome epaper display configured using Sensecraft HMI)

Information will be given regarding how to configure a Sensecraft dashboard to use these APIs and icons.

## Icon naming
### Pirate Weather
Here are all the possible icon names returned when calling the Pirate Weather API:<br>
clear-day, clear-night, thunderstorm, rain, snow, sleet, wind, fog, cloudy, partly-cloudy-day, partly-cloudy-night<br>
[Link to the relevant Pirate Weather documentation](https://pirateweather.net/en/latest/API/)

### Visual Crossing
Here are all the icon names returned when calling the Visual Crossing API using the default (smallest) icon set:<br>
clear-day, clear-night, rain, snow, wind, fog, cloudy, partly-cloudy-day, partly-cloudy-night

### Comparison

| Icon codes          | Pirate Weather | Visual Crossing |
| ------------------- | -------------- | --------------- |
| clear-day           | Used           | Used            |
| clear-night         | Used           | Used            |
| rain                | Used           | Used            |
| snow                | Used           | Used            |
| wind                | Used           | Used            |
| fog                 | Used           | Used            |
| cloudy              | Used           | Used            |
| partly-cloudy-day   | Used           | Used            |
| partly-cloudy-night | Used           | Used            |
| thunderstorm        | Used           | **Not used**    |
| sleet               | Used           | **Not used**    |

