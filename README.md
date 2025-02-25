# Wheatly API

Fetch weather data:
> `http/GET https://hacked-zg4z.onrender.com/?weather=[year]`

This will return a large JSON object including a weekly set of weather conditions up till the end of the year.

Valid years are 2021 through to 2024.

Set/Get the colour for the field's LEDs on the Pi Sense HAT:
> `http/GET https://hacked-zg4z.onrender.com/colour?[id]=[colour]`

The entry `id` is the fields's LEDs you want to change the colour of, and `colour` is the state of the LED.

Following on from this, you can get the colours via:

> `http/GET https://hacked-zg4z.onrender.com/?connection=getc`

This will return 6 values, with each field's colour. These numbers are then interpreted by the Raspberry Pi as a different pre-set colour.
