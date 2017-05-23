
<!-- README.md is generated from README.Rmd. Please edit that file -->
lubridate
=========

[![Build Status](https://travis-ci.org/tidyverse/lubridate.svg?branch=master)](https://travis-ci.org/tidyverse/lubridate) [![Coverage Status](https://codecov.io/gh/tidyverse/lubridate/branch/master/graph/badge.svg)](https://codecov.io/gh/hadley/devtools) [![CRAN RStudio mirror downloads](http://cranlogs.r-pkg.org/badges/lubridate)](https://cran.r-project.org/package=lubridate) [![Development version](https://img.shields.io/badge/devel-1.6.0.9000-orange.svg)](https://github.com/tidyverse/lubridate) [![CRAN version](http://www.r-pkg.org/badges/version/lubridate)](https://cran.r-project.org/package=lubridate)

Date-time data can be frustrating to work with in R. R commands for date-times are generally unintuitive and change depending on the type of date-time object being used. Moreover, the methods we use with date-times must be robust to time zones, leap days, daylight savings times, and other time related quirks, and R lacks these capabilities in some situations. Lubridate makes it easier to do the things R does with date-times and possible to do the things R does not. Specifically, lubridate provides:

-   a set of intuitive date-time related functions that work the same way for all common date-time classes (including those from `chron`, `timeDate`, `zoo`, `xts`, `its`, `tis`, `timeSeries`, `fts`, and `tseries`)

-   easy and very fast parsing of date-times: `ymd()`, `ymd_hms`, `dmy()`, `dmy_hms`, `mdy()`, ...

-   simple functions to extract and modify components of a date-time, such as years, months, days, hours, minutes, and seconds: `year()`, `month()`, `day()`, ...

-   helper functions for handling time zones: `with_tz()`, `force_tz()`

Lubridate also expands the type of mathematical operations that can be performed with date-time objects. It introduces three new time span classes borrowed from <http://joda.org>.

-   `durations`, which measure the exact amount of time between two points

-   `periods`, which accurately track clock times despite leap years, leap seconds, and day light savings time

-   `intervals`, a protean summary of the time information between two points
