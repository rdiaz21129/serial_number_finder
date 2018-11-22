# Purpose: 
Program goes through files (show inventory output) and obtains serial number
The script would open a file (below example) and parse the serial number for the switch. It will search PID "WS-C" and the SN.

===============<br />
COMMAND: show run | in hostname<br />
===============<br />
show run | in hostname<br />
hostname usnyc-csw-01<br />

===============<br />
COMMAND: terminal length 0<br />
===============<br />
terminal length 0<br />

===============<br />
COMMAND: show clock<br />
===============<br />
show clock<br />
14:44:52.248 CET Sat Oct 20 2018<br />

===============<br />
COMMAND: show switch<br />
===============<br />
show switch<br />
             ^<br />
% Invalid input detected at '^' marker.<br />


===============<br />
COMMAND: show inventory<br />
===============<br />
show inventory<br />
NAME: "1", DESCR: "WS-C3560G-24PS"<br />
PID: WS-C3560G-24PS-S  , VID: V05  , SN: FOCXXXXRRR3<br />

NAME: "GigabitEthernet0/25", DESCR: "1000BaseLX SFP"<br />
PID: Unspecified       , VID:      , SN: FOCCCCCCDD2<br />

NAME: "GigabitEthernet0/26", DESCR: "1000BaseLX SFP"<br />
PID: Unspecified       , VID:      , SN: ABCDEFGHI12<br />


