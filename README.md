# AB3AP_Random_Antenna_Calc
https://udel.edu/~mm/ham/randomWire/

Mike Markowski, ab3ap

mike.ab3ap@gmail.com

This script was posted on the web at the above link. Please visit this page to read the context and to understand what it's all about. I am still learning to work with it myself.

This is a minor modification of Mike AB3AP's endfed random wire length calculator that will output the results as a PNG file from the command line, instead of requiring an X server. I changed one line and added some setup instructions here; that is the extent of it.

## Mike AB3AP's Introduction:
```
This is a simple program that uses 468/f at all band edges of interest.  Red
boxes are drawn from edge to edge indicating spans of resonance for
particular frequencies.  At resonant frequency highest voltage is at the end
of an end fed and difficult to match.  If you have a modest antenna tuner,
avoid these areas.  If you have a capable tuner, -use- these areas since
signal is strongest.

Bands must be in: 160,80,60,40,30,20,17,15,12,10,6 m
```

## Setup is easy:

Ensure you have Python, Pip and Venv installed.

Clone this repo to your local machine, or, open it in a CodeSpace.

``python3 -m venv venv``

``source venv/bin/activate``

``pip install -r requirements.txt``

You're now good to go.

## Mike AB3AP's Instructions:

```
Usage example up to half wavelength:
  endfed.py 40 20 15 10

Usage example up to full wavelength:
  endfed.py -f 40 20 15 10

or to generate the same in meters:
  endfed.py -m 40 20 15 10

and a graph pops up.  Red areas indicate highest voltage at end of wire.
Mouse cursor can be moved on image to read values.  Image can also be saved
as a png.

Mike Markowski, ab3ap
mike.ab3ap@gmail.com
March 2024
```
* Note that this version will only save as a PNG


