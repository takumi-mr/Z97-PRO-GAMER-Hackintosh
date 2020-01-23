# Z97-PRO-GAMER-Hackintosh
config.plist and kexts to boot Catalina or Mojave with Z97-PRO-GAMER (ASUS)

GPU : RX570
CPU : i7 4790k

kext list  
* FakeSMC.kext
* Lilu.kext
* WhateverGreen.kext
* AppleALC.kext
* USBInjectAll.kext
* AHCI_Intel_Generic_SATA.kext
* IntelMausiEthernet.kext
* FakeSMCSensor**.kext

You may have to change below  

    ```
    <key>Boot</key>
	<dict>
        ...
		<key>Arguments</key>
		<string>dart=0 uia_exclude=HS02;HS08;HS11;HS12;SS02</string>
	    ...
	</dict>
    ``` 
This make total of using USB port 15 in my env.  
But the port you use is differ from me.  
so if you use as it is, Some USB port cannot work.  
I recommend delete the args or change port to use.

