# NPR One CLI for the NTC CHIP

This is a simple command line based NPR One client for OS X and Linux. A tutorial with setup instructions can be found [in the Adafruit Learning System](https://learn.adafruit.com/raspberry-pi-zero-npr-one-radio), not everything applies this fork does not include the code to interact with the capacitive touch as inclusion of that code would not allow the original Adafruit version to run on the NTC CHIP the target device for this fork. The MAC OSX instructions are left intact as it is likely to work fine on any device that the Adafruit original version does.

## Interface
This version has been tweaked to work with a 10 key numeric pad and has been tested on the NTC CHIP.

## Installation

This package requires the latest stable version of [Node.js](https://nodejs.org) (v6.0 or higher due to the use of es6).

```sh
$ node -v
v6.2.0
```

Install `mplayer` on OS X using [homebrew](http://brew.sh/):

```
$ brew install mplayer
```

Install `mplayer` on Linux:

```
$ sudo apt-get install -y mplayer
```

Make sure you have the latest stable [node.js](https://nodejs.org/en/) installed (6.0 or higher), and then run:

```
npm install -g npr-one
```

## Usage

Sign into the [NPR Dev Console](http://dev.npr.org/), create a new app, and use your App ID & Secret to authorize the CLI. The audio player will save your authorization and begin playing.

```
$ npr-one

\\\\\\\\\\\\\\\\\\\\\\\\\\\>>>>>>>>>>>>>>>>>>>>>>>>>> \\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\>>>>>>>>>>>>>>>>>>>>>>>>>> \\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\>>\\\\\\\\\\\\>>>>>>>>>>>>>>>>>>>>>>>>>> \\\\\\\\\\\\\\>>>\\\\\\\\\
\\\\\\\           >\\\\\\\\>>>>>>>          \>>>>>>>> \\\\\\\\         (\\\\\\\\
\\\\\\\   .>>>>=   \\\\\\\\>>>>>>>   =>>>>    >>>>>>> \\\\\\\\    (>>>>\\\\\\\\\
\\\\\\\   )\\\\\   (\\\\\\\>>>>>>>   >>>>>>   )>>>>>> \\\\\\\\   .\\\\\\\\\\\\\\
\\\\\\\   )\\\\\   (\\\\\\\>>>>>>>   >>>>>>   )>>>>>> \\\\\\\\   )\\\\\\\\\\\\\\
\\\\\\\   )\\\\\   (\\\\\\\>>>>>>>   >>>>>\   >>>>>>> \\\\\\\\   )\\\\\\\\\\\\\\
\\\\\\\   )\\\\\   (\\\\\\\>>>>>>>          ->>>>>>>> \\\\\\\\   )\\\\\\\\\\\\\\
\\\\\\\>>>>\\\\\>>>>\\\\\\\>>>>>>>   >>>>(>>>>>>>>>>> \\\\\\\\>>>>\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\>>>>>>>   >>>>>>>>>>>>>>>> \\\\\\\\\\\\\\\\\\\\\\\\\\
\\\\\\\\\\\\\\\\\\\\\\\\\\\>>>>>>>===>>>>>>>>>>>>>>>> \\\\\\\\\\\\\\\\\\\\\\\\\\

[downloaded] WYPR FM
[downloaded] NPR thanks our sponsors
[playing] WYPR FM
[downloaded] Welcome To Czechia: Czech Republic Looks To Adopt Shorter Name
[downloaded] Belgian Transport Minister Resigns Over Airport Security Debate
[downloaded] Tax Season
[downloaded] Adapting To A More Extreme Climate, Coastal Cities Get Creative
[downloaded] NPR thanks our sponsors
```

### Keyboard Controls

```
Return / Enter   play/pause
↑       volume up
↓       volume down
←       rewind 15 seconds
→       skip to the next story
i       mark as interesting (only if you have a full keyboard attached, there was an issue with keypress library used that does not accept input from numeric keys or any other key it consideres 'undefined'.
```

## License

Copyright (c) 2016 Adafruit Industries. Licensed under the MIT license.

The NPR logo is a registered trademark of NPR used with permission from NPR.  All rights reserved.
