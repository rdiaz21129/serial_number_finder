Purpose: Program goes through files (show inventory output) and obtains serial number
The script would open a file (below example) and parse the serial number for the switch. It will search PID "WS-C" and the SN.
===============
COMMAND: show run | in hostname
===============
show run | in hostname
hostname usnyc-csw-01

===============
COMMAND: terminal length 0
===============
terminal length 0

===============
COMMAND: show clock
===============
show clock
14:44:52.248 CET Sat Oct 20 2018

===============
COMMAND: show switch
===============
show switch
             ^
% Invalid input detected at '^' marker.


===============
COMMAND: show inventory
===============
show inventory
NAME: "1", DESCR: "WS-C3560G-24PS"
PID: WS-C3560G-24PS-S  , VID: V05  , SN: FOCXXXXRRR3

NAME: "GigabitEthernet0/25", DESCR: "1000BaseLX SFP"
PID: Unspecified       , VID:      , SN: FOCCCCCCDD2     

NAME: "GigabitEthernet0/26", DESCR: "1000BaseLX SFP"
PID: Unspecified       , VID:      , SN: ABCDEFGHI12     


