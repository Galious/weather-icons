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

Both Pirate Weather and Visual Crossing use a naming scheme based on the defunct weather app Dark Sky, bought by Apple in 2020.<br>
The Dark Sky API was shut down on March 31, 2023, and has been replaced by Apple's WeatherKit API.<br>
Information about the Dark Sky API can still be found in a [capture made by the Internet Archive](https://web.archive.org/web/20200723173936/https://darksky.net/dev/docs).<br>
Pirate Weather and Visual Crossing aim at offering a replacement for the Dark Sky API. See [this blog post by Visual Crossing](https://www.visualcrossing.com/resources/blog/how-to-replace-the-dark-sky-api-using-the-visual-crossing-timeline-weather-api/) and information in the [Pirate Weather documentation](https://pirateweather.net/en/latest/API/).

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

