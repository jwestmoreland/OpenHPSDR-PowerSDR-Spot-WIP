# OpenHPSDR-PowerSDR

Latest Test Release v3.6.0 Oct. 26, 2020

# 3.6.0 (2020-10-26)

Debug version of 'Spot' feature developed by KE9NS:  
Main reason currently adding this is for the WWV(B/H) capability to sync the PC's clock via
tuning to WWV(B/H) - not sure if WWVB currently works but I'm planning on adding it if it
isn't there already.  Note, some items are stubbed as the time sync feature was my main
reason for doing this plus having something that runs on the Atlas-Bus based OpenHPSDR rigs.
The 'spot' menu is 'hidden' - not on purpose - it's just where this is right now - between
the Collapse and RA items on the main menu bar.  If you get an exception, just hit continue -
that's one of the current side-effects of me stubbing out come code (that I will fix as
time permits hopefully).

Read the RealeaseNotes.md for more information.

# 3.4.9 (2018-3-19)
- Bug fix for manually entering frequency

# 3.4.8 (2018-3-17)
- Creates new wisdom file for each folder when using the -datapath command
- Bug fix for Behringer mini-wheels mapping issue when mapping AGC gain
- Added support for mapping drive level to a Behringer mini-wheel
- Added Panafall display for RX2
- Corrected a resizing problem when enabling RX2
- NB/NB2 is turned OFF while transmitting when DUP is enabled
- Added 2kHz Tune Step
- Changed ANF behavior so that it is disabled when in CW mode
- Removed the 750Hz CW filter and added a 150Hz CW filter (requires database reset to update)
- Added an Audio Adaptive Variable Resampler with monitor tools
- Increased display buffer to support larger than 4k displays
- Added separate VFO Lock controls for VFOA and VFOB. New VFO Lock button will require additional skin files to operate correctly.
- Added several CAT Commands. (see ReleaseNotes for details)
- Added a dropped packet ("OOOPs") counter that measures the number of dropped receive packets from radio to PC. This may be useful in identifying problems with network setup.
- fixed bug in CAT Command ZZPT## to change TXProfiles in different modes
- Updated CAT Commands documentation. Found in the Documentation/Radio folder

# 3.4.7 (2017-12-22)
- Control added to force the LPF to the 6m/ByPass position during receive. Filters must be under manual control to use. (Setup=>General=>Ant/Filters=>LPF, HPF/LPF, BPF1)
- VFO Lock correctly locks VFOA and VFOB.
- TX Amplitude scaling added to waterfall display. (Setup=>Display=>TX)

# 3.4.6 (2017-11-20)
- Corrected problem with blank waterfall display in Panafall mode.

# 3.4.5 (2017-11-20)
- Bug fix for .NET unhandled exception error when starting without radio online.

# 3.4.4 (2017-11-19)
- Added MIDI CAT support for the Behringer CMD Studio 2a
- Added support for the ANAN-7000DLE transceiver
- Added feature to select between receive or transmit antenna for receiving
- Use of seperate TX Profiles for various modes. 
  - LSB, USB, DSB, CWL, CWU, SPEC, & DRM 
  - FM
  - AM & SAM 
  - DIGL & DIGU
- PRO Latency feature added.

# 3.4.2 (2017-7-5)
- CTUN has had several modifications and bug fixes.
- Band Stacks have been increased to 5 deep for each band.
- CW Filters are now being saved correctly.

# 3.4.1 (2017-6-1)
- Swapped places with XIT and RIT controls on the console.
- Added 4 CAT Commands
 - ZZAP Audio Peak Filter On/Off
 - ZZAT APF Tune
 - ZZAB APB Bandwidth
 - ZZAA APF Gain
- Corrected compatibility issue with N1MM+ and FocusMaster.
- relabeled the 'CW Break-In' feature from 'Enabled' to 'Semi Break-In' to better describe the actual behavior. Toggles between Full Break-In and Semi Break-In.
- Single side-band Full Carrier (SSBFC)
- Continuous Frequency Compressor (CFC) audio tools
- Database enhancements allowing importing old databases

