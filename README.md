README.md
Vehicle functions by Mike (MP2) http://forum.sa-mp.com/showthread.php?t=339088

FEATURES:

Random vehicle colors (-1 in CreateVehicle) are synced between players
GetVehicleInterior function
GetVehicleColor function
ChangeVehicleColor works with -1 (random) colors
Siren automatically added to Ladder Firetruck
CHANGELOG: 1.2 (05/05/2015)

Updated for 0.3.7 (added siren parameter for CreateVehicle and AddStaticVehicleEx
Removed 'interior' parameter from CreateVehicle/AddStaticVehicleEx to keep in line with SA-MP's functions. Use LinkVehicleToInterior or SetVehicleInterior instead.
Commented out some unfinished code. May get around to finishing it.
AddStaticVehicle and AddStaticVehicleEx no longer re-direct to CreateVehicle. They use their own respective functions
Using y_hooks again...
Added GetVehicleSeatCount and GetVehicleModelSeatCount
1.1.3 (10th of February 2013):

Fixed a bug that caused OnVehicleSpawn to not be called. Caused by another array index out of bounds issue due to me not checking whether a vehicle colour was set to -1 (-1 is an invalid array index).
1.1.2 (7th of February 2013):

y_hooks no longer used (proper plug-n-play)
Hooked 'OnVehicleRespray' (reported missing by 'im'
1.1.1 (22nd of January 2013):

Fixed out of bounds array index issue with vehicle ID 2000.
1.1 (4th of May 2012):

Removing a paintjob now restores the vehicle's color (fixes SA:MP bug where vehicle became white)
Added 'GetVehiclePaintjob' function
Added RemoveVehiclePaintjob (simple macro ('redirect') to ChangeVehiclePaintjob)
1.0 (2nd of May 2012):

Initial Release
NOTE: This include relies on YSI's y_hooks, which can be found here: http://forum.sa-mp.com/showthread.php?t=570884
