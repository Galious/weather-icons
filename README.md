# weather-icons

Collections of weather icons suitable for epaper displays and compatible with free APIs.

## Goal
My main objective is to be able to use my epaper display (SeeedStudio reTerminal E1001) with sources of weather data other than the built-in one included in the no-code Sensecraft HMI.
I want to be able to use third-party free APIs to get the weather data, and display appropriate icons. This no-code environment has many restrictions, so the suitable icons sets also have to meet specific criteria. 

## Compatible APIs
The first objective is to support the following weather APIs offering a free tier for home usage:
* Pirate Weather (up to 10,000 API requests per month in the free plan, amounting to 320 per day, more than 13 per hour)
* Visual Crossing (up to 1,000 API requests per day in the free plan, amounting to 41 per hour)

## Devices
The reference epaper device used to test these icons and API is:
* reTerminal E1001 (7.5" monochrome epaper display configured using Sensecraft HMI)

Information will be given regarding how to configure a Sensecraft dashboard to use these APIs and icons.

## Icon naming
Both Pirate Weather and Visual Crossing use a naming scheme based on the defunct weather app Dark Sky, bought by Apple in 2020.<br>
The Dark Sky API was shut down on March 31, 2023, and has been replaced by Apple's WeatherKit API that is more difficult to implement and does not use the same namings for weather conditions.<br>
Information about the Dark Sky API can still be found in a [capture made by the Internet Archive](https://web.archive.org/web/20200723173936/https://darksky.net/dev/docs).<br>
Pirate Weather and Visual Crossing aim at offering a replacement for the Dark Sky API. See [this blog post by Visual Crossing](https://www.visualcrossing.com/resources/blog/how-to-replace-the-dark-sky-api-using-the-visual-crossing-timeline-weather-api/) and information in the [Pirate Weather documentation](https://pirateweather.net/en/latest/API/).

### Dark Sky (not available any more)
Here are all the possible icon names that were returned when calling the Dark Sky API:<br>
icons codes : clear-day, clear-night, rain, snow, sleet, wind, fog, cloudy, partly-cloudy-day, partly-cloudy-night

### Pirate Weather
Here are all the possible icon names returned when calling the Pirate Weather API:<br>
clear-day, clear-night, thunderstorm, rain, snow, sleet, wind, fog, cloudy, partly-cloudy-day, partly-cloudy-night<br>
[Link to the relevant Pirate Weather documentation](https://pirateweather.net/en/latest/API/)

### Visual Crossing
Here are all the icon names returned when calling the Visual Crossing API using the default (smallest) icon set:<br>
clear-day, clear-night, rain, snow, wind, fog, cloudy, partly-cloudy-day, partly-cloudy-night

### Comparison

| Icon codes          | Dark Sky     | Pirate Weather | Visual Crossing |
| ------------------- | ------------ | -------------- | --------------- |
| clear-day           | Used         | Used           | Used            |
| clear-night         | Used         | Used           | Used            |
| rain                | Used         | Used           | Used            |
| snow                | Used         | Used           | Used            |
| wind                | Used         | Used           | Used            |
| fog                 | Used         | Used           | Used            |
| cloudy              | Used         | Used           | Used            |
| partly-cloudy-day   | Used         | Used           | Used            |
| partly-cloudy-night | Used         | Used           | Used            |
| sleet               | Used         | Used           | **Not used**    |
| thunderstorm        | **Not used** | Used           | **Not used**    |

In  order to properly support Pirate Weather, all the above icons will be included, even if *thunderstorm* was not in Dark Sky.

## Icon formats
At first, only SVG will be offered. Depending on how it goes with testing, maybe raster icon sets will also be offered in different sizes.<br>
Since Sensecraft do not handle correctly cycling icons of multiple aspect ratios, all icons will be square.

## Alternatives
For the moment, I did not manage to find an icon set that ticks all the boxes:
* icons available using an individual URL for each one
* square format
* black and white
* names following the Dark Sky naming pattern
* if possible, SVG format

You can look at the following projects:
* [Visual Crossing's WeatherIcons](https://github.com/visualcrossing/WeatherIcons/tree/main/SVG/2nd%20Set%20-%20Monochrome) (4 different sets available) : not square, no icon for *thunderstorm* (there is *thunder* instead)
* [John Graham-Cumming's eink-weather](https://github.com/jgrahamc/eink_weather/tree/main/icons/svgs) : no icon for *thunderstorm*
* [Paul Reed's weather icons lite](https://github.com/Paul-Reed/weather-icons-lite/tree/master/images) : not black and white, names not following the Dark Sky naming pattern, no SVG
* [Erik Flowers'Weather Icons](https://github.com/erikflowers/weather-icons/tree/master/svg) : names not following the Dark Sky naming pattern

I have not found an icon set designed specifically for Pirate Weather yet.

