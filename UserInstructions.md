# Introduction #

This page explains how to use and connect to the SwiFTP server on your Android phone. It assumes you've already downloaded and installed the program.

If you're a resourceful sort of person, you can probably figure everything out just by messing around with SwiFTP. Simplicity is a major design goal, and nothing is very complicated.

Questions can be addressed to the SwiFTP-users group: http://groups.google.com/group/swiftp-users if they're not answered here. I (Dave) monitor this list and usually respond immediately.

# General instructions #

Here are rudimentary instructions for those who are familiar with FTP. More detailed instructions with

  * The server is listening to port 2121 on the wifi network interface, unless you've configured something different.
  * Your wifi IP address is shown from the main SwiFTP screen as a convenience
  * Any FTP client should work. If not, please report this, it's probably a SwiFTP bug: http://code.google.com/p/swiftp/issues/list. Please include as many details as possible about the software and operating system that you are using.

Modern browsers have at least read-only FTP support. Try punching in your server URL (the "ftp://...." thing) into the address bar of your browser to get read-only access to your files.

## Android filesystem permissions and the /sdcard directory ##

If you're running a T-Mobile G1 like I am, you don't have write permissions to much of your filesystem. This is an unfortunate fact of life that has been inflicted on us by T-Mobile for business reasons. Most likely you want to store your stuff in the /sdcard directory. **Update:** there are ways to get root access on your G1. Google can find the details.

# Windows XP/2000 #

Follow these steps:

  * Start Menu -> Run.
  * In the box that appears type "explorer", press enter.
  * Enter the Server URL as it appears inside the SwiFTP application. This is the thing that starts with "ftp://".
  * If you are prompted for a username, enter "anonymous". If you are prompted for a password, enter anything you like.
  * Rock out.

Here's a tip from a user named Byron for easy Windows integration:

_I easily set up Windows Explorer to show my G1 as a folder. This works on both
XP and Vista. Right click on My Computer and select Add a Network Location. I
typed in `ftp://myusername:mypassword@192.169.1.100:2121/sdcard` and named it
"My G1." When I click on My G1 in Explorer now, it takes me straight to my
sdcard without having to enter username and password each time._

# Windows Vista #

Someone please help with this one. Wiki!

# Mac OS X #

## Read-Only Access ##

The Finder has built in read-only support for FTP. Select "Go → Connect to
Server..." or press ⌘K and enter the Server URL as displayed by SwiFTP
(e.g., `ftp://192.168.1.100:2121/`). You'll be prompted for your SwiFTP
username and password.

## Read-Write Access ##

If you need to add or delete files from your device, you'll need a third party
FTP client. We recommend [Cyberduck](http://cyberduck.ch/) (free), but
commercial clients like [Transmit](http://www.panic.com/transmit/) should work
as well. As before, simply point the client to your phone's IP address, and
change the port number to match your SwiFTP settings (2121 by default). If
you're using Cyberduck, you can just type "Server URL" shown by SwiFTP into the
Quick Connect box.