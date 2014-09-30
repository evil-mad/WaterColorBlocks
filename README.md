WaterColorBlocks
================

Code examples for driving the WaterColorBot from within block-based programming languages like Scratch and Snap!

##Current project status:

_For Snap!:_

The Snap! interface and examples are tested and working under the new CNCserver REST-less API (9/29/2014), with the exception of the known issues listed in the next section.


_For Scratch:_

The good news: We have implemented a new REST-less API (9/29/2014) within CNCserver, that appears to work around the new restriction on extensions added in recent versions. The scratch extensions (.s2e) can be loaded from within the Scratch 2 offline editor, or by opening the WCB-blocks.sb2 example file.

The bad news: Only the "bare blocks" are currently available -- these are interface elements that operate the WaterColorBot, but do not move the sprite.  Please also see known issues, below.


----

Known issues, as of 9/29/2014:
* The "Turn off motors & zero" command is not working as intended. The motors do turn off, but zeroing does not. That is to say, the program assumes that the carriage remains in the same position while motors are off.
* Documentation has not been updated for the new REST-less API.


----


## The helper app:
Currently requires "current" version of CNCserver:  https://github.com/techninja/cncserver

Run CNCserver in background, launched with command:

  node cncserver
  
*In the near future*, this will get a lot easier. RoboPaint ( https://github.com/evil-mad/robopaint ) will include this version of CNCserver, and you will only need to launch RoboPaint (a regular Mac/Win/Linux application) and let it run in the background.  
  
## More info:

Scratch is available at: http://scratch.mit.edu

Snap! is available at: http://snap.berkeley.edu

WaterColorBot is available at: http://watercolorbot.com

The Scratch API in CNCserver is documented here: https://github.com/techninja/cncserver/blob/master/SCRATCH.API.md
