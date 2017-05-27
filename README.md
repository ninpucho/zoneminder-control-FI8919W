# zoneminder-control-FI8919W
Control file for FOSCAM FI8919W, source FI8918W from zoneminder project.

# Original descriptions in FI8918W file

# Modified on Jun 19 2016 by PP
 Changes made
 	- modified command to work properly and pick up credentials from Control Device
	- the old script did not stop moving- added autostop 
	  (note that mjpeg cameras have onestep but that is too granular)
	-  You need to set "user=xxx&pwd=yyy" in the ControlDevice field (NOT usr like in Foscam HD)

==========================================================================

 ZoneMinder Foscam FI8918W IP Control Protocol Module, $Date: 2009-11-25 09:20:00 +0000 (Wed, 04 Nov 2009) $, $Revision: 0001 $
 Copyright (C) 2001-2008 Philip Coombes
 Modified for use with Foscam FI8918W IP Camera by Dave Harris
 Modified Feb 2011 by Howard Durdle (http://durdl.es/x) to:
      fix horizontal panning, add presets and IR on/off
      use Control Device field to pass username and password
 Modified May 2014 by Arun Horne (http://arunhorne.co.uk) to:
      use HTTP basic auth as required by firmware 11.37.x.x upward

 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation; either version 2
 of the License, or (at your option) any later version.

 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.

 You should have received a copy of the GNU General Public License
 along with this program; if not, write to the Free Software
 Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.

==========================================================================

 This module contains the implementation of the Foscam FI8918W IP camera control
 protocol

#FI8918W

ZoneMinder::Database - Perl extension for FOSCAM FI8918W

#SYNOPSIS

Control script for Foscam MJPEG 8918W cameras. 

#DESCRIPTION

You need to set "user=xxx&pwd=yyy" in the ControlDevice field
of the control tab for that monitor.
Auto TimeOut should be 1. Don't set it to less - processes
start crashing :)
NOTE: unlike HD foscam cameras, this one uses "user" not "usr"
in the control device

#AUTHOR

Philip Coombes, E<lt>philip.coombes@zoneminder.comE<gt>

#COPYRIGHT AND LICENSE

Copyright (C) 2001-2008  Philip Coombes

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself, either Perl version 5.8.3 or,
at your option, any later version of Perl 5 you may have available.
