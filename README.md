# Lapres Jarkom - Modul 2 - T12
## Oleh
- Anggada Putra Nagamas – 05311840000025
- Mohammad Ifaizul Hasan – 05311840000029

## Soal Shift Modul 4 Subnetting & Routing
![Gambar 1](Images/Soal%20Shift%20Modul%204.png)

**Keterangan**
- Cloud diberikan IP TUNTAP
- Server diberikan IP DMZ
- Setiap UML diberikan memori sebesar 64MB

## Pengerjaan
## VLSM (Variable Length Subnet Masking) Pada Cisco Packet Tracer (CPT)
**Langkah 1**
- Buat pembagian subnet dan hitung subnet pada tiap bagian seperti gambar berikut ini:

![Gambar 2](Images/Pembagian_Subnet.png)

**Langkah 2**
- Hitung IP Address yang dibutuhkan (Jumlah Host, Router, dan Server). Pada soal ini ada kurang lebih 5845 IP Address maka subnet yang dipakai untuk membuat pohon IP yaitu subnet 19. 

| Nama | Jumlah IP | Netmask |
|--|--|--|
| A1 | 721 | /22 |
| A2 | 252 | /24 |
| A3 | 2 | /30 |
| A4 | 2 | /30 |
| A5 | 521 | /22 |
| A6 | 13 | /28 |
| A7 | 502 | /23 |
| A8 | 2 | /30 |
| A9 | 2 | /30 |
| A10	| 701 | /22 |
| A11	| 2 | /30 |
| A12	| 2021 | /21 |
| A13	| 101 | /25 |
| A14	| 2 | /30 |
| A15	| 1001 | /22 |
| **Total** | **5845** | **/19** |

- Buat pohon IP berdasarkan pembagian subnet yang ada pada topologi seperti gambar berikut ini:

![Gambar 3](Images/VLSM.PNG)
**Keterangan :**
- Untuk Server, IP yang digunakan yaitu IP DMZ tiap kelompok.

**Langkah 3**
- Lakukan konfigurasi pada Router, Client, Server, dan Cloud.



