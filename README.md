
Nama : Ahmad Syukron<p>
NIM  : 312110056<p>

### Program nilai random
1. Tampilkan n bilangan acak yang lebih kecil dari 0.5.
2. nilai n diisi pada saat runtime
3. anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya
4. gunakan fungsi random() yang dapat diimport terlebih dahulu
- <b>Program</b><p>
```bash
from random import random
n = int(input("Masukkan nilai N: "))
for i in range(n):
    while 1:
        n = random()
        if (n < 0.5):
            break
    print("data ke: ",i, "=>",n)
print("Selesai")
```
![Gambar 01](Image/NilaiRandom.PNG)<P>
- <b>Hasil program</b><p>
![Gambar 02](Image/HasilNilaiRandom.PNG)<P>
<p>

## Latihan 2
### Program mencari bilangan terbesar
1. Buat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan. Masukkan angka 0 untuk berhenti.<P>
- <b>program</b><p>
```bash
max = 0
while True:
    n = int(input("Masukkan bilangan: "))
    if max < n :
        max = n
    if n == 0:
        break
print("Bilangan terbesar adalah: ",max)
```
![Gambar 03](Image/NilaiTerbesar.PNG)<p>
- <b>penjelasan</b><p>
max () adalah fungsi bulid-in untuk mencari nilai tertinggi<p>
- <b>Hasil Program</b><p>
![Gambar 04](Image/HasilNilaiTerbesar.PNG)
<p>

## Latihan 3
### Program perulangan bertingkat
- <b>Program input</b><p>
```bash
for i in range(0, 10):
  for j in range(10):
    print('%3d'%(i+j), end = ' ')
  print(' ')
```
![Gambar 07](Image/PerulanganBertingkat.PNG)
- <b>Hasil program</b><p>
![Gambar 08](Image/HasilPerulanganBertingkat.PNG)
<p>

## Program 1
### program sederhana dengan perulangan
- <b>Seorang pengusaha menginvestasikan uangnya untuk memulai usahanya dengan modal awal 100 juta, pada bulan pertama dan kedua belum mendapatkan laba. pada bulan ketiga baru mulai mendapatkan laba sebesar 1% dan pada bulan ke 5, pendapatan meningkat 5%, selanjutnya pada bulan ke 8 mengalami penurunan keuntungan sebesar 2%, sehingga laba menjadi 3%. Hitung total keuntungan selama 8 bulan berjalan usahanya.</b><p>
- <b>program input</b><p>
```bash
a = 100000000
for i in range(1, 9):
    if (i >= 1 and i <= 2):
        b = a * 0
        print("Laba bulan ke- ", i, "Sebesar: ", b)
    if (i >= 3 and i <= 4):
        c = a * 0.1
        print("Laba bulan ke- ", i, "sebesar: ", c)
    if (i >= 5 and i <= 7):
        d = a * 0.5
        print("Laba bulan ke- ", i, "sebesar: ", d)
    if (i == 8):
        e = a * 0.2
        print("Laba bulan ke- ", i, "sebesar: ", e)
        total = b + b + c + c + d + d + d + e
        print = ("\nTotal : ", total)
```
![Gambar 05](Image/Hitung.PNG)
- <b>Hasil program</b><p>
![Gambar 06](Image/HasilHitung.PNG)
<p>

# Terima Kasih