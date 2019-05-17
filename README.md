# FGFS201831-METAR-patch
Patched LINUX (LUbuntu 18.04) binary after NOAA changed URL for METAR data.
This patch uses additive python script for redirecting to new NOAA URL
Usage :
Backup Your original fgfs.exe
Download this package, extract fgfs.exe and overwrite original one
Set EXECUTE permission on this new file
Run Terminal and use command python3 metar.py. Then start FGFS. 
Based on SurferTim's solution described at https://forum.flightgear.org/viewtopic.php?p=342372#p342372
All credits and big thanks to SurferTim

Attention !!!
This is patched FGFS 2018.3.1. It will work only with original FGFS2018.3.1. No other version supported.

Manual patch with hex editor :
find text http://tgftp.nws.noaa.gov/data/observations/metar/stations/
replace it with http://mgouin.appspot.com/fg?icao-station-identifier-name1= 
