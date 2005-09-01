/***************************************************************************/
/* README.txt                                                              */
/*   - ReadMe for the HL-MapConf script                                    */
/*   - Description and use for the HL-MapConf script package               */
/*   - Distributed under the GPL terms - see the readme (this doc) for info*/
/*   - Copyright Brian Porter <beporter@users.sourceforge.net>             */
/*   - Part of HL-MapConf v0.91                                            */
/***************************************************************************/
/* CVS $Id$ */
/***************************************************************************/

    HL-MapConf
    Copyright (C) 2005 Brian Porter     <beporter@users.sourceforge.net>
    All Rights Reserved

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program; if not, write to the Free Software
    Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

-----------------------------------------------------------------------------

DESCRIPTION
-----------

HLmapconf is a Perl script designed to help Steam-based server admins
maintain map-specific cfg files. The script provides batch creation and
modification of cfg files.


REQUIRES
--------
 + A Steam-based Half-Life server
 + Perl 5.6+ installed on the game server machine (*nix OR Win)
 + A bit of common sense

INSTALLING
----------
1) If you're reading this, you've already decompressed the script package.

3) Set the internal variables. In order to be easier to use on a daily basis,
   the script stores the locations of the directories and files it works
   within inside itself. Open hlmapconf.pl in your favorite text editor and
   point the config variables at the top of the file to your server's
   base directory. Set the name of the mod you are using ('cstrike' for
   Counter-Strike, for example), and the name of your mapcyce file (usually
   'mapcycle.txt'). Save and close the file.

3) Move hlmapconf.pl to wherever you like to keep utilities scripts (probably
   in your PATH somewhere) and optionally make sure its executable. A detailed
   description of how to use the script can be found by calling it with the
   -v argument.

USAGE NOTES
-----------
- If you place the script in your mod's directory and call it using 
  ./hlmapconf.pl [args] you can do without editing the internal config
  variables (assuming you're running a CS1.6 server that is).
  
- There is a chance there might one day be a visual Tk-based version of
  this script. When that day comes, it will be good for this file to have some
  info on getting the Tk Perl module.
  
- Be warned that the script will not prompt before it overwrites existing
  config files.

- There are many ways this script could be improved. If you care to do so,
  please consider submitting your changes back to me to roll into the 
  SourceForge release so everyone can benefit.
  
  
--
Thanks and good luck!
Brian and the HL-MapConf Development Team

/*#########################################################################*/
