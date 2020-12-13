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

**Konfigurasi pada SURABAYA -> TULUNGAGUNG**
- Atur IP pada interface SURABAYA yang mengarah ke BATU dengan 192.168.0.5.

![Gambar 4](Images/VLSM1.PNG)
- Atur IP pada interface BATU yang mengarah ke SURABAYA dengan 192.168.0.6.

![Gambar 5](Images/VLSM2.PNG)

- Atur IP pada interface BATU yang mengarah ke KEDIRI dengan 192.168.0.1.

![Gambar 6](Images/VLSM3.PNG)
- Atur IP pada interface KEDIRI yang mengarah ke BATU dengan 192.168.0.1.

![Gambar 7](Images/VLSM4.PNG)
- Atur IP pada interface KEDIRI yang mengarah ke BLITAR dengan 192.168.1.1.

![Gambar 8](Images/VLSM5.PNG)
- Atur IP pada interface BLITAR yang mengarah ke KEDIRI dengan 192.168.1.2.

![Gambar 9](Images/VLSM6.PNG)
- Selanjutnya atur IP pada subnet A1 & A2. 
- Atur IP pada interface KEDIRI yang mengarah ke LUMAJANG dengan 192.168.1.1.

![Gambar 10](Images/VLSM5.PNG)
- Atur IP pada interface BLITAR yang mengarah ke TULUNGAGUNG dengan 192.168.12.1.

![Gambar 11](Images/VLSM7.PNG)
Atur IP pada client dengan cara :
- Masuk ke client
- Pilih tab Desktop
- Pilih IP Configuration

- Atur IP pada IP Configuration LUMAJANG yang mengarah ke KEDIRI dengan 192.168.1.3.

![Gambar 12](Images/VLSM8.PNG)
- Atur IP pada IP Configuration TULUNGAGUNG yang mengarah ke BLITAR dengan 192.168.12.2.

![Gambar 13](Images/VLSM9.PNG)
Lakukan hal yang sama untuk mengatur alamat IP setiap interface pada device yang ada dalam topologi. Setelah selesai, lakukan langkah selanjutnya yaitu Routing agar topologi dapat berfungsi dengan semestinya.
