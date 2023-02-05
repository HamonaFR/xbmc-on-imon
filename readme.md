# XBMC on iMON Display

**UPDATE by HamonaFr (Febuary 2023)**

![Screenshot](docs/XbmcOniMon.JPG)

I have updated XBMC on iMON Display to work with newest version of Kodi (Nexus).

I made some change on 


---------------

Table of Contents
=================
1. Hardware Requirements
2. Software Requirements
3. Installation
4. Preparations
5. Usage
6. Known Issues
7. Support
8. Disclaimer


## 1. Hardware Requirements
To be able to use "XBMC on iMON Display" you need an LCD or VFD from
Soundgraph's product line "iMON". Soundgraph has not yet provided detailed
information about the compatibility of different Display versions. If you
cannot get "XBMC on iMON Display" to show anything on your LCD or VFD,
please report this so we can help investigate the problem.

## 2. Software Requirements

 - Windows 7 or newer
 - Microsoft .NET Framework 2.0: https://learn.microsoft.com/en-us/dotnet/framework/install/dotnet-35-windows
 - iMON Manager v8.12.1202: You need to install iMON Manager v8.12.1202 or higher
   (https://www.lo4d.com/get-file/imon/723e98d0999412c6b7cac5b094b5e31c/)
 - Kodi 18 or newer: http://mirrors.kodi.tv/releases/windows/


## 3. Installation

There is no real installation. Simply extract all the files into a folder.
If you want to have a desktop icon, right-click the file called XbmcOniMon.exe
and choose "Send to" --> "Desktop". 

## 4. Preparations

Before you start "XBMC on iMON Display" you need to make some configurations.

General
-------
Make sure no other running software on your computer is using TCP port 9090.
You can do that by using NMap (http://nmap.org/) to scan the port and see if
it is currently used. Unfortunately this port is currently hardcoded within
XBMC and therefore can't be changed.

iMON Manager
------------
Open iMON Manager and go to "Options" --> "Plug-in Mode" and activate the "Use 
Display Plug-in Mode" checkbox. Then go to "iMON Utilities" --> "FrontView" and 
make sure "Run FrontView When iMON Starts" is either set to "Always" or 
"Automatically".
Now go to "iMON Utilities" --> "FrontView" and open the "Media Information" tab.
Here you need to disable the "XBMC" option under "Available Player".
Also make sure that iMON Manager is running when you start "XBMC on iMON Display".

Kodi (XBMC)
----
Open Kodi and go into "Settings" --> "Network" --> "Services". Activate the option
"Allow control of XBMC via HTTP" and enter a Port (Username and Password are optional).

## 5. Usage

Start "XBMC on iMON Display" simply by double-clicking the XbmcOniMon.exe.
A window will open up which consists of a menu bar (allowing to manually
connect/disconnect with/from XBMC and initialize/uninitialize the iMON
Display API), a navigation (General, iMON, XBMC) and options. All the options
should be self-explaining. Simply click one of the three option areas in the
navigation to see their specific options. Changing an option immediatelly 
affects the way "XBMC on iMON Display" behaves.

Make sure you provide the correct information to be able to connect with XBMC.

## 6. Known Issues

Here is a list of a few known issues. Please DO NOT report these as bugs!
 - The iMON Display stays dark after initialization when it is deactivated in
   iMON Manager
 - The progress bar does not adjust correctly when Fast Forwarding / Rewinding
 - The display freezes for a short time when pressing a button on a remote. To
   avoid this disable the "iMON Remote Control Messages" in "iMON Manager" --> 
   "iMON Utilities" --> "FrontView" --> "Auto mode"

## 7. Support

If you encounter any bug or have a problem using "XBMC on iMON Display" please visit
the project management site at https://github.com/HamonaFR/xbmc-on-imon/issues.

## 8. Disclaimer

This Program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2, or (at your option)
any later version.

This Program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with UMM; see the file COPYING.htm in the main solution.  If not, write to
the Free Software Foundation, 675 Mass Ave, Cambridge, MA 02139, USA.
http://www.gnu.org/copyleft/gpl.html
