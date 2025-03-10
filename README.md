`ggz-tools` is a set of tools to handle [Garmin](https://www.garmin.com/en-US/)'s [GGZ files](https://support.garmin.com/en-US/?faq=VtaaU06nPHAihnOIcMmXyA).

GGZ files store the information of a huge number of [Geocaches](https://en.wikipedia.org/wiki/Geocaching) in a format which allows some Garmin handheld [GPS](https://en.wikipedia.org/wiki/Global_Positioning_System) receivers to quickly display them. 

Note that this work is not related to or endorsed by Garmin.

## How to install
### Prerequisites
`ggz-tools` is written in Python, so you will need to install Python 3. If you need this tool then most likely you are running on GNU/Linux and Python will already be installed.

Otherwise you can follow [these instructions](https://wiki.python.org/moin/BeginnersGuide/Download).

### Steps
1. Download [all files as zip](https://github.com/brandl-muc/ggz-tools/archive/refs/heads/master.zip) 
1. Unzip to a directory
1. Make both tools executable: `chmod +x ggz_verify.py gpx2ggz.py`
1. Optional: Add the directory to your path or add links to a directory in your path

## Usage
### gpx2ggz
This tool converts [gpx files](https://en.wikipedia.org/wiki/GPS_Exchange_Format) into a single GGZ file.

Simply pass the input gpx files as positional arguments and the output ggz file as last positional argument:
`gpx2ggz.py [input.gpx]... output.ggz`

#### How to store Pocket Queries on your Garmin GPSr
1. run your [Pocket Queries](https://www.geocaching.com/pocket/) on [geocaching.com](https://www.geocaching.com)
1. download the resulting zip files
1. unzip them to a directory
1. create the GGZ by running e.g. `gpx2ggz *.gpx output.ggz`
1. store the GGZ file in the `/Garmin/GGZ` directory of your Garmin device

This workflow worked as of 2025-03-10.

### ggz-verify
I have not used this tool so far and cannot provide information for now.

## License

This tool is available to anybody free of charge, under the terms of BSD 3-clause license (see [LICENSE.md](./LICENSE.md)).

This work is based on [ggz-tools](https://github.com/rsaxvc/ggz-tools) by Richard Allen which was published without an explicit license. 
