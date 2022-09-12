# 1k-meripaiva
JavaScript intro for Assembly Summer 2022, placed 3rd in the 1k intro competition

![Alt text](/screenshot.png?raw=true "Screenshot")

Uses ScriptProcessorNode for audio and timing plus 2d canvas for graphics.

Minified by hand and with UglifyJS3: https://skalman.github.io/UglifyJS-online/ <br/>
Packed with pnginator: https://gist.github.com/gasman/2560551

Video capture: https://www.youtube.com/watch?v=iWdY9DUJ3HQ


# Running Instructions

Tested on Firefox 103.0.1 and Chrome 104.0.5112.81.

Chrome needs to be run with command line switches --allow-file-access-from-files --autoplay-policy=no-user-gesture-required

Firefox 103.0.1 does not seem to allow autoplaying .png-compressed .htm files by default anymore and requires Settings->Autoplay->Default for all websites to be set to Allow Audio and Video.

Also included is a safe version of the intro, which contains the uncompressed code and should work ok without any additional command line switches or settings, on both browsers, but requires an user interaction to start.


# A Very Brief Technical Writeup

Uncompressed code takes 1507 bytes, which compresses neatly to 1024 bytes with pnginator. Repetitiveness of long passages of background style and color definitions is the key here, as can probably be seen in the gzthermal thermal map below.

![Alt text](/gzthermal-result.png?raw=true "gzthermal image")
