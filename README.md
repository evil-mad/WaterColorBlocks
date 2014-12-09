WaterColorBlocks
================

Code examples for driving the WaterColorBot from within block-based programming languages like Scratch and _Snap!_ To use these examples, you will need to also download and launch a helper app (see below) that manages communication with the WaterColorBot.


##Current project status: Sneak Preview stage! We are gearing up for "official release," working on checks, balances, bug fixes, additional examples, and documentation. Additional eyes are welcome now, as we head towards official release, currently estimated at late December 2014 or early January 2015.


####_For Snap!:_
The _Snap!_ interface and examples are tested and working under the new CNCserver REST-less API (9/29/2014).


####_For Scratch v2 Offline:_
The Scratch interface and examples are tested and working under the new CNCserver REST-less API (9/29/2014).

Please note that only the Scratch interface is somewhat simpler than the  _Snap!_ interface: The blocks in the interface move the WaterColorBot, but do not automatically move the sprite on the screen to match. 

####_For Scratch v2 Online:_
Pending full support for 3rd party extensions, you can enable WaterColorBlocks in the [Scratch online editor](http://scratch.mit.edu/projects/editor/) using the following code as the URL in a bookmark to make a bookmarklet:
```javascript
javascript:(function(){var%20s=document.createElement('script');s.setAttribute('src','https://cdn.rawgit.com/techninja/cncserver/8a95b420519e09a6692177a8a4d5fa87fc26b54c/watercolorbot_scratch.js');document.body.appendChild(s);}());)
```
Once you have that saved, just click the bookmark while in the loader and the WaterColorBlocks will appear in the **More Blocks** section.

----

## The Helper App
Using the WaterColorBot through WaterColorBlocks requires the use of a helper application that runs in the background operating the robot.  


### RoboPaint :
The WaterColorBot interface is built into RoboPaint, versions 0.9.0b and higher.  Download RoboPaint at https://github.com/evil-mad/robopaint/releases .  When you launch RoboPaint, it should automatically connect to the WaterColorBot. All that you need to do is simply launch it, and leave it running in the background while you use Scratch or _Snap!_. It is recommended to leave RoboPaint on the _Home screen_ (asking you to choose between Create/Print/Manual) while it is running.


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
