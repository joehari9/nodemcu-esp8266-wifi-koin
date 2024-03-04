# Cara instalasi wifi koin dengan nodemcu esp8266 dan mikrotik
1. Pastika mikrotik sudah disetting utuk hotspot/voucher disini tidak akan disertakan cara setting hotspot/voucher di pastikan sudah bisa.<br>
2. Download file **loginpage.zip** dan upload ke mikrotik harap jangan di rubah folder wifikoin jika di rubah wifikoin tidak akan bekerja arahkan saja HTML directory hotspot pada server profile mikrotik ke folder wifikoin sehingga tapilan login akan tampak seperti dibawah.<br>
<p align="center">
           ![image.png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/loginpage.jpg) 
</p>
3. Pastikan semua part sudah siap yang terdiri dari:<br>
           1. multy koin acceptor.<br>
           2. nodemmcu esp8266<br>
           3. dc stepdown dengan output 5 volt yang adjustable atau bukan atau bisa juga dengan ic 7805<br>
           4. 2 buah lampu led dengan warna berbeda<br>
           5. adaptor 12 volt 2 ampere<br>
           6. lcd 20x4 sudah terpasang modul i2c (optional bisa pakai bisa juga tidak)<br>
           7. kabel seperlunya<br>
4. Download file wifikoin.bin<br>
5. Upload sketch ke nodemcu menggunakan esp8266 flasher untuk windows atau esp8266 loader untuk android<br>
6. Setelah sketch berhasil terupload ke nodemcu rangkaikan semmua komponen seperti pada diagram dibawah<br>
![image.png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/diagram.jpg)
