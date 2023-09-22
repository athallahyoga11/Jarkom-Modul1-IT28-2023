 
# Lapres Modul 1 Jarkom IT28
## Yoga Hartono - 5027211023
## Athallah Narda Wiyoga - 5027211041 

### Soal 1
<img width="603" alt="Screenshot 2023-09-22 at 14 07 01" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/b1b1d024-fd05-49f3-8859-22da5c2231c2">

Melakukan filtering string yang berisikan "STOR", lalu akan terdapat Sequence Number dan Acknowledgement Number. Untuk responsesnya dilakukan hal yang sama untuk mendapatkan Sequence Number dan Acknowledgement Numbernya. Setelah itu lakukan nc dan akan didapatkan flagnya

### Soal 2
<img width="593" alt="Screenshot 2023-09-22 at 14 07 53" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/e37d0624-2b2a-4207-b662-1738651859d8">
<img width="601" alt="Screenshot 2023-09-22 at 14 08 13" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/7ce97035-af86-4495-b74f-524ea15c1253">

Melakukan follow tcp stream, lalu cari hingga menemukan nama servernya yang bernama gunicorn. Setelah itu, jalankan nc dan akan muncul perintah untuk menginput nama server gunicorn, jika benar maka akan langsung muncul flagnya

### Soal 3
Filter query yang digunakan untuk mengetahui berapa  paket yang terkumpul dengan alamat IP sumber dan tujuan 239.255.255.250 dengan port 3702 adalah dengan menggunakan “ip.addr == 239.255.255.250 and udp.port == 3702”, lalu hitung  yang tersedia paket, seperti gambar https berikut:
<img src="https://i.ibb.co/Bnqb8h0/Whats-App-Image-2023-09-18-at-21-36-59.jpg">

Dari gambar berikut, banyak paket yang tersedia sebanyak 21 paket untuk menjawab pertanyaan a dan protokol yang digunakan adalah UDP untuk menjawab pertanyaan b. Kemudian akses nc yang disediakan dan jawab pertanyaan a dan b dengan benar.
<img src="https://i.ibb.co/bKrDvmN/3b.png">

### Soal 4
Pertama buka file pcap, lalu cari paket 130, lalu cari checksum.
![4a](https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/89679766/17c2af0b-f944-4a7c-a4a1-23e94dc68930)

Didapatkan nilai checksumnya 0x18e5, masukkan pada nc
![4b](https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/89679766/a0ecab59-8cd3-4d9d-802f-cd8ad0b25b1e)


### Soal 5
<img width="601" alt="Screenshot 2023-09-22 at 14 08 54" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/7d26d4bf-2e50-4b4e-a923-0df9bde57748">

Melakukan follow tcp stream, maka akan didapatkan password yang masih belum dicode. Setalah itu, dicode terlebih dahulu passwordnya hingga mendapatkan passeord yang benar, setelah menginput password maka akan mendapatkan command untuk melakukan nc

### Soal 6


### Soal 7
<img width="1512" alt="Screenshot 2023-09-22 at 14 10 04" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/1d7b30b7-a53e-4804-a5e1-3e665a24b70f">
<img width="598" alt="Screenshot 2023-09-22 at 14 10 21" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/41aa60a5-47c9-4780-9ff9-708430083814">

Melakukan filter menggunakan command "ip.addres == 184.87.193.88" maka akan bisa mengetahui berapa jumlah packet yang masuk ke ip tersebut yang sesuai dengan perintah saat telah melakukan nc. Setelah itu, input berapa jumlah packet yang sesuai dan akan langsung mendapatkan flagnya

### Soal 8
<img width="598" alt="Screenshot 2023-09-22 at 14 10 52" src="https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/112833954/2cbc7443-a425-4512-ad30-cd0ca8f1d5ff">

Masukkan kueri filter agar wireshark hanya mengambil protokol yang menuju ke port 80 dengan menggunakan tcp.dstport == 80 || udp.dstport == 80. Setalah itu, langsung masukkan kedalam nc dan akan mendapatkan flagnya

### Soal 9
Permintaan filter untuk Wireshark untuk hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak  ke alamat 10.39.55.34 adalah "ip.src == 10.51.40.1 && ip.dst != 10.39.55.34" . Kemudian masukkan kueri  sebagai respons setelah akses nc diberikan, maka didapatkan flag seperti gambar dibawah.
![Uploading 9.png…]()

### Soal 10
Pertama buka file pcap, lalu tekan protokol untuk mengurutkan protokol. Kemudian, cari protokol TELNET dan ikuti aliran TCP. Nanti, miliki beberapa nama pengguna dan kata sandi dan coba satu per satu di NC.
Nantinya Anda akan mendapatkan user dan password dan memasukkannya ke NC
![10](https://github.com/athallahyoga11/Jarkom-Modul1-IT28-2023/assets/89679766/61807357-70ec-4f9c-876c-3ed6a7d7d304)




