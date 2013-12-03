What is it?
-----------

Colors the nick in irssi; you can opt to set the color of nicks to what you prefer, else it randomly colors each nick.

The orginal code was taken from http://scripts.irssi.org/ and was slightly modified to add more colors by using reverse mode.

Loading Scripts
---------------

1. Download the code as nickcolor.pl (https://raw.github.com/vigith/random/master/irssi/nickcolor.pl)
2. move to ~/.irssi/scripts/ or /usr/local/lib/irssi/scripts/ (for system wide use)
3. /SCRIPT LOAD nickcolor
4. if you want to unload /SCRIPT UNLOAD nickcolor 

Scripts are run with /SCRIPT LOAD command, or the default /RUN alias.
"/SCRIPT" shows list of running script, and /SCRIPT UNLOAD can unload
scripts.

Scripts should be placed to ~/.irssi/scripts/ or
/usr/local/lib/irssi/scripts/ (or depending on where irssi was
installed) directories. After that /RUN script_name should work, you
don't need to add the .pl suffix.


More Doc: http://www.irssi.org/documentation/perl

Supported Commands
------------------

**_/color preview_** lists all the available colors

**_/color set nick int** sets the color (please replace nick with the nick of the user and int with a value >2 and <=28)

**_/color save_** saves the color

**_/color list_** shows the saved colors

**_/color clear_ <nick>** will clear the saved color for the nick

Not Working?
------------

Run **/load** on your irssi window and check whether perl is listed in loaded modules. If not, you need to use a irssi compiled with perl. More Info: http://www.irssi.org/documentation/perl

if you think there is a bug, please feel free to open a bug.

TODO
----
1. more options by using smart backgroud coloring
2. underlining to be used with colors to increase the option?
