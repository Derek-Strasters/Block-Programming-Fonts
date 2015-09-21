# Block-Programming-Fonts

##Introduction

MicroBlock is a **very** tiny monospaced programming font who's main design feature is to work in modern IDE's with a crisp clean and readable look (while still being, _very_, **_very_** small).

The pixel width of each glyph is just 4 pixels wide per character with one blank column totalling only 5 pixels wide and no glyph has a height greater than 10 pixels making a charming 2:1 height to width ratio.

It's design is of a small bitmaped square font, except wherever possible the North-West and South-East corners of each glyph are truncated at 45 degree angles that leaves a very natrual - human - looking font that has easily distinguished lettering. 

A notable feature is that the "Italic" version is not actually slanted, rather it is a completely square font.  The purpose of Italics in the perview of moder IDE's is to identify certain types of code, so it needs only to be distinguashable from the Regular version of the font.  That was the reasoning for this anyways, feedback is welcome.

I created this font out of a need and desire to have this small size while retaining the features I value as most important in a good programming font.  The features include the following:

###Features

- Clearly distinguashable bracketing () {} [] 
  The bracketing glyphs are larger in combined height and descent of all apha-numerical glyphs. (See Fig. 1)
(Figure 1)![]({{site.baseurl}}//images/screenshot63.png)

- Easy differentiation between commonly mixed up glyphs: 1, l, i, and I or o, O, and 0 for example.  Each is very unique. (See Fig. 1)
- Easy Number Identification. The numbers are both emboldened and raised one pixel above the alphabetical glyphs to make them very easy to identify. (See Fig. 2)
(Figure 2)![]({{site.baseurl}}//images/screenshot64.png)

- Bold Lettering that is easy to read, not ugly, and fits in the alloted space.  An outline font is used, it goes beyond the typical width and so may touch the edges of other glyphs, but will not overlap.  The value here somewhat depends on the idea that bold and regular font do not normally touch. (See Fig. 3)
(Figure 3)![]({{site.baseurl}}//images/screenshot65.png)

- Includes box making glyphs.  They are inverted in the bold styles.
- Includes Currency glyphs and common symbols.
- BFD formats have been included for those that would like to attemp instalation as a TTY font.

##Installation

###Support

Currently the only tested OS for this font is Linux Ubuntu on the desktop environments xfce4 and Ubuntu-MATE.
Please contact me if you can confirm other builds or to report bugs.

###Installing

The .ttf files are easily installed using the standare font viewers, however in some cases they may not be installed to the correct location.  The recommended method of install is by terminal (See below).

###Install by Terminal

Run the following commands one line at a time into a terminal to install the Microblok font:

> cd ~/.local/share/fonts
    
	> wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Regular.ttf
    
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Bold.ttf
    
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Italic.ttf
    
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Bold-Italic.ttf

