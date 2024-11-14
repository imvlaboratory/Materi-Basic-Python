# TIPE DATA

Tipe data merupakan klasifikasi dari data yang disimpan dalam variabel. Pada python, tipe data dibagi menjadi 2 kategori utama, yaitu :

## **Tipe Data Primitif**

Merupakan tipe data dasar dari berbagai bahasa pemrograman, salah satunya python. Pada python sendiri tipe data primitif adalah sebagai berikut :

- Integer

  Tipe data yang menyimpan bilangan bulat. Integer dapat berupa bilangan bulat positif, negatif, atau nol.

  ```
  umur = 20
  tahun = 2000
  nilai = 0
  suhu = -10
  ```

- Float

  Tipe data untuk bilangan desimal. Dapat berupa bilangan desimal positif, negatif, atau nol.

  ```
  tinggi = 121.1
  suhu = 0.0
  ```

- String

  Tipe data yang menyimpan text. Dapat berupa karakter, kata, kalimat, atau bahkan paragraf.

  ```
  nama = 'Andini'
  status = "Mahasiswi"

  multi_line = """ dengan tipe data ini bisa buat paragraf, puisi, dll"""
  ```

- Boolean

  Tipe data untuk menyimpan nilai logika.

  ```
  True or False aja pokoknya.

  a = True
  b = False
  c = not a # False
  d = not b # True
  ```

## **Tipe Data Kompleks**

Tipe data yang didalamnya terdapat atau terdiri dari berbagai macam tipe. Tipe data kompleks pada python adalah sebagai berikut :

- List
  Tipe data yang dapat menyimpan kumpulan data. List dapat berupa kumpulan bilangan, string, atau kumpulan data kompleks lainnya.

  ```
  siswa = ["Andi", "Budi", "Citra"]
  print("Daftar siswa:", siswa)

  # Menambah elemen
  siswa.append("Dedi")
  print("Setelah menambah Dedi:", siswa)

  # Mengubah elemen
  siswa[1] = "Bayu"
  print("Setelah mengubah Budi menjadi Bayu:", siswa)

  # Menghapus elemen
  siswa.remove("Citra")
  print("Setelah menghapus Citra:", siswa)
  ```

* Tuple

  Tipe data yang berfungsi menyimpan kumpulan data yang tidak dapat diubah (Immutable). Tuple dapat berupa kumpulan bilangan, string, atau kumpulan data kompleks lainnya.

  ```
  koordinat = (10, 20, 30)
  print("Koordinat:", koordinat)

  # Mengakses elemen dengan indeks
  x = koordinat[0]
  y = koordinat[1]
  z = koordinat[2]
  print(f"x: {x}, y: {y}, z: {z}")
  ```

* Set

  Merupakan kumpulan data yang tidak memiliki urutan.

  ```
  tag = {"python", "programming", "tutorial"}
  print("Tag:", tag)

  # Menambah elemen ke dalam set
  tag.add("coding")
  print("Setelah menambah 'coding':", tag)

  # Menghapus elemen dari set
  tag.remove("tutorial")
  print("Setelah menghapus 'tutorial':", tag)

  # Melakukan operasi himpunan
  tag_baru = {"coding", "learning"}
  gabungan = tag.union(tag_baru)  # gabungan set
  print("Gabungan tag:", gabungan)

  irisan = tag.intersection(tag_baru)  # irisan set
  print("Irisan tag:", irisan)
  ```

* Dictionary

  Tipe data yang digunakan untuk menyimpan pasangan **key** - **value** (kunci-nilai). Directory dapat digunakan untuk menyimpan data dalam bentuk tabel. Setiap item dipisahkan oleh tanda titik dua `:`

  ```
  profil = {
    "nama": "Alice",
    "umur": 25,
    "kota": "Jakarta"
  }
  print("Profil pengguna:", profil)

  # Mengakses nilai dengan kunci
  print("Nama:", profil["nama"])
  print("Umur:", profil["umur"])

  # Menambah atau mengubah nilai
  profil["pekerjaan"] = "Programmer"  # menambah kunci baru
  profil["umur"] = 26  # mengubah nilai umur
  print("Profil setelah update:", profil)

  # Menghapus elemen dengan kunci
  del profil["kota"]
  print("Profil setelah menghapus kota:", profil)
  ```

Setelah membahas berbagai macam Type data yang ada, selanjutnya kita akan membahas tentang perbedaan dari set, list, dictionary, dan tuple berdasarkan beberapa aspek, mulai dari **mutabilitas**, **indeks**, **duplikasi**, **penggunaan memory**, **fleksibilitas**, dan **kasus penggunaan**.

![14](../assets/14.png "14.png")

- Mutabilitas

  - **Mutable** : Data dapat dimodifikasi, ditambah, atau dihapus setelah membuat.

  * **Immutable** : Data tidak dapat diubah setelah didefinisikan. Jika mau diubah harus membuat ulang struktur datanya.

- Indeks

  - **Indeks** : Struktur data yang memiliki posisi tertentu untuk setiap elemen, sehingga elemen dapat diakses menggunakan indeks (Kunci untuk Dictionary).

  * **Tidak Indeks** : Elemen tidak memiliki memiliki urutan posisi.

- Duplikasi

  - **Dapat Diduplikasi** : Elemen yang sama dapat ditambahkan berkali-kali.

  * **Tidak Mengizinkan Duplikasi** : Elemen harus unik dan tidak boleh ada elemen identik.

- Penggunaan Memori

  - Struktur data yang **Mutable** biasanya menggunakan lebih banyak memori karena perlu menyediakan ruang untuk perubahan.

  * Struktur data yang **Imutable** sering kali lebih efisien dalam penggunaan memori.

- Fleksibilitas

  - Struktur data yang **Fleksibel** bisa digunakan diberbagai kasus dan bisa disesuaikan untuk berbagai kebutuhan.

  * Struktur data **Kurang Fleksibel** memiliki kegunaan yang terbatas, tetapi lebih efisien atau aman untuk data tetap.
