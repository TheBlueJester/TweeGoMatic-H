# TweeGoMatic

## What is TweeGoMatic?
This project aims to build upon the existing [Tweego software](https://github.com/tmedwards/tweego/) and bring a number of features centered around automation of Tweego to eliminate the need to learn and enter command-line instructions found in [Tweego's documentation](http://www.motoslave.net/tweego/docs/).

The primary goal of TweeGoMatic is to allow people to quickly and easily move from the Twine.exe program provided on [Twinery.org](twinery.org) to using [Twee3 Notation](https://github.com/iftechfoundation/twine-specs/blob/master/twee-3-specification.md) and their choice of IDE's. <br>
This was inspired by my transfer to using VS Code with the plug-in [Twee 3 Language Tools](https://marketplace.visualstudio.com/items?itemName=cyrusfirheir.twee3-language-tools). <br>
While it's a fantastic extension, it doesn't assist in the migration of projects from Twine.exe and isn't able to compile .twee files into useable .html files. Like Twine.exe offers. <br>

TweeGoMatic meakes it easy to migrate to using Twee3 Notation via "drag and drop" interactions to decompile .html made with Twine.exe into .twee files. <br>
And then allows users to "drag and drop" compile their .twee files into usable .html files once they are ready to test or publish their work. <br>
There is also the option to run TweeGoMatic the entire time someone works on their project and have it automatically detect changes to the .twee file and re-compile it to .html.

At the end of the day thanks needs to go to <b>[tmedwards]((https://github.com/tmedwards/)<b> for creating tweego in the first place. <br>
I have simply updated what they built and made scripts of convenience and nothing more.


### Current Features & Usage:
-- Drag and Drop .twee files onto "compile.bat" will compile them and generate a .html with no user input required. <br>
This uses tweego's automatic story format detection and may not work perfectly in all cases. <br>
-- Drag and Drop .html files onto "decompile.bat" will decompile a .html file into a .twee file with no user input required. <br>
This uses tweego's automatic story format detection and may not work perfectly in all cases. <br>
-- Drag and Drop .twee files onto "live recompiler.bat" to have them continuously compiled to .html whenever changes are made.


### What is Tweego?
[Tweego](https://github.com/tmedwards/tweego/) is command-line software that assists with the generation of Twine 2 Interactive Fiction & Games from Twee code. [Twine/Twee](http://twinery.org/)

## Current Release
The current release is [v0.0.2](https://github.com/TheBlueJester/TweeGoMatic/releases/tag/v0.0.2) <br>
See Change Log below for it's contents and changes.

## Notes
Progress on this project was made more rapidly than I had anticipated. I had intended for versions 0.0.X to be pre-release and very limited. <br>
However these versions actually contain the majority of the "Road Map" updates I'd planned out and thus the versioning doesn't match well with the road-map. <br>
I will get to correcting this at some point soon. <br>

## Change Log

### Version 0.0.1

#### Tweego Binaries updated
-- tweego binary has been recomplied using the latest version of GO, which includes 2 years of updates. <br>
-- tweego.exe is now about 12% smaller then the official version 2.1.1 binary. <br>

#### Story Formats updated
-- Chapbook-1 Story Format has been updated from version 1.0.0 to 1.2.2 <br>
-- Sugarcube-1 Story Format was confirmed as latest. <br>
-- Sugarcube-2 Story Format has been updated from version 2.30.0 to 2.36.1 <br>
-- Paperthin-1 Story Format was confirmed as latest. <br>
-- Harlowe-1 Story Format was confirmed as latest. <br>
-- Harlowe-2 Story Format was confirmed as latest. <br>
-- Harlowe-3 Story Format has been updated from version 3.1.0 to 3.3.0 <br>
-- Snowman-1 Story Format was confirmed as latest. <br>
-- Snowman-2 Story Format was confirmed as latest. <br>
-- Added Snowman-3 Story Format, current version is Version 3.0.0 <br>

### Automated Features
--Dragging a .twee file onto compile.bat will generate a compiled .html file based on tweego's automated detection of the Story Format. <br>
--Dragging a .html file onto the decompile.bat will generate a decompiled .twee file based on tweego's automated detection of the Story Format. <br>

### Version 0.0.2

#### Story Formats
-- Includes a seperate .zip file containing all of the updated format.js files listed as updated in v0.0.1 <br>

#### Automated Features
-- Updated versions of "compile.bat" and "decompile.bat" with improved language / information prompting. <br>
-- The first edition of "live compiler.bat" which takes in a .twee file via drag and drop and continuously monitors for changes, upon which it recompiles to .html output.


## Road Map

This initial release, Version 0.1.0 will be the only release that targets multiple operating systems. 
Future releases that include the planned automated features will be Windows exclusive software.
If some level of popularity occurs, scripts for Linux will also be made avalible. 
At no stage will MacOS recieve support.

### Version 0.1.0 - Reboot
First the Tweego base code will be recompiled using the latest version of GO which includes 2 years of improvements.

Second the story formats included with Tweego will be updated to their current versions, again with 2 years of changes and improvements since the last offical Tweego release.

### Version 0.2.0 - Automation
Using Windows batch files (.bat) the following automations will be introduced.
1) Drag and Drop Compiling of .tw and .twee files to .html
2) Drag and Drop Decompiling of .html files into .twee
3) Automatic detection of changes to .twee source and continuous recompile .html

### Version 0.3.0 - Apply Polish
This version will move the project from .bat files to .exe files for Windows.
These .exe files will include icons, upgrading from the iconless tweego.exe and batch files included in priror releases. 
User interaction, prompts and menus, will be reworked to be more professional and intuitive.
