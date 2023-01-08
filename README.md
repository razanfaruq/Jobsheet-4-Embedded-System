# Jobsheet-4-Embedded-System
### Cara Kerja Sensor Membaca Data dan Dikirim ke Database

#### Alat dan Bahan yang Digunakan
1. ESP32
2. Breadboard
3. Sensor DHT11 atau DHT22
4. Kabel Jumper
5. Lampu LED

#### I. Cayenne (MQTT) Sensor Button Website Monitoring
Pada Jobsheet 4 ini, menggunakan website Cayenne untuk mengontrol LED yang telah terhubung dengan sensor suhu (supaya dapat mengukur berapa derajat suhu dalam satuan Celcius dan kelembabannya) dan ESP32 yang sudah dimasukkan program cayennesensorsuhu.ino. Dimana, saat simbol LED pada website cayenne diklik ON, maka lampu LED yang terhubung pada ESP32 akan ON. Sebaliknya, saat simbol lampu LED pada cayenne di-OFF-kan, maka lampu LED yang terhubung ke ESP32 akan OFF. Selain itu, pada website tersebut juga dapat menampilkan suhu yaitu pada channel 1 dengan satuan Celcius dan kelembaban pada channel 2. Berikut ini adalah dokumentasi hasilnya.


https://user-images.githubusercontent.com/118172386/211182880-138f4aca-cff3-4e70-9b0d-ca5121cb6c8d.mp4

Hasil dari program yang dijalankan.

![210519993-8292af25-f3e0-4068-8599-541414e60f95](https://user-images.githubusercontent.com/118172386/211182989-2d28970c-e17e-4084-a306-15286aa70c8c.jpg)

Channel 1 menampilkan suhu dalam satuan derajat Celcius, channel 2 menampilkan kelembaban, dan simbol lampu LED sebagai indikator sekaligus tombol ON/OFF lampu LED yang terhubung pada ESP32.

#### II. Adafruit.IO+Sensor+LED+Suara
Percobaan selanjutnya yaitu membutuhkan library adafruit IO (MQTT) yang kemudian ditambah LED sebagai indikator untuk mengetahui apakah sensor tersebut bekerja. Kemudian data disimpan ke database lalu Google Assistan yang akan mengendalikannya.

<img width="906" alt="211001238-2e07925a-bc5d-43f0-ba17-6e55e99538fe" src="https://user-images.githubusercontent.com/118172386/211183115-4f7bd1c9-ff37-44e4-8ce1-4fffc75874aa.png">

<img width="896" alt="211001105-1a85dce7-babe-43f0-a264-cc424d432cc1" src="https://user-images.githubusercontent.com/118172386/211183116-18fad760-5b5f-4df2-8cfe-29d5bab110fe.png">

![210932884-070680e2-a6f1-4e45-b3cd-b4082061a005](https://user-images.githubusercontent.com/118172386/211183126-78e384f0-81d5-4b7c-9762-fdff1f41a177.png)


#### III. Thing Speak+Sensor
Percobaan selanjutnya percobaan yang ketiga menggunakan sensor DHT 11 untuk membaca suhu dan kelembapan udara. Data dari sensor kemudian di kirim ke ThingSpeak untuk menampilkan data yang dibaca oleh sensor tadi. Data yang ditampilkan berupa chart atau diagram.

![211070609-aca11c56-bc3e-460d-a59a-0f5301b70201](https://user-images.githubusercontent.com/118172386/211183179-58e1b3b8-5cf4-40e5-ba55-6f6a9b83c7eb.jpg)

Setelah membuat rangkaian seperti diatas masukkan program seperti pada thinkspeaksensor.io, maka hasilnya akan seperti dibawah.

![211070782-2d943257-a687-4188-860b-cea6a600d7fe](https://user-images.githubusercontent.com/118172386/211183184-69279459-53f6-49de-9e91-4a7d83651163.jpg)

![211070803-22d74764-23cd-4888-8696-360fe239b5ea](https://user-images.githubusercontent.com/118172386/211183189-1d34ac06-699e-46d4-83af-7a9d6cef875d.jpg)

#### IV. ESP Now+IOT

![211071008-a7794705-ccec-4b8e-9257-5be82d87ccd4](https://user-images.githubusercontent.com/118172386/211183329-e286c2b5-3f74-4047-a38a-3dbe158840cb.png)
![211070961-2bbe8a6d-8def-4a1b-b878-4755ee589a4a](https://user-images.githubusercontent.com/118172386/211183331-01b48a56-c69d-4659-a1fc-8f8a1aff0b49.jpg)


