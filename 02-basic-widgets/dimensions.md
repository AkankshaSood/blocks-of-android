# Dimensions

Different mobile devices have different screen sizes as well as diffrent pixel sizes. It means that if this difference in pixel sizes is not taken into account while designing the layouts, then either the images will blur out due to scaling or will be displayed in wrong sizes.

Consider an example of a two devices having the same screen size but different resolution (Resolution is expressed in the form of x*y, where x denotes the number of pixels in the horizontal direction and y denotes the number of pixels in the vertical direction). So now if a button of size 2px is added to both the screens,, it will appear differently because 2px will mean a larger size in the screen having lesser resolution. Here dp comes to our rescue.

<b>Dp</b> stands for <b>density independent pixels</b>. It is a virtual pixel that is independent of the density of pixels of the device. dp or dip is equivalent to one physical pixel on a 160 dpi(density per inch) screen, which is the baseline density assumed by the system for a "medium" density screen. The conversion takes place according to the formula: px = dp * (dpi / 160). The scaling of dp is handled at the runtime based on the density of the device screen.

Next, there comes another unit known as <b>sp</b> or <b>scale independent pixels</b>. Similar to dp, sp is also device independent and has 160 units per square inch but in addition to that, it is also scalable according to the user's font size preference.

Therefore, always use sp for defining the text size and for everything else like layout dimensions or position use dp.
