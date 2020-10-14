# opencore-atheros-kext

## All Atheros kext that can feat with Opencore bootloader, working on latest Mac OS - [English](https://github.com/daniasefine/opencore-atheros-kext/blob/main/README_en.md) - www.firstplato.com

![](https://raw.githubusercontent.com/daniasefine/opencore-atheros-kext/main/img/2.png)

Pada repo ini, kamu bisa mendapatkan kext IO80211Family.kext yang telah dimodifikasi, khusus untuk device yang memakai Atheros40 (terinspirasi dari CtlnaAHCIPort.kext). Jadi kita tidak perlu melakukan perubahan apapun pada S/L/E atau L/E. Cukup inject saja via Opencore, dan akan bisa menjalankan Big Sur tanpa mengutak atik sistem (tidak perlu menghapus vanilla IO80211Family.kext di /S/L/E).

![](https://raw.githubusercontent.com/daniasefine/opencore-atheros-kext/main/img/0.png)

Maaf karena belum dicoba di Mojave dan Catalina, namun kita yakin pasti berjalan lancar juga koq. Silahkan beri feedback atau buat pull request, jika kamu mengalami isu, masalah atau memerlukan bantuan untuk melakukan patch Atheros tipe lain yang belum terlist di sini.

Apa yang perlu dilakukan :
- Cukup copas kedua kext, HS80211Family.kext & AirPortAtheros40.kext, pada EFI/OC/Kexts dan pastikan sudah melakukan inject via config.plist. Jangan melakukan inject IO80211NetBooter pada config.plist. Perhatikan gambar berikut : 

![](https://raw.githubusercontent.com/daniasefine/opencore-atheros-kext/main/img/1.png)

- Kamu dapat menambahkan sendiri dari VendorID di IONameMatch (atheros40) jika ID kamu belum ada.
- Berdasarkan tutorial dari om Maldon di Olarila untuk Wifi Atheros AR9565, AR9462, AR9463, AR9485 yang sudah dites dan lancar, berikut ini adalah file modifikasinya (tidak memerlukan injector) :

- [AR9565 AirPortAtheros40-9565.kext.zip](https://github.com/ipang-dwi/opencore-atheros-kext/raw/main/kext/AirPortAtheros40-9565.kext.zip)
- [AR9462 AirPortAtheros40-9462.kext.zip](https://github.com/ipang-dwi/opencore-atheros-kext/raw/main/kext/AirPortAtheros40-9462.kext.zip)
- [AR9463 AirPortAtheros40-9463.kext.zip](https://github.com/ipang-dwi/opencore-atheros-kext/raw/main/kext/AirPortAtheros40-9463.kext.zip)
- [AR9485 AirPortAtheros40-9485.kext.zip](https://github.com/ipang-dwi/opencore-atheros-kext/raw/main/kext/AirPortAtheros40-9485.kext.zip)

Feel free to reach us on :
- https://www.firstplato.com
- https://www.facebook.com
- admin@firstplato.com
- WhatsApp : [+62-8999-302-702](https://wa.me/628999302702)
