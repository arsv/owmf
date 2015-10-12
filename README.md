OpenWeatherMap Forecast, plaintext output with some formatting.
See http://openweathermap.org/forecast

```
# owmf Lviv
Lviv, UA

2014-11-23 Sun
    17    +1  overcast clouds   NN >>
    20    -0  broken clouds     NE >>
    23    -2  scattered clouds  EE >>
2014-11-24 Mon
    02    -3  broken clouds     EE >>
    05    -3  scattered clouds  SE >>>
    08    -5  few clouds        SE >>>
    11    -3  sky is clear      SE >>>>
    14    +1  sky is clear      SE >>>>> >
```

The script should work both with Python 2 and Python 3.

Inspired by https://github.com/HalosGhost/shaman

Note starting from Oct 2015 OWM _requires_ valid API key for any request.
To get API key, register at http://home.openweathermap.org/users/sign_up,
take the key from your profile page http://home.openweathermap.org/ and
run owmf once with -s and +KEY arguments:

    owmf +00000000000000000000000000000000 -s [your-city]

The key will be saved in ~/.config/owm.json. Further calls need no +KEY.
