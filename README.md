WaterColorBlocks
================

Code examples for driving the WaterColorBot from within block-based programming languages like Scratch and _Snap!_ To use these examples, you will need to also download and launch a helper app (see below) that manages communication with the WaterColorBot.


##Current project status:

_For Snap!:_

The _Snap!_ interface and examples are tested and working under the new CNCserver REST-less API (9/29/2014), with the exception of the known issues listed in the next section.


_For Scratch:_

The good news: We have implemented a new REST-less API within CNCserver, that appears to work around the new restriction on extensions added in recent versions. The scratch extensions (.s2e) can be loaded from within the Scratch 2 offline editor, or by opening the WCB-blocks.sb2 example file.

The bad news: Only the "bare blocks" are currently available -- these are interface elements that operate the WaterColorBot, but do not move the sprite.  Please also see known issues, below.



----

## The Helper App
Using the WaterColorBot through WaterColorBlocks requires the use of a helper application that runs in the background operating the robot.  


### RoboPaint :
The WaterColorBot interface is built into RoboPaint, versions 0.9.0b and higher.  Download RoboPaint at https://github.com/evil-mad/robopaint/releases .  When you launch RoboPaint, it should automatically connect to the WaterColorBot. All that you need to do is simply leave it running in the background while you use Scratch or _Snap!_.


### Alternate helper app (CNCserver):
If you cannot (or do not wish to) run RoboPaint for any reason, you can alternately run CNCserver in the background, to manage communication with the WaterColorBot. You can download the current version of CNCserver here:  https://github.com/techninja/cncserver

Run CNCserver in background, launched with command:

  node cncserver
  
It is worth noting that "under the hood," RoboPaint contains and runs a copy of CNCserver that it uses to communicate with the WaterColorBot.

  
## More info:

Scratch is available at: http://scratch.mit.edu

_Snap!_ is available at: http://snap.berkeley.edu

WaterColorBot is available at: http://watercolorbot.com

The Scratch API in CNCserver is documented here: https://github.com/techninja/cncserver/blob/master/SCRATCH.API.md
