# opencore-atheros-kext

## All Atheros kext that can feat with Opencore bootloader, working on latest Mac OS - www.firstplato.com

![](https://raw.githubusercontent.com/daniasefine/opencore-atheros-kext/main/img/2.png)

In this repo you will find modified IO80211Family.kext, especially who use device based on Atheros40 (the idea came from CtlnaAHCIPort.kext). So we don't need to touch /S/L/E and or L/E. Just inject via OpenCore, and we can running Big Sur without open Sealed (no need remove/delete vanilla IO80211Family.kext in /S/L/E)

![](https://raw.githubusercontent.com/daniasefine/opencore-atheros-kext/main/img/0.png)

I'm not try in Mojave or Catalina but I'm sure is worked too. Please give feedback or open pull request, if you face any issue, trouble or need help to patch the other one.

What you need to do :
- Just put 2 kext, HS80211Family.kext & AirPortAtheros40.kext, on EFI/OC/Kexts and make sure inject via config.plist. Do not inject IO80211NetBooter in the plist (must do research so i leave there in plugin),  I remove IO80211NetBooter from plugin so as not to confuse. See my picture below just add 2 value :

![](https://raw.githubusercontent.com/daniasefine/opencore-atheros-kext/main/img/1.png)

- You can add value manually from VendorID in IONameMatch (atheros40) if your ID not present.
- Refer to MaLd0n guide in olarila for working Wifi Atheros AR9565, AR9462, AR9463, AR9485 here is the modification (no need injector) :

[AR9565 AirPortAtheros40-9565.kext.zip]()
[AR9462 AirPortAtheros40-9462.kext.zip]()
[AR9463 AirPortAtheros40-9463.kext.zip]()
[AR9485 AirPortAtheros40-9485.kext.zip]()

Feel free to reach us on :
- https://www.firstplato.com
- https://www.facebook.com
- admin@firstplato.com
- WhatsApp : [+62-8999-302-702](https://wa.me/628999302702)
