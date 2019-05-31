Z-ENEMY 2.00  From: Dk & Enemy (z-enemy)

IMPORTANT:
For maximum performance make sure you have latest drivers 
http://www.nvidia.com/Download/index.aspx


This version includes a new way to manage and monitor the miner.

New features:
- Added new HTTP JSON API (see json_api_help.txt for the details), available at port 4067 by default
- Added web control panel with real-time monitoring and charts. 
  The UI is responsive and should be looking well on most mobile phones and tablets.

Other changes:
- The miner informs about API servers (both Telnet and HTTP) being started
- You can now disable both servers with --api-bind=0 and --api-bind-http=0 respectively
- Minor bugfixes and stability improvements

Notes:
- For HTTP server --api-allow command line option isn't having any effect (for now?)

_____________________________________
First time or troubleshooting x16:
-   First time users - all ver. 1.16+ works on Cuda 9.x and it is recommended to make sure you've updated your NVIDIA drivers. You can find drivers here: http://www.nvidia.com/Download/index.aspx ver., 398+++
-   Next important thing is intensity. We recommend intensity -20 at first.
-   X16r algo is very wild and eratic.  *Very important*  Make sure to have enough power reserve on PSU. Please be sure you have a minimum 20% headroom on your PSU or set your PL on 70-80% usage.
-   Using +core and -mem is useful but, use no OC at first until you verify stability. 


Performance and fine tuning x16: 
-   This release z-enemy 1.16 is reported to be more stable when it using higher PL (90-110%) and +core and -memory , feel free to experiment with it.
-   Updating drivers can provide more gains
-   Recommended intensity is 21 for Ti and 20-21 for 10x0
-   Recommended memory: 0  or -502
-   Recommended core +50+150 ( 1800-1900MHz 1080 Ti)
-   Overclock slowly and allow plenty of time to verify stability (12-24hrs) before making anymore adjustments. x16r is a very chaotic algorithm so just because it works for 1 hr doesn't mean you can't crash over longer time. Sometimes hash order can lead to 2000+mhz and crash system. Keep in mind – overclocking is always at your own risk!
-   Yiimp pools recommend  manual diff (-p d=16) - for  small farms or  (-p d=48 ) - for good farms like 5-6 1080 Ti   If you need to name your rigs as well as set diff you may try -p rigname,d=16
