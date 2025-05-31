# Call

## What is this?

A thing that parses [the ITU list of amateur callsign prefixes](https://www.itu.int/en/ITU-R/terrestrial/fmd/Pages/call_sign_series.aspx) into a JSON of regexes that can then be used on a silly single-serving website to check what country a callsign corresponds to.

The python code isn't particularly beautiful, but the main thing is getting to the actual JSON.

## Does it work?

Probably? A flaw of the ITU data is that it does not include numeric ranges, so even the callsign prefix "M7" (the one I currently hold!) can't be identified by default.

As a workaround, we check if the list of countries for each single, double and triple letter prefix is unique - if so, we assume it is assigned the whole range.

## Hasn't anyone else done this?

Probably.
