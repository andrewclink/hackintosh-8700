High Sierra & Coffee Lake
========================

October 2017

* i7-8700
* Z370m/ac
    * ALC892
	* Intel Graphics (0x3e92)
	* M.2 SSD (in SATA mode)

Clover
-------

Config.plist is usually what you want to use, but not always.
Experimental changes are made there occasionally, and in those cases there will be a previously known-good working config, usually `config-CFL.plist` or `config-KBL.plist` depending on what system you're booting.

At this time no macOS supports CFL processors; the difference between the CFL and KBL configs is the integrated GPU device ID. In 10.13.0 the IGPU in the CFL processors matches AppleIntelKBLGraphics but acceleration is not achieved. Use KBL until Apple updates their drivers.

Sierra did not support Kaby Lake processors prior to 10.12.6, and on those you'll need to spoof the CPU as a Sky Lake model— use `config-SKL.plist`. 

