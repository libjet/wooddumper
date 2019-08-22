# wooddumper
Automatically exported from code.google.com/p/wooddumper

"wooddumper" is a tool made around 2010 that aims to dump SLOT-1 Cartridges into a .nds format on the Nintendo DS.

Since the google code archive source is really messy, I decided to fork a "github-ified" version which makes it much easier to work
with, especially to a newbie like me.

The last time this was updated was on Mar 26, 2010, and hasn't really been updated until then so of course it doesn't readily
compile. As far as I can tell, the app uses a custom library called "libcard" which needs to be built before anything else.
The only exception is woodsec, which according to the creator is a "tool to manipulate secure area."

There actually has been a patch made to support libnds 1.4.8 on Mar 19, 2016, and will be tested to see if it fixes any issues that
have arisen over the years, but even that's outdated as the current version is libnds 1.7.3-3 as of Aug 22, 2019.


# User guide
This is a tool that can dump "problematic" (512 byte data buffer) cards with correct full header {previously FF-filled/replicated/undumpable). It performs the same as patched FTPd.

For Slot 2 version, put rom to a Microsd and it saves the rom to a slot 2 card.

For WiFi version, it is a FTP server app. It waits for connection from FTP client (supports passive transfer mode) or common Internet browsers (tested with Firefox and IE8).

Server IP address is displayed on NDS top screen. It expects connection on port 21, login/pass can be anything. Resume is supported.

Client disconnection is required for changing card to be dumped.
(taken from gamebrew.org)

# Credits
TrashMan, WRG, Sir VG and Caravan.
