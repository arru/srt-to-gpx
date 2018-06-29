DJI-style .SRT to GPX converter
===============================

### What it does
Some DJI drones provide the option for generating SRT (subtitle) files accompanying movie files recorded by the drone. When viewed in a video player these will elegantly annotate the video with GPS position and other metadata. If one wishes to view this flight log on a map or do other geographical post-processing, a more established GPS log format like GPX has much better support in 3rd party software. This script lets you do straightforward conversion from the former to the latter.

### Features
* Converts .SRT files containing GPS coordinates to GPX files 
* Preserves non-geographic metadata (such as exposure level and air pressure, varies by DJI drone model) in the `extensions` tag under `dji:` namespace. While this option will keep the extra metadata included in the SRT files during conversion, it won't be of much use unless you plan to write custom software for analyzing this data. For more common use cases it can be left off which will result in smaller GPX files.
* Tested with Mavic Pro and Inspire SRT files
* Pure Python 3 – no funny stuff

### Requirements
* Python 3.2

Usage
-----
Please run `python srt_to_gpx.py -h` for usage guidance.

License
-------
This piece of software is copyright © 2018 Arvid Rudling. Licensed under the Revised BSD License, se LICENSE file

DJI, Inspire and Mavic Pro are trademarks of Dà-Jiāng Innovations Science and Technology Co. Ltd.
All other trademarks are the property of their respective owners.

The software is developed without any affiliation to the mentioned vendors.
