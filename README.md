# Call

## What is this?

A thing that parses `cty.dat` file from the [WSJT-X source code](https://wsjt.sourceforge.io/) into a JSON of regexes that can then be used on a silly single-serving website to check what country a callsign corresponds to.

The python code isn't particularly beautiful, but the main thing is getting to the actual JSON.

## Does it work?

Probably? Probably.

Our first attempt used [the ITU list of amateur callsign prefixes](https://www.itu.int/en/ITU-R/terrestrial/fmd/Pages/call_sign_series.aspx) which has some flaws (the code to process this is still under `bin/process_itu.ipynb` but isn't currently used).

Switching to the same file used by WSJT-X is probably more useful if you're looking up callsigns while doing FT8, but there is a lot more info in the `cty.dat` file that I'm essentially throwing away. Caveat emptor.

## Hasn't anyone else done this?

Probably.
