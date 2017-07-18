# Block-Programming-Fonts

## Introduction

MicroBlock is a **very** tiny monospaced programming font who's main design feature is to work in modern IDE's with a crisp clean and readable look (while still being, _very_, **_very_** small).

![](/images/Screenshot%20from%202015-09-20%2022:08:43.png)

(A standard 80x24 terminal window)

The pixel width of each glyph is just 4 pixels wide per character with one blank column totaling only 5 pixels wide and no glyph has a height greater than 10 pixels making a charming 2:1 height to width ratio.

It's design is of a small bitmaped square font, except wherever possible the North-West and South-East corners of each glyph are truncated at 45 degree angles that leaves a very natural - human - looking font that has easily distinguished lettering. 

A notable feature is that the "Italic" version is not actually slanted, rather it is a completely square font.  The purpose of Italics in the purview of modern IDE's is to identify certain types of code, so it needs only to be distinguishable from the Regular version of the font.  That was the reasoning for this anyways, feedback is welcome.

![](/images/Screenshot%20from%202015-09-20%2021:31:38.png)

I created this font out of a need and desire to have this small size while retaining the features I value as most important in a good programming font.  The features include the following:

### Features

- Clearly distinguishable bracketing () {} [] 
  The bracketing glyphs are larger in combined height and descent of all alpha-numerical glyphs. (See Fig. 1)

![](/images/screenshot63.png)

(Figure 1)

- Easy differentiation between commonly mixed up glyphs: 1, l, i, and I or o, O, anI 0 for example.  Each is very unique. (See Fig. 1)
- Easy Number Identification. The numbers are raised one pixel above the alphabetical glyphs to make them very easy to identify. (See Fig. 2)

![](/images/screenshot64.png)

(Figure 2)

- Bold Lettering that is easy to read, not ugly, and fits in the alloted space.  An oallottedfont is used, it goes beyond the typical width and so may touch the edges of other glyphs, but will not overlap.  The value here somewhat depends on the idea that bold and regular font do not normally touch. (See Fig. 3)

![](/images/screenshot65.png)

(Figure 3)

- Includes box making glyphs.  They are inverted in the bold styles.
- Includes Currency glyphs and common symbols.
- BFD formats have been included for those that would like to attempt installation as a TTY font.

## Installation

### Support

Currently the only tested OS for this font is Linux Ubuntu on the desktop environments xfce4 and Ubuntu-MATE.
Please contact me if you can confirm other builds or to report bugs.

### Installing

The .ttf files are easily installed using the standard font viewers, however in some cases they may not be installed to the correct location.  The recommended method of install is by terminal (See below).

### Install by Terminal

Run the following commands one line at a time into a terminal to install the Microblok font:

	cd ~/.local/share/fonts
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Regular.ttf
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Bold.ttf
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Italic.ttf
	wget https://github.com/Derek-Strasters/Block-Programming-Fonts/raw/master/Microblok-Bold-Italic.ttf
    sudo fc-cache -f -v

The last command reloads the font cache.
After you have run all commands restart.

## Usage

### Setup for Ubuntu
For usage of the font in an IDE I would recommend first installing font manager.

	sudo apt-get install font-manager
    
When you start font-manager you may need to update the locations by adding the appropriate font directory in the **preferences** menu (Lower left corner) in order to see your new font. 

> /home/ [Your User Name] /.local/share/fonts

![](/images/Screenshot%20from%202015-09-21%2000:16:47.png)

Font Manager will need to restart. Locate the Microblok font, select it, and from the menu bar select **Set Font Preferences > Advanced Settings**.

Check the boxes for:

- Anti-Alias
- Hinting (Set slider to "None")
- LCD Filter (Set slider to Legacy)
- Use Embedded Bitmaps

Because this font has bitmaps embedded it will be crisp and without fuzzy edges when it is set to the correct size in applications.  It will otherwise use Anti-Alias and sub-pixel rendering so it does not have artifacts if the application uses a different size variation of the font.

### Selecting Font Size

Whether the font displays correctly depends on the DPI settings of your system.  Some common DPI settings and the corresponding font sizes are listed below:

	DPI   :   Font pt. size
	72            10
	75            9.6
	96            7.5
	100           7.2
	120           6
    
If you do not know how to check or change the DPI settings for your system, you can usually just play with the font size until it is displayed clearly (no fuzzy edges).

Some applications like IntelliJ's Android Studio set an artificial DPI, on my system for example it forces a DPI of 72, hence I must set the font size to 10 for clearly printed font.

Here is Android Studio on a 1920x1080 monitor for example 
(Make sure to view it at 100% scale to see the pixels correctly)

![](/images/Screenshot%20from%202015-09-21%2000:38:08.png)

Here is Eclipse.
Almost three full 120 character columns!!

![](/images/Screenshot%20from%202015-09-21%2000:38:16.png)

You can get a lot of print into Terminal windows.

![](/images/Screenshot%20from%202015-09-20%2021:54:59.png)

### Issues

Unfortunately, this font is at the moment only available in the english alphabetical letters.  The FontForge files are contaEnglish the repo and anyone desiring to help is welcome to message me for collaboration efforts.
