# Sketchbook_Starter_Kit_V2.0 with Some Notes

## Prerequiste

This journey begins when one day I got a free Grove Starter Kit (Gen2).

My studying mates are my Macbook, Arduino Uno R4, and using the [official CLI](https://arduino.github.io/arduino-cli/1.0/) for operation. All steps are following the guides in official website.

## Install the core/platform

It is necessary to install the package, called the **core**, in arduino ecosystem.
This software pack is based the board, to install the accurate one on your PC, first check your board.


### Check the board

```
// Linked the board to PC
$ arduino-cli board list
Port                            Protocol Type              Board Name            FQBN                       Core
/dev/cu.usbmodem14101           serial   Serial Port (USB) Arduino UNO R4 Minima arduino:renesas_uno:minima arduino:renesas_uno 
```

In the label core, you can now know the name is `arduino:renesas_uno`.
**Port** and **FQBN** is also essential parameters when we run the promgram, would need to check frequently if you forget.

Then, installing the core by following command:

```
$ arduino-cli core install $CORE_NAME

// Verified the installed cores
$ $ arduino-cli core list
ID                  Installed Latest Name
arduino:renesas_uno 1.2.0     1.2.0  Arduino UNO R4 Boards
```


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


