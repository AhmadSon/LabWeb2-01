<body>
    <table border="1">
        <tr>
            <th> Nama</th>
            <th>NIM</th>
            <th>Kelas</th>
        </tr>
        <tr>
            <td>Ahmad Syukron</td>
            <td>312110056</td>
            <td>TI.21.A.1</td>
        </tr>
    </table>
</body>

# Layout Sederhana

## Tugas Latihan
- <b>Soal</b><p>
![Gambar 00](Image/TLatihan.PNG)<p>

- <b>index.html</b><p>
```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>

    <!-- CSS -->
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
        </header>
        <nav>
            <ul>
              <a href="index.html" class="active">Home</a>
              <a href="#article">Artikel</a>
              <a href="about">About</a>
              <a href="contact">Kontak</a>
            </ul>
          </nav>
      <section id="hero">
        <h1>Hello World!</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin
          in leo fringilla, vestibulum mi porta, faucibus felis. Integer
          pharetra est nunc, nec pretium nunc pretium ac.
        </p>
        <a href="#"
          ><button class="button" style="vertical-align: middle">
            <span>Learn more </span>
          </button></a
        >
      </section>
      <section id="wrapper">
        <section id="main">
          <div class="row">
            <div class="box">
              <img
                src="https://dummyimage.com/120/db7d25/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#"
                ><button type="button" class="button-img">
                  View detail
                </button></a
              >
            </div>
            <div class="box">
              <img
                src="https://dummyimage.com/120/3e73e6/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#"
                ><button type="button" class="button-img">
                  View detail
                </button></a
              >
            </div>
            <div class="box">
              <img
                src="https://dummyimage.com/120/71e6d4/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#"
                ><button type="button" class="button-img">
                  View detail
                </button></a
              >
            </div>
          </div>

          <hr class="divider" />
          <article id="article" class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </article>
          <hr class="divider" />
          <article class="entry">
            <h2>First featurette heading.</h2>
            <img
              src="https://dummyimage.com/150/7b8a70/fff.png"
              alt=""
              class="right-img"
            />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </article>
        </section>
        <aside id="sidebar">
          <div class="widget-box">
            <h3 class="title">Widget Header</h3>
            <ul>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
            </ul>
          </div>
          <div class="widget-box">
            <h3 class="title">Widget Text</h3>
            <p>
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </div>
        </aside>
      </section>
      <footer>
        <p>&copy; 2023 - Universitas Pelita Bangsa</p>
      </footer>
    </div>
  </body>
</html>
```
- <b>Tampilan Hasil Program</b><p>
![Gambar 01](Image/HLatihan.PNG)<p>


## Tugas Pratikum
- <b>Soal</b><p>
![Gambar 02](Image/TPratikum.PNG)<p>

- <b>Codingan</b><p>

```bash
x = {}

while True:
    header="PROGRAM INPUT NILAI MAHASISWA"
    print(header.center(97,"="))
    print()
    print("[ (L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar")
    c = input("Masukkan Pilihan: ")

    if c == 'T' or c == 't':
        print("TAMBAH DATA")
        nim = int(input("Masukkan NIM\t\t: "))
        nama = input("Masukkan Nama\t\t: ")
        tugas = int(input("Masukkan Nilai Tugas\t: "))
        uts = int(input("Masukkan Nilai UTS\t: "))
        uas = int(input("Masukkan Nilai UAS\t: "))
        akhir = tugas*.3 + uts*.35 + uas*.35
        x[nama] = nim, uts, uas, tugas, akhir

    elif c == 'U' or c == 'u':
        print("UBAH DATA")
        print("Cari Data Mahasiswa Menggunakan Nama")
        nama = input("Masukkan Nama Mahasiswa: ")
        if nama in x.keys():
            nim = int(input("Masukkan NIM yang benar\t\t: "))
            tugas = int(input("Masukkan Nilai Tugas yang benar\t: "))
            uts = int(input("Masukkan Nilai UTS yang benar\t: "))
            uas = int(input("Masukkan Nilai UAS yang benar\t: "))
            akhir = tugas*.3 + uts*.35 + uas*.35
            x[nama] = nim, uts, uas, tugas, akhir
        else:
            print("Nama {0} tidak ditemukan".format(nama))

    elif c == 'h' or c == 'H':
        print("HAPUS DATA")
        nama = input("Masukkan Nama untuk menghapus: ")
        if nama in x.keys():
            del x[nama]
        else:
            print("Nama {0} Tidak Ditemukan".format(nama))

    elif c == 'C' or c == 'c':
        print("CARI DATA")
        nama = input("Masukkan Nama : ")
        if nama in x.keys():
            print("="*73)
            print("|                             Daftar Mahasiswa                          |")
            print("="*73)
            print("| Nama            |       NIM       |  UTS  |  UAS  |  Tugas  |  Akhir  |")
            print("="*73)
            print("| {0:15s} | {1:15d} | {2:5d} | {3:5d} | {4:7d} | {5:7.2f} |"
                  .format(nama, nim, uts, uas, tugas, akhir))
            print("="*73)
        else:
            print("Nama {0} Tidak Ditemukan".format(nama))

    elif c == 'L' or c == 'l':
        if x.items():
            print("="*78)
            print("|                               Daftar Mahasiswa                             |")
            print("="*78)
            print("|No. | Nama            |       NIM       |  UTS  |  UAS  |  Tugas  |  Akhir  |")
            print("="*78)
            i = 0
            for z in x.items():
                i += 1
                print("| {no:2d} | {0:15s} | {1:15d} | {2:5d} | {3:5d} | {4:7d} | {5:7.2f} |"
                      .format(z[0][:13], z[1][0], z[1][1], z[1][2], z[1][3], z[1][4], no=i))
            print("=" * 78)
        else:
            print("="*78)
            print("|                               Daftar Mahasiswa                             |")
            print("="*78)
            print("|No. | Nama            |       NIM       |  UTS  |  UAS  |  Tugas  |  Akhir  |")
            print("="*78)
            print("|                                TIDAK ADA DATA                              |")
            print("="*78)

    elif c. lower() == 'k':
        break

    else:
        print("Pilih menu yang tersedia")

```
- <b>Hasil Program</b><p>
![Gambar 03](Image/HPratikum.PNG)
<p>

# END
![Gambar 04](Image/anime-love.gif)