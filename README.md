# Bluetooth controlled mBot SoccerBot

Using the [mBot Bluetooth version](http://www.makeblock.cc/mbot/) and
[mBot NodeBots](https://github.com/Makeblock-official/mbot_nodebots/blob/master/README.md).

## Getting Started

* Install Node 4
* Install USB [driver](https://github.com/Makeblock-official/mbot_nodebots/tree/master/driver) for your platform

### Install Dependencies

```
  git clone https://github.com/EmergingTechnologyAdvisors/mbot-soccer
  cd mbot-soccer
  npm i
```  

### Install Firmware (USB)

* Connect the USB cable
* Install the USB Firmata:

```
  interchange install git+https://github.com/Makeblock-official/mbot_nodebots -a uno --firmata=bluetooth
```

### Install Firmware (Bluetooth)

* Remove the Bluetooth module from the mBot
* Connect the USB cable
* Install the Bluetooth Firmata:

```
  interchange install git+https://github.com/Makeblock-official/mbot_nodebots -a uno --firmata=usb
```

* Restart the mBot with the Bluetooth module installed again
* Pair the MakeBlock Bluetooth module (device Bluetooth settings)

## Running the Code

```
  node eg/controls.js /dev/tty.Makeblock-ELETSPP
```
* Control the mBot using the right keyboard keys and spacebar
