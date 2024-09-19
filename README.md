# Sketchbook_Starter_Kit_V2.0 with Some Notes
===========================

## Prerequiste

This journey begins when one day I got a free Grove Starter Kit (Gen2).

My studying mates are my Macbook, Arduino Uno R4, and using the [official CLI](https://arduino.github.io/arduino-cli/1.0/) for operation. 

## Run a program

1. Compile a sketch

```
$ arduino-cli compile -b arduino:renesas_uno:minima scanner/
```
with a library

2. Upload a sketch

```
$ arduino-cli upload -p /dev/cu.usbmodem14401 --fqbn arduino:renesas_uno:minima scanner
```

3. Others: install a package



## Reset the board 

Based on the [official documents](https://support.arduino.cc/hc/en-us/articles/5779192727068-Reset-your-board), 

single click -> stop the power shortly and rerun the stored sketch, memory is cleaned.

double click -> Go to boatloader mode: waiting a new sketch coming, actually the stored sketch is still there.

By uploading a clean sketch


