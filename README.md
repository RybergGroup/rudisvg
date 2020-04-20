# rudisvg
Rudisvg is a very rudimentary svg viewer. It was designed to view trees output as svg by treebender of the [phylommand](https://github.com/RybergGroup/phylommand) package. It is far from a complete svg viewer.You should be able to navigate in the image using the arrow keys, and zoom in and out with + and -. What makes rudisvg useful is that you can pipe the image into it. If you have no need for this there are much better software to view svg images out there.

Rudisvg depends on the x11 developmental libraries. If rudisvg is installed on for example bash on Ubuntu on Windows, you will need a X server as well, for example [Xming](https://sourceforge.net/projects/xming/), and set the DISPLAY variable:

    export DISPLAY=localhost:0.0

There is no need to do this on OS X or ordinary linux distributions (like Ubuntu) as the x server is integrated in these systems.

