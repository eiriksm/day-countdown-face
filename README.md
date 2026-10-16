# day-countdown-face
A [Second Movement](https://github.com/joeycastillo/second-movement) watch face that counts down the number of days to a set of events.

Events are read from `days.txt` on the watch filesystem, one `Label|unix timestamp` per line:

```
# Summer vacation, 1 July 2027
VAC|1814400000
```

Without the file it counts down to THAI on 1 February 2027. The events are followed by XMAS, which counts down to the next Christmas Eve.

ALARM cycles through the events, holding ALARM shows the date of the event as YYMMDD.

## Installation

Install with composer:

```
composer require eiriksm/day-countdown-face:dev-main
```

The face depends on the Second Movement firmware headers (`movement.h`, `watch.h` and friends), so it only builds as part of the firmware.
