# Geoweather

Geolocated weather forecasts using the power of the World Wide Web.

## Problem

Installing a [spyware-ridden application](https://www.nytimes.com/2019/01/03/technology/weather-channel-app-lawsuit.html) on your telephone is dumb. When the only function of that application is to fetch and display data from the internet, installing it is even dumber. We have web browsers that can accomplish that (minus most of the spyware).

You can use your browser to bookmark your favorite weather forecasting site but, after loading, most sites require a second click to identify your current location. That is one too many clicks.

## Solution

Geoweather is a simple HTML web page which uses the [Javascript geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation) to get your current coordinates, use those coordinates to build a forecast URL for your location, and redirect you to the URL.

## Use

Upload the HTML page someplace on the Information Super Highway, or [use mine](https://havenaut.net/weather/). Bookmark the URL and [add the bookmark to your home screen](https://blog.mozilla.org/theden/2012/12/13/create-a-mobile-shortcut-on-your-home-screen/). You can now get geolocated weather forecasts with a single click.

Bonus: the forecast service doesn't have permission to locate you.

## Supported Forecasts

The default forecast service is the [National Weather Service](https://www.weather.gov/). If your screen width is less than 800px, you'll be directed to [the mobile version](https://mobile.weather.gov/).

Append the `?darksky` querystring to be redirected to [Dark Sky](https://darksky.net/).

Append the `?windy` querystring to be redirected to [Windy](https://www.windy.com/).

## Tips

If they detect that you are on a mobile device, both Both Dark Sky and Windy will waste valuable screen real estate with elements that ask you to install their mobile application. Use the [uBlock Origin element picker](https://github.com/gorhill/uBlock/wiki/Element-picker) to eliminate this waste.
