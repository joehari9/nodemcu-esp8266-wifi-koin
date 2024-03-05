# Cara instalasi wifi koin dengan nodemcu esp8266 dan mikrotik
1. Pastika mikrotik sudah disetting utuk hotspot/voucher disini tidak akan disertakan cara setting hotspot/voucher di pastikan sudah bisa.<br>
2. Download file **loginpage.zip** dan upload ke mikrotik harap jangan di rubah folder wifikoin jika di rubah wifikoin tidak akan bekerja arahkan saja HTML directory hotspot pada server profile mikrotik ke folder wifikoin sehingga tapilan login akan tampak seperti dibawah.<br>
![loginpage png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/login.jpg) 
3. Pastikan semua part sudah siap yang terdiri dari:<br>
           1. multy koin acceptor (kalibrasi terlebih dahulu dan ingat urutannya)<br>
           2. nodemcu esp8266<br>
           3. dc stepdown dengan output 5 volt yang adjustable atau bukan atau bisa juga dengan ic 7805<br>
           4. 2 buah lampu led dengan warna berbeda (optional jika tidak ada lcd)<br>
           5. 3 buah resistor masing-masing berukuran 39k 10k dan 220 ohm<br>
           6. buzzer<br>
           7. adaptor 12 volt 2 ampere<br>
           8. lcd 20x4 sudah terpasang modul i2c (optional bisa pakai bisa juga tidak)<br>
           9. kabel seperlunya<br>
5. Download file **wifikoin.bin**<br>
6. Upload sketch ke nodemcu menggunakan esp8266 flasher untuk windows atau esp8266 loader untuk android<br>
7. Setelah sketch berhasil terupload ke nodemcu rangkaikan semmua komponen seperti pada diagram dibawah<br>
![diagram png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/diagram.jpg)<br>
8. tancapkan adaptor tunggu hingga muncul wifi degan nama ssid vending_setup <br>
9. hubungkan ke ssid vending_setup buka browser masukkan ip **192..168.4.1** akan terbuka halaman instalasi step 1<br>
10. isi semua form ,karena terhubung ke jarinngan hotspot yang tanpa password untuk kolom password pada seting ap/ssid bisa dikosongkan ,sedangkan untuk lisensi bisa di isi apa saja seperti gambar dibawah<br>
![install png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/istall-step1.jpg)<br>
11. klik simpan data dan selanjutya akan di arahkan ke step2<br>
![step2 png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/install-step2.png)<br>
12. copy semua text di text area lalu buka terinal mikrotik kemudia paste text tersebut lalu klik enter ,atau bisa juga binding manual copy mac address saja masuk winbox **ip->hotspot->ip binding->** paste mac address pilih type bypass<br>
13. selanjutnya login ke admin panel IP address, dapat dilihat di lcd saat loading start atau bisa dilihat dengan membuka browser kunjungi **alamat/ip login hotspot/host.txt** login dengan user password admin saat proses instalasi dan lengkapi semua setingan wifikoin ready <br>
![admin png](https://raw.githubusercontent.com/joehari9/nodemcu-esp8266-wifi-koin/main/screenshot/Screenshot_20240305_071420.jpg)
#### catatan : untuk trial hanya bisa membuat satu tarif dengan satu koin dan countdown timer 10 detik full feature dapatkan valid license
