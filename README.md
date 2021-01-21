# football-data

This repository contains data-sets about the results of *football* (or *soccer* if you are from the US) games in various championships worldwide.


## Path format

Files are organised in directories and the name of them follows the schema below.

```
${DECADE}/${SEASON}/${COUNTRY}.${TIER}.${FORMAT}
```

Where

* `DECADE` is the decade the season belongs to
* `SEASON` is the season in format `${start_year}-${end_year}` or `${year}` if the championship is a single-year one
* `COUNTRY` is the name of the country (all lowercase)
* `TIER` is the number of the tier (1 is the highest)
* `FORMAT` is about how the information is stored (*CSV* by default)

## File format

By default the information is stored in [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) format. Fields are separated by `,` character. The first line is the header.

Files contain the following fields.

* `round` - the number or name of the match day
* `date` - the starting time and/or the date of the game (`Month/Day/Year Hour:Minutes`)
* `home_team` - the name of the home team
* `away_team` - the name of the away team
* `home_score` - the number of goals the home team scored (or empty string if the game hasn't been played yet)
* `away_score` - the number of goals the away team scored (or empty string it the games hasn't been played yet)
* `stadium` - the venue where the game was played in
* `stage` - the name of the stage or an empty string in case of a single-staged championship
