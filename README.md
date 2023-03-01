# µVox

Is an open source smart power audio amplifier, released under CC-BY-SA License.
Powered by the Merus MA12070P Amplifier 🔊 & an ESP32 µC. 

- Designed in Denmark 🇩🇰 - proudly challenging the status quo of the wellestablished Danish Audio Industry. 

This repository contains the KiCAD PCB project files for µVox. **Requires KiCAD 6.0**

## Goals

- To provide a truly plug and play amplifier solution to **any** speaker. 
- Allow **anybody** have a truly open audio streaming solution.
- Let this platform be flexible enough to live up any, and all, expectations for a fully digital smart amplfier. 
- Don't let anyone be stuck with a unusable device, even late in its product lifecycle.  

## Hardware Features

µVox is the first of several designs in our portfolio. We're eager to release our platform, and have thus opted to release our first, and certainly most minimal design, as a standing invitation for the comminunity to come join our open audio-endeavours.
µVox features the essential hardware necessary, for anyone to get started with open audio, this includes: 

- Audio Amplifier IC (Merus MA12070P)
  - 2 x 80W (@ 10% THD) or 2 x 35W (@ 1% THD), @ DC 26V input.
  - Supply Voltage 7-26V.
  - Multilevel Class-D Switching technology for unparalleled power efficiency.
    
- ESP32 WROVER E Microprocessor Core
  - 16MB Flash + 8MB PSRAM
  - Wifi (2.4 GHz) & Bluetooth connectivity.
  - Unlimited possibilities, with regards to functionality. Your fantasy is the limit!

- Onboard RGB diode for user feedback.

- Connector for optional extension boards. (Compatible with Adafruits Stemma QT)

- (Optional) IDC connector for 'advanced' audio expansion modules.

- Power Protection Circuit
  - Reverse polarity protection.
  - Short circuit protection.
  - Over voltage protection on both the PVDD (up to 26V) and DVDD (5V) rail.

- All the essential DC-DC power regulation.

- Connector for external USB/UART bridge, for programming the µC. 


## Software Features

Officially supported by 'Euphonium', the most sophisticated open source embedded audio streaming platform we've ever seen, µVox is able to not only do classic A2DP Bluetooth Audio Streaming and native webradio streaming, but also native Spotify Connect. All of this functionality is bundled with a web-interface, hosted directly on the ESP, such that µVox is a stand-alone all-in-one open source streaming platform. 
See, FeelFreeLinux' repository for more details: https://github.com/feelfreelinux/euphonium
'Euphonium' is under rapid development, and as such isn't quite product-mature (as of Dec. '22), but we're in daily contact with FeelFreeLinux, updating oneanother with the latest features and bug-fixes, effectively co-developing the board.

## How to get involved!

Join our matrix-room! We update the ESP32-Audio community there regularly, and are always open to input, and or questions, there. 
https://matrix.to/#/#esp32_audio:matrix.org

## Where can i get one!?

We'll be back shortly with an official public sales channel, soon as we're satisfied with the initial hardware. 
However if you're eager to get your hands on one NOW - reach out, and we might just consider you for our beta-tester team!

## As seen in!.. 

We're already involved with several companies, wanting to use the platform in their products.
We're happy to announce our collaboration with 'Lyd By Dissing', featured in their latest product 'STRØM' - an open source smart speaker. 
See: https://github.com/LydByDissing/stroem and https://stroem.readthedocs.io/en/latest/ for further details. 
And if you happen to speak danish, our article in the newspaper 'the engineer': https://ing.dk/artikel/saa-skal-bygges-ings-laesere-udvikler-helt-ny-open-source-hoejttaler-vaer-med-254857

Besides STRØM, we're also involved with Lennart Jarde' latest project. 
Coming from a background as a prestigious classical musician, and serious hi-fi tinkering, Lennart is now focussing on his magnum opus: 
http://ljweb.dk/Loudspeakers/project/project.html
Again, if you happen to speak danish: https://dmf.dk/news/lennart-jarde-et-todelt-liv

We have several more collaborations in the works, however none of which are public, just yet. Stay tuned!

## Current status
**(March '23)**
Rev 0.9 units are almost done in production. Due to fault by the PCB manufactorer, the whole process has been delayed.
In the mean time Rev 0.92 has been developed. Changes include: Replacing our 3v3 LDO with a buck converter, replacing the 5v0 Buck, replacing the audio peripheral connector with a FPC connector (more on this later), replacing the speaker terminals with springloaded ones and shortening the board by ~8mm. Boards and parts will be ordered in the coming days.

![plot](./Renders/muvox_full.png)
![plot](./Renders/muvox_closeup.png)
