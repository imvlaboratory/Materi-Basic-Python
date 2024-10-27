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
  H = "Hello world!"
  x = 'ur my ex'
  j = '11'

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
  angka = [1,1,2,3,4,10] # List of integer
  nama = ["Nur", "Winana", "Nisa"] # List of string
  data = [1, "IMV", True, (1,0.5,8)] # List of mixed data types
  ```

* Tuple

  Tipe data yang berfungsi menyimpan kumpulan data yang tidak dapat diubah (Immutable). Tuple dapat berupa kumpulan bilangan, string, atau kumpulan data kompleks lainnya.

  ```
  Acara_imv = ("openlab", "IMV Transfer Learning") # Tuple of string
  data = (1, "Dini", 2021, "Asisten IMV") # tuple of mixed types
  ```

* Set

  Merupakan kumpulan data yang tidak memiliki urutan.

  ```
  bilangan = {1,2,0,100,-2,0.4} # Set of Numerik
  lab = {'IMV', '2023', "kaya! Kaya! Kaya!"} # Set of String
  mixed = {1, "Jhon doe", True} # Set of Mixed types
  ```

* Dictionary

  Tipe data yang digunakan untuk menyimpan pasangan **key** - **value** (kunci-nilai). Directory dapat digunakan untuk menyimpan data dalam bentuk tabel. Setiap item dipisahkan oleh tanda titik dua `:`

  ```
  biodata = {
  'nama' : 'Muhammad Dawwam',
  'alamat': 'Telkom University Landmark Tower Lantai 11 no 08 (TULT 11.08)',
  'jurusan': 'Teknik Telekomunikasi',
  'umur': 78,
  'is_married': True,
  'tinggi_badan': 309.62,
  'laboratorium': ('Daskom','IMV'),
  'murid': {
    'nama': 'Ridwan Maulana Tanjung',
    'alamat': 'Perumahan Bogor Ogah Geser Blok B1, No 7',
    'jurusan': 'Teknik Fisika',
    'is_married': False,
    'matkul_fav': ['Kalkulus', 'Pengolahan Sinyal', 'Elektromagnetika', 'Fisika Modern'],
    }
  }
  ```

Setelah membahas berbagai macam Type data yang ada, selanjutnya kita akan membahas tentang perbedaan dari set, list, dictionary, dan tuple berdasarkan beberapa aspek, mulai dari **mutabilitas**, **indeks**, **duplikasi**, **penggunaan memory**, **fleksibilitas**, dan **kasus penggunaan**.

- Mutabilitas

  - **Set** : Mutable, element dapat diubah setelah pembuatan.
  - **List** : Mutable, element dalam list dapat diubah, ditambah, atau dihapus.
  - **Dictionary** : Mutable, kunci dan nilai dalam dictionary dapat diubah.
  - **Tuple** : Immutable, element dalam tuple tidak dapat diubah setelah pembuatan

- Indeks

  - **Set** : Tidak dapat diindeks karena elementnya tidak diurutkan
  - **List** : Dapat diindeks, element-element dalam list diakses dengan indeks.
  - **Dictionary** : Tidak dapat diindeks menggunakan angga, tetapi harus menggunakan kunci.
  - **Tuple** : Dapat diindeks, element-element dalam tuple dapat diindeks.

- Duplikasi

  - **Set** : Tidak mengizinkan element duplikat, hanya element unik yang diterima.
  - **List** : Dapat memiliki element duplikat, element dnegan nilai yang sama dapat muncul lebih dari sekali.
  - **Dictionary** : Tidak mengzinkan kunci duplikat, tetapi nilai-nilai dapat diduplikat.
  - **Tuple** : Dapat memiliki element duplikat, element yang sama dapat muncul lebih dari sekali.

- Penggunaan Memori

  - **Set** : Menggunakan lebih banyak memori karena harus mempertahankan elemen-elemen unik dan melakukan operasi hash untuk memastikan keunikan.
  - **List** : Menggunakan lebih banyak memori dari pada tuple karena memungkinkan elemen duplikat dan perlu menyimpan urutan elemen.
  - **Dictionary** : Menggunakan lebih banyak memori karena perlu menyimpan pasangan kunci-nilai dan melakukan operasi hash untuk mengakses nilai berdasarkan kunci.
  - **Tuple** : Menggunakan memori lebih sedikit dibandingkan list karena elemennya immutable.

- Fleksibilitas

  - **Set** : Tidak terurut, tidak dapat diindeks, dan fokus pada operasi set seperti gabungan, irisan, dan perbedaan.
  - **List** : Terurut, dapat diindeks, dan lebih fleksibel untuk modifikasi, penambahan, penghapusan elemen.
  - **Dictionary** : Tidak terurut (di Python sebelum versi 3.7), memungkinkan penyimpanan data yang terstruktur menggunakan pasangan kunci-nilai.
  - **Tuple** : Terurut, dapat diindeks, dan lebih aman karena immutable.

- Kasus Penggunaan
  - **Set** : Cocok untuk menyimpan elemen unik, melakukan operasi matematika seperti gabungan, irisan, atau perbedaan set.
  - **List** : Cocok untuk menyimpan dan mengelola kumpulan data yang dapat diubah-ubah, seperti daftar item atau log data.
  - **Dictionary** : Berguna untuk merepresentasikan data yang membutuhkan pasangan kunci-nilai, seperti konfigurasi, entitas terstruktur, atau data yang membutuhkan akses berdasarkan kunci.
  - **Tuple** : Digunakan ketika data harus tetap konstan, seperti kumpulan data yang relevan seperti nama, usia, dll., yang tidak boleh diubah.
